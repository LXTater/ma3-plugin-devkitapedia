# UserVars() [AI]
Gives you a handle to the set of user variables. `[P]`

---

## UserVars()

### "[V2.2][Manual] Definition"
```lua
UserVars()
```

### Returns
A handle to the user variable set. `[P]`

### Example `[P]`
```lua
local vars = UserVars()
SetVar(vars, "demo", 42)
Printf("demo = " .. tostring(GetVar(vars, "demo")))
DelVar(vars, "demo")
```
- Pair it with SetVar, GetVar and DelVar. `[P]`

---

## See Also
[SetVar](SetVar) · [GetVar](GetVar) · [DelVar](DelVar)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_uservars.html
