# GetPresetData() [AI]
Returns the contents of a preset as a nested Lua table. `[P]`

---

## GetPresetData(handle[, boolean[, boolean]])

### "[V2.2][Manual] Definition"
```lua
GetPresetData(handle[, boolean[, boolean]])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | Preset to read `[P]` |
| phaser only | boolean (optional, default false) | `true` returns only phaser data `[P]` |
| by fixtures | boolean (optional, default true) | `true` adds a `by_fixtures` table keyed by fixture ID instead of UI channel index `[P]` |

### Returns
A multi-level table, or `nil`. `[P]`

### Example `[P]`
```lua
return function()
    local preset = DataPool().Presets:Children()[1]
    local data = preset and GetPresetData(preset)
    if not data then Printf("No preset data") return end
    for k, v in pairs(data) do Printf("%s : %s", tostring(k), type(v)) end
end
```
- Always handle a `nil` return. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[DataPool](DataPool) · [Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpresetdata.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpresetdata.html
