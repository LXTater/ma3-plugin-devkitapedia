# CurrentScreenConfig() [AI]
Returns a handle to the current user's screen configuration. `[P]`

---

## CurrentScreenConfig()

### "[V2.2][Manual] Definition"
```lua
CurrentScreenConfig()
```

### Returns
A handle to the screen configuration. `[P]`

### Example `[P]`
```lua
local cfg = CurrentScreenConfig()
Printf("---- screens ----")
cfg:Dump()
Printf("---- end ----")
```
- Dump() lists its properties and children `[P]`.

---

## See Also
[DefaultDisplayPositions](DefaultDisplayPositions) · [CurrentProfile](CurrentProfile)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_currentscreenconfig.html
