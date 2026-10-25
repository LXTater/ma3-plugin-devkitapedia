# GetDMXUniverse() [AI]
Returns the current values of a whole DMX universe as a table. `[P]`

---

## GetDMXUniverse(integer[, boolean])

### "[V2.2][Manual] Definition"
```lua
GetDMXUniverse(integer[, boolean])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | Universe number, 1 to 1024 `[P]` |
| boolean | boolean (optional) | `true` for percent (0-100), `false` for DMX (0-255) `[P]` |

### Returns
A table of address/value pairs, or `nil` if the universe is not granted or out of range. `[P]`

### Example `[P]`
```lua
return function()
    local u = GetDMXUniverse(1, false)
    if not u then Printf("Universe 1 unavailable") return end
    for addr, val in pairs(u) do
        if val > 0 then Printf("ch %s = %s", addr, val) end
    end
end
```
- Always handle the `nil` case. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetDMXValue](GetDMXValue) · [Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getdmxuniverse.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getdmxuniverse.html
