# CurrentUser() [AI]
Returns a handle to the user that is currently logged in on this station. `[P]`

---

## CurrentUser()

### "[V2.2][Manual] Definition"
```lua
CurrentUser()
```

### Returns
A handle to the user. `[P]`

### Example `[P]`
```lua
local user = CurrentUser()
Printf("---- user ----")
user:Dump()
Printf("---- end ----")
```
- The manual page has no explicit signature line; the call form is inferred `[?]`.

---

## See Also
[CurrentProfile](CurrentProfile) · [CurrentEnvironment](CurrentEnvironment)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_currentuser.html
