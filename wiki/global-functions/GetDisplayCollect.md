# GetDisplayCollect() [AI]
Returns a handle to the DisplayCollect object, the container of all displays. `[P]`

---

## GetDisplayCollect()

### "[V2.2][Manual] Definition"
```lua
GetDisplayCollect()
```

### Returns
A handle to the DisplayCollect. `[P]`

### Example `[P]`
```lua
return function()
    local dc = GetDisplayCollect()
    Printf("children: %d", dc:Count())
    Dump(dc)
end
```
- Takes no arguments. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetDisplayByIndex](GetDisplayByIndex) · [GetFocusDisplay](GetFocusDisplay)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getdisplaycollect.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getdisplaycollect.html
