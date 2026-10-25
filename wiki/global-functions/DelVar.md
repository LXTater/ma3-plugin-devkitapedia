# DelVar() [AI]
Removes a named variable from a variable set. `[P]`

---

## DelVar(handle, string)

### "[V2.2][Manual] Definition"
```lua
DelVar(handle, string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | The variable set holding the variable. |
| string | string | Name of the variable to delete. |

### Returns
true if deleted; false if not deleted, including when it does not exist. `[P]`

### Example `[P]`
```lua
local removed = DelVar(UserVars(), "myUserVar")
Printf(removed and "Deleted" or "Not deleted")
```
- A missing variable also gives false, so the result cannot distinguish the two failure cases `[P]`.

---

## See Also
[AddonVars](AddonVars) · [CurrentUser](CurrentUser)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_delvar.html
