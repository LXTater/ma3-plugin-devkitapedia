# GlobalVars() [AI]
Returns a handle to the global variable set. `[P]`

---

## GlobalVars()

### "[V2.2][Manual] Definition"
```lua
GlobalVars()
```

### Returns
A handle to the global variable set. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local gv = GlobalVars()
SetVar(gv, "counter", 1)
Printf("counter = " .. tostring(GetVar(gv, "counter")))
DelVar(gv, "counter")
```
- Use with GetVar and the related set/delete variable functions. `[P]`

---

## See Also
[GetVar](GetVar)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_globalvars.html
