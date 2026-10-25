# CreateUndo() [AI]
Creates a labelled undo list so several actions can be undone as one. `[P]`

---

## CreateUndo(string)

### "[V2.2][Manual] Definition"
```lua
CreateUndo(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Label for the undo list. |

### Returns
A handle to the undo list. `[P]`

### Example `[P]`
```lua
local undo = CreateUndo("Batch edit")
Cmd('Label Group 1 "Front"', undo)
Cmd('Label Group 2 "Back"', undo)
CloseUndo(undo)
```
- Always close the list with CloseUndo `[P]`.

---

## See Also
[CloseUndo](CloseUndo) · [Cmd](Cmd)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_createundo.html
