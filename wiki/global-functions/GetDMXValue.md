# GetDMXValue() [AI]
Reads the value at one DMX address. `[P]`

---

## GetDMXValue(integer[, integer, boolean])

### "[V2.2][Manual] Definition"
```lua
GetDMXValue(integer[, integer, boolean])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| address | integer | 1-512 when a universe is given; otherwise absolute 1 to 524288 `[P]` |
| universe | integer (optional) | Universe number `[P]` |
| percent | boolean (optional) | `true` returns 0-100, `false` returns 0-255 `[P]` |

### Returns
A number for the address value, or `nil` if the address is not granted. `[P]`

### Example `[P]`
```lua
return function()
    local v = GetDMXValue(10, 1, true)
    if v then Printf("U1.10 = %s%%", v) else Printf("Not granted") end
end
```
- Check for `nil` before using the value. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetDMXUniverse](GetDMXUniverse) · [Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getdmxvalue.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getdmxvalue.html
