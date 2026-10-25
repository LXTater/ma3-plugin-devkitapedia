# CloseUndo() [AI]
Closes an undo list that was opened with CreateUndo. `[P]`

---

## CloseUndo(handle)

### "[V2.2][Manual] Definition"
```lua
CloseUndo(handle)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | The undo list handle from CreateUndo. |

### Returns
true if the list was closed, false if it is still in use. `[P]`

### Example `[P]`
```lua
local undo = CreateUndo("Two labels")
Cmd('Label Group 1 "A"', undo)
Cmd('Label Group 2 "B"', undo)
local closed = CloseUndo(undo)
Printf(closed and "Grouped as one undo step" or "Undo list still busy")
```
- Commands run with the handle are undone together in one step `[P]`.

---

## See Also
[CreateUndo](CreateUndo) · [Cmd](Cmd)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_closeundo.html
