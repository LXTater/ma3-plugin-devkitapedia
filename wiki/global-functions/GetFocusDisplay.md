# GetFocusDisplay() [AI]
Returns the display that currently has focus. `[P]`

---

## GetFocusDisplay()

### "[V2.2][Manual] Definition"
```lua
GetFocusDisplay()
```

### Returns
A handle to the focused display. `[P]`

### Example `[P]`
```lua
return function()
    local d = GetFocusDisplay()
    if d then Printf("Focused display: " .. tostring(d.name)) Dump(d) end
end
```
- Takes no arguments. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetFocus](GetFocus) · [GetDisplayByIndex](GetDisplayByIndex) · [GetDisplayCollect](GetDisplayCollect)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getfocusdisplay.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getfocusdisplay.html
