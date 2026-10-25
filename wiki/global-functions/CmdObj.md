# CmdObj() [AI]
Returns a handle to the command line object so its state can be inspected. `[P]`

---

## CmdObj()

### "[V2.2][Manual] Definition"
```lua
CmdObj()
```

### Returns
A handle to the command line object. `[P]`

### Example `[P]`
```lua
local cmd = CmdObj()
cmd:Dump()
Printf("Current text: " .. tostring(cmd.Cmd))
```
- The manual lists properties such as command text, destination, user, profile and selected object; exact property names are not verified here `[?]`.

---

## See Also
[Cmd](Cmd) · [CurrentUser](CurrentUser)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_cmdobj.html
