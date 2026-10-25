# Selection() [AI]
Gives you a handle to the object that holds the current fixture selection. `[P]`

---

## Selection()

### "[V2.2][Manual] Definition"
```lua
Selection()
```

### Returns
A handle to the Selection object. `[P]`

### Example `[P]`
```lua
local obj = Selection()
if obj then
  Printf("--- Selection ---")
  obj:Dump()
else
  Printf("Selection: nothing returned")
end
```
- Takes no arguments. `[P]`
- For simple counts or iteration, SelectionCount, SelectionFirst and SelectionNext are lighter. `[P]`

---

## See Also
[SelectionCount](SelectionCount) · [SelectionFirst](SelectionFirst) · [SelectionNext](SelectionNext)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_selection.html
