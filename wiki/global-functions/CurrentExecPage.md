# CurrentExecPage() [AI]
Returns a handle to the executor page selected by the current user. `[P]`

---

## CurrentExecPage()

### "[V2.2][Manual] Definition"
```lua
CurrentExecPage()
```

### Returns
A handle to the executor page. `[P]`

### Example `[P]`
```lua
local page = CurrentExecPage()
Printf("---- page ----")
page:Dump()
Printf("---- end ----")
```
- The manual description names the wrong function (copy error) `[?]`.

---

## See Also
[CurrentUser](CurrentUser) · [DataPool](DataPool)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_currentexecpage.html
