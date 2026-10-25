# CmdIndirect() [AI]
Queues a command line command to run in the Main task without blocking the script. `[P]`

---

## CmdIndirect(string[, handle[, handle]])

### "[V2.2][Manual] Definition"
```lua
CmdIndirect(string[, handle[, handle]])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | The command text; no "Please" and no Enter. |
| handle | handle | Optional. Undo list from CreateUndo. |
| handle | handle | Optional. Target of the command, e.g. a screen. |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
Printf("before")
CmdIndirect('Menu "Patch"')
Printf("after - printed without waiting")
```
- Asynchronous: the script carries on while the command runs in the Main task `[P]`.

---

## See Also
[Cmd](Cmd) · [CmdIndirectWait](CmdIndirectWait)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_cmdindirect.html
