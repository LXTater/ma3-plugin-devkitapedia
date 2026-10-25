# CmdIndirectWait() [AI]
Runs a command line command in the Main task; the script is not blocked but later commands queue behind it. `[P]`

---

## CmdIndirectWait(string[, handle[, handle]])

### "[V2.2][Manual] Definition"
```lua
CmdIndirectWait(string[, handle[, handle]])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | The command text; no execute keyword. |
| handle | handle | Optional. Undo list from CreateUndo. |
| handle | handle | Optional. Target of the command, e.g. a screen. |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
Printf("step 1")
CmdIndirectWait('Menu "Patch"')
Printf("step 2 - ordered after the command")
```
- Unlike CmdIndirect, execution is synchronous in the Main task so ordering is preserved `[P]`.

---

## See Also
[Cmd](Cmd) · [CmdIndirect](CmdIndirect)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_cmdindirectwait.html
