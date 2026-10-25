# Cmd() [AI]
Runs a command on the grandMA3 command line and waits for it to finish. `[P]`

---

## Cmd(string[, handle])

### "[V2.2][Manual] Definition"
```lua
Cmd(string[, handle])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | The command text; no "Please" and no Enter. |
| handle | handle | Optional. Undo list from CreateUndo. |
| ... | any | Optional extra arguments for the command. |

### Returns
A feedback string: "OK", "Syntax Error" or "Illegal Command". It can be ignored. `[P]`

### Example `[P]`
```lua
local result = Cmd("ClearAll")
Printf("Cmd said: " .. tostring(result))
```
- Runs in the Lua task, synchronously, and blocks that task; a bad command can stall the system `[P]`.
- For non-blocking execution see CmdIndirect `[P]`.

---

## In the Wild: Importing frames and storing a macro `[onPC]`
```lua
Cmd(string.format('Import Scribble %d "%s.xml" /Path "%s" /NC', slot, name, folder))
Cmd('Store Macro ' .. MACRO .. ' /NC')
```
`/NC` suppresses the confirmation popup, which a plugin cannot answer. `[P]`

*Excerpt from the Steamboat Willie Player plugin, CC BY 4.0, Badass Lighting Tools. [Source](https://github.com/badasslighting/R-D-Lab/tree/main/MA3-Scribble-Animator/releases/steamboat-willie).*

See [Steamboat Willie Player](Steamboat-Willie-Player).

---

## See Also
[CmdIndirect](CmdIndirect) · [CmdIndirectWait](CmdIndirectWait) · [CreateUndo](CreateUndo)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_cmd.html
