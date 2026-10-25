# GetApiDescriptor() [AI]
Returns descriptions of every object-free Lua function as a table. `[P]`

---

## GetApiDescriptor()

### "[V2.2][Manual] Definition"
```lua
GetApiDescriptor()
```

### Returns
A table of entries; each entry holds three strings: function name, argument description, return description. Order is not guaranteed. `[P]`

### Example `[P]`
```lua
return function()
    for _, d in ipairs(GetApiDescriptor()) do
        Printf("%s | args: %s | returns: %s", d[1], d[2], d[3])
    end
end
```
- Descriptions only; the functions themselves are not included. `[P]`
- Output is unsorted, so sort it yourself if you need order. `[P]`

---

## See Also
[GetObjApiDescriptor](GetObjApiDescriptor) · [Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getapidescriptor.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getapidescriptor.html
