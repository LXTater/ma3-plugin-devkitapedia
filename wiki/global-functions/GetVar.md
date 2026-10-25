# GetVar() [AI]
Reads a named variable from a variable set. `[P]`

---

## GetVar(handle, string)

### "[V2.2][Manual] Definition"
```lua
GetVar(handle, string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | Handle of the variable set `[P]` |
| string | string | Variable name `[P]` |

### Returns
The variable's value, or nil if it does not exist. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local v = GetVar(UserVars(), "scene")
Printf("scene = " .. tostring(v))
```
- Pair with GlobalVars() for global variables. `[P]`

---

## See Also
[GlobalVars](GlobalVars)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getvar.html
