# SetVar() [AI]
Writes a value to a named variable in a variable set, creating it if needed and overwriting it otherwise. `[P]`

---

## SetVar(handle, string, value)

### "[V2.2][Manual] Definition"
```lua
SetVar(handle, string, value)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | Handle | The variable set, e.g. from UserVars(). `[P]` |
| string | String | Variable name. `[P]` |
| value | String, integer or double | The value to store. `[P]` |

### Returns
A boolean: true if the variable was set, false if not. `[P]`

### Example `[P]`
```lua
local ok = SetVar(UserVars(), "greeting", "hello")
Printf(ok and "stored" or "not stored")
```
- Existing variables of the same name are overwritten. `[P]`

---

## See Also
[UserVars](UserVars) · [GetVar](GetVar) · [DelVar](DelVar)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_setvar.html
