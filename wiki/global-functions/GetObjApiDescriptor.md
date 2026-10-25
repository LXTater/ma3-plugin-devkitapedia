# GetObjApiDescriptor() [AI]
Returns descriptions of all object-based Lua functions as a table. `[P]`

---

## GetObjApiDescriptor()

### "[V2.2][Manual] Definition"
```lua
GetObjApiDescriptor()
```

### Returns
A table whose entries each hold three strings: function name, argument description, return description. It is unsorted. `[P]`

### Example `[P]`
```lua
return function()
    local n = 0
    for _, d in ipairs(GetObjApiDescriptor()) do
        n = n + 1
        Printf("%s -> %s", d[1], d[3])
    end
    Printf("%d object functions described", n)
end
```
- Descriptions only, not callable functions. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetApiDescriptor](GetApiDescriptor) · [Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getobjapidescriptor.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getobjapidescriptor.html
