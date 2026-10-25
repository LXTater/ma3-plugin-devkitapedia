# GetSelectedAttribute() [AI]
Gets a handle to the attribute that is currently selected. `[P]`

---

## GetSelectedAttribute()

### "[V2.2][Manual] Definition"
```lua
GetSelectedAttribute()
```

### Returns
A handle to the selected attribute. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local attr = GetSelectedAttribute()
if attr then
  Printf("Selected attribute follows")
  attr:Dump()
end
```
- Takes no arguments. `[P]`

---

## See Also
[GetUIChannels](GetUIChannels)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getselectedattribute.html
