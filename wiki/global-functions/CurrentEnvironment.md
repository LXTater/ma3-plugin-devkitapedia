# CurrentEnvironment() [AI]
Returns a handle to the environment the user has currently selected. `[P]`

---

## CurrentEnvironment()

### "[V2.2][Manual] Definition"
```lua
CurrentEnvironment()
```

### Returns
A handle to the environment. `[P]`

### Example `[P]`
```lua
local env = CurrentEnvironment()
Printf("---- env ----")
env:Dump()
Printf("---- end ----")
```
- Use Dump() on the handle to see its properties `[P]`.

---

## See Also
[CurrentUser](CurrentUser) · [CurrentProfile](CurrentProfile)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_currentenvironment.html
