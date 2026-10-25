# HandleToInt() [AI]
Turns an object handle into an integer. `[P]`

---

## HandleToInt(handle)

### "[V2.2][Manual] Definition"
```lua
HandleToInt(handle)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | Handle to convert `[P]` |

### Returns
The integer form of the handle. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local n = HandleToInt(Root())
Printf("root as int: " .. n)
local back = IntToHandle(n)
Printf("round trip valid: " .. tostring(IsObjectValid(back)))
```
- The integer can be turned back with IntToHandle. `[P]`

---

## See Also
[IntToHandle](IntToHandle) · [HandleToStr](HandleToStr)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_handletoint.html
