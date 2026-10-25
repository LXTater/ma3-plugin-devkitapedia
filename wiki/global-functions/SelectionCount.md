# SelectionCount() [AI]
Tells you how many fixtures are in the current selection. `[P]`

---

## SelectionCount()

### "[V2.2][Manual] Definition"
```lua
SelectionCount()
```

### Returns
An integer: the number of selected fixtures (0 when nothing is selected). `[P]`

### Example `[P]`
```lua
local n = SelectionCount()
Printf("Fixtures selected: " .. n)
```
- Takes no arguments. `[P]`

---

## See Also
[Selection](Selection) · [SelectionFirst](SelectionFirst) · [SelectionNext](SelectionNext)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_selectioncount.html
