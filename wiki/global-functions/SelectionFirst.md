# SelectionFirst() [AI]
Returns the patch index of the first fixture in the selection, plus its position in the selection grid. `[P]`

---

## SelectionFirst()

### "[V2.2][Manual] Definition"
```lua
SelectionFirst()
```

### Returns
Four integers in order: patch index, grid X, grid Y, grid Z (all 0-based). `[P]`

### Example `[P]`
```lua
local idx, gx, gy, gz = SelectionFirst()
if idx == nil then
  Printf("Nothing selected")
  return
end
Printf("First: patch index %d at grid %d/%d/%d", idx, gx, gy, gz)
```
- The first value is a patch index, not an FID or CID. `[P]`
- You may ignore return values you do not need. `[P]`
- Behaviour with an empty selection is not stated, so the nil check is a precaution `[?]`.

---

## See Also
[SelectionNext](SelectionNext) · [SelectionCount](SelectionCount) · [GetSubfixture](GetSubfixture)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_selectionfirst.html
