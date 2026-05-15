# Calling grandMA3's Native Preset Picker from a Plugin

**Status:** VERIFIED — Tier-1 (onPC 2.3.2, hardware + screenshot confirmed)
**Headline:** A user plugin *can* open MA's real native list picker and get the
selected object back. No recreation, no file injection, no native patching.

## The mechanism

`PopupInput{}` is an **engine-provided global** (no Lua definition anywhere in
the resource tree; used by MA's own menus and the systemtests). It opens MA's
real native popup, **blocks** until the user picks/cancels, and returns the
selection.

### Signature (dumped verbatim by the engine on bad args)

```
PopupInput({ title:str, caller:handle, items:table, selectedValue:str,
             x:int, y:int, target:handle,
             render_options:{left_icon,number,right_icon},
             useTopLeft:bool, properties:{prop:value},
             add_args:{FilterSupport='Yes'/'No'} })
  returns  integer:selected_index, string:selected_value
```

- `items` = array of `{ kind, label, value }`, `kind` ∈ `'str'|'int'|'lua'|'handle'`.
  For objects use `{ 'handle', tostring(obj.Name), obj }`.
- `selected_value` comes back as a **handle string** like `#4000086B`.
  `StrToHandle("#4000086B")` → the real object.
- `selected_index` is the 1-based index into `items`.
- Returns immediately with `nil` (no signature error) if the popup is torn down
  before it can run — see caller lifecycle.

### Caller lifecycle — the one gotcha

`caller` must be a **real, initialized, on-screen** UIObject. A degenerate
(`W=1,H=1`) caller, or deleting the caller before/at the call, makes the popup
flash for a frame and return `nil`. Correct recipe:

```lua
local so     = (GetFocusDisplay() or GetDisplayByIndex(1)).ScreenOverlay
local caller = so:Append("BaseInput")
caller.Name = "PickCaller"; caller.W = "400"; caller.H = "120"
caller.AlignmentH = "Center"; caller.AlignmentV = "Center"
caller:WaitInit()
coroutine.yield({ ui = 1 })          -- realize it on screen (valid AbsRect)

local idx, val = PopupInput{ title="Select", caller=caller, items=items,
                             x=600, y=360, render_options={left_icon=true,number=true} }

caller:CommandDelete()               -- safe: PopupInput blocked, has returned
```

`PopupInput` **blocks** (measured `dt≈4s` of user interaction) — it is fully
synchronous from a plugin coroutine. Do all readback after it returns.

## Minimal preset picker

```lua
local function PickPreset(poolNo)
    local pool = DataPool().PresetPools[poolNo or 1]
    local items = {}
    for _, pr in ipairs(pool:Children()) do
        if pr and not pr:IsEmpty() then
            items[#items+1] = { 'handle', tostring(pr.Name), pr }
        end
    end
    local idx, raw = PopupPick("Select Preset", items)   -- see caller recipe
    if not idx then return nil end                        -- cancelled
    return StrToHandle(tostring(raw)), idx                 -- real Preset handle
end
```

Reusable implementation: `gma3_library/datapools/plugins/TaterProbes/TaterPickPreset.lua`
(exports `signalTable.PickPreset` / `signalTable.PopupPick`).

## Related — the menu registry (also VERIFIED)

- `Root().Menus` is a live, name-indexed registry of all 547 XML `<Menu>`
  resources. `Root().Menus["PresetPopup"]` etc. are the real Menu objects.
- `Menu:CommandCall(placeholderUIObject, false)` renders MA's real menu into a
  plugin-owned overlay (proven). But the popup shell (`ui/input/popup.uixml`,
  `<Popup OnLoad=":OnLoaded">`) has **no Context wiring**, so that route needs
  the invoker to bind `Context`; `Context`/`Value` are **string** properties set
  via `Obj.Set(handle,"Context",string)` — not object assignment.
- For "pick a value, get it back," the `PopupInput` path above is the clean win
  and uses MA's own native picker engine.

## Packaging note

UserPlugin XML that imports cleanly: no `Path` attribute; `<ComponentLua>` needs
`FileName` **and** `FilePath` (absolute dir). MA assigns Guids on add.
