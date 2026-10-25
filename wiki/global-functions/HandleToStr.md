# HandleToStr() [AI]
Turns an object handle into a hexadecimal string. `[P]`

---

## HandleToStr(handle)

### "[V2.2][Manual] Definition"
```lua
HandleToStr(handle)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | Handle to convert `[P]` |

### Returns
A string holding the handle number in hexadecimal. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local s = HandleToStr(Root())
Printf("root handle: " .. s)
```
- The manual shows converting the result back to a handle for display `[?]`.

---

## See Also
[HandleToInt](HandleToInt) · [IntToHandle](IntToHandle)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_handletostring.html
