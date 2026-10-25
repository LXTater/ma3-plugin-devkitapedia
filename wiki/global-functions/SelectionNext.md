# SelectionNext() [AI]
Moves on to the next fixture in the selection, given an index that is already part of it. `[P]`

---

## SelectionNext(integer)

### "[V2.2][Manual] Definition"
```lua
SelectionNext(integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | Integer | Index of a fixture in the current selection; the next one after it is returned. `[P]` |

### Returns
Four integers in order: patch index, grid X, grid Y, grid Z (all 0-based). `[P]`

### Example `[P]`
```lua
local idx, gx, gy, gz = SelectionFirst()
while idx do
  Printf("Fixture %d at grid %d/%d/%d", idx, gx, gy, gz)
  idx, gx, gy, gz = SelectionNext(idx)
end
```
- Start the walk with SelectionFirst, then feed each returned index back in. `[P]`
- The manual's description of the first return value reads as if it were the first fixture, which seems inconsistent with the function's purpose `[?]`.
- The loop ends once no further fixture is returned. `[P]`

---

## See Also
[SelectionFirst](SelectionFirst) · [SelectionCount](SelectionCount) · [GetSubfixture](GetSubfixture)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_selectionnext.html
