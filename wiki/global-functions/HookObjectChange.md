# HookObjectChange() [AI]
Registers a callback that runs whenever the watched object changes. `[P]`

---

## HookObjectChange(function, handle, handle[, handle])

### "[V2.2][Manual] Definition"
```lua
HookObjectChange(function, handle, handle[, handle])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| function | function name | Callback invoked on each change `[P]` |
| handle | handle | Object to watch; passed to the callback first `[P]` |
| handle | handle | Handle of the plugin creating the hook `[P]` |
| handle | handle | Optional object passed to the callback as third argument `[P]` |

### Returns
An integer hook id; keep it to unhook later. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local function OnChange(obj)
  Printf("changed: " .. tostring(obj.name))
end
local id = HookObjectChange(OnChange, Root(), my_plugin_handle)
```
- Store the returned id so the hook can be removed. `[P]`

---

## See Also
[IsObjectValid](IsObjectValid)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_hookobjectchange.html
