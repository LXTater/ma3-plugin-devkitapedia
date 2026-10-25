# GetUIObjectAtPosition() [AI]
Finds the UI object under a pixel coordinate on a display. `[P]`

---

## GetUIObjectAtPosition(integer, table)

### "[V2.2][Manual] Definition"
```lua
GetUIObjectAtPosition(integer, table)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | Display index `[P]` |
| table | table | Position with numeric `x` and `y` fields in pixels from the left/top `[P]` |

### Returns
A handle to the object, or nil if nothing is there. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local obj = GetUIObjectAtPosition(1, {x = 400, y = 300})
if obj then
  obj:Dump()
else
  Printf("Nothing at that point")
end
```
- Coordinates are pixels from the display's top-left corner. `[P]`

---

## See Also
[GetTopOverlay](GetTopOverlay) · [GetTopModal](GetTopModal)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getuiobjectatposition.html
