# UnhookMultiple() [AI]
Removes every hook that matches a filter of function, target object and context object. `[P]`

---

## UnhookMultiple(function, handle, handle)

### "[V2.2][Manual] Definition"
```lua
UnhookMultiple(function, handle, handle)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| function | Function or nil | The triggered function to match. `[P]` |
| handle | Handle or nil | Target object. `[P]` |
| handle | Handle or nil | Context object. `[P]` |

### Returns
An integer: how many hooks were removed. `[P]`

### Example `[P]`
```lua
local removed = UnhookMultiple(MyCallback, nil, nil)
Printf("Removed " .. removed .. " hooks")
```
- Use nil for a filter you do not care about. `[P]`
- DumpAllHooks helps find the target and context names. `[P]`

---

## See Also
[Unhook](Unhook) · [HookObjectChange](HookObjectChange) · [DumpAllHooks](DumpAllHooks)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_unhookmultiple.html
