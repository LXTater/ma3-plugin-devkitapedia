# IntToHandle() [AI]
Converts an integer back into the object handle it came from. `[P]`

---

## IntToHandle(integer)

### "[V2.2][Manual] Definition"
```lua
IntToHandle(integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | Number matching an existing handle `[P]` |

### Returns
The handle of the matching object. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local n = HandleToInt(Root())
local h = IntToHandle(n)
Printf("valid: " .. tostring(IsObjectValid(h)))
```
- The integer must match an existing handle. `[P]`

---

## See Also
[HandleToInt](HandleToInt) · [HandleToStr](HandleToStr) · [IsObjectValid](IsObjectValid)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_inttohandle.html
