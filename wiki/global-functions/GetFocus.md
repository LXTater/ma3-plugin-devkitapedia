# GetFocus() [AI]
Returns the UI object that currently has focus. `[P]`

---

## GetFocus()

### "[V2.2][Manual] Definition"
```lua
GetFocus()
```

### Returns
A handle to the focused object. `[P]`

### Example `[P]`
```lua
return function()
    local f = GetFocus()
    if f then Printf("Focused: " .. f:ToAddr()) Dump(f) end
end
```
- Takes no arguments. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetFocusDisplay](GetFocusDisplay)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getfocus.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getfocus.html
