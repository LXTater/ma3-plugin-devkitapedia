# GetDisplayByIndex() [AI]
Returns the display object that sits at a given index. `[P]`

---

## GetDisplayByIndex(integer)

### "[V2.2][Manual] Definition"
```lua
GetDisplayByIndex(integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | Index of the display `[P]` |

### Returns
A handle to the display. `[P]`

### Example `[P]`
```lua
return function()
    local d = GetDisplayByIndex(1)
    if d then Dump(d) else Printf("No display at index 1") end
end
```
- The manual's own example finds the index of a named display through the DisplayCollect first. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetDisplayCollect](GetDisplayCollect) · [GetFocusDisplay](GetFocusDisplay)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getdisplaybyindex.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getdisplaybyindex.html
