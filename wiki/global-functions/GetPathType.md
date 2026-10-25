# GetPathType() [AI]
Returns the name of the path type that belongs to an object, which helps when importing objects. `[P]`

---

## GetPathType(handle[, integer])

### "[V2.2][Manual] Definition"
```lua
GetPathType(handle[, integer])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | Object whose path type you want `[P]` |
| integer | integer (optional) | `0` system path type, `1` user path type; `Enums.PathContentType` may be used `[P]` |

### Returns
A string with the path type name. `[P]`

### Example `[P]`
```lua
return function()
    local m = DataPool().Macros:Children()[1]
    if not m then Printf("No macro found") return end
    Printf("system: " .. tostring(GetPathType(m, 0)))
    Printf("user: " .. tostring(GetPathType(m, 1)))
end
```
- The handle should be of the object type you are importing. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetPath](GetPath) · [GetPathOverrideFor](GetPathOverrideFor) · [DataPool](DataPool)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpathtype.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpathtype.html
