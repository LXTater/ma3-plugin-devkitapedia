# IsObjectValid() [AI]
Checks whether a value refers to a valid object. `[P]`

---

## IsObjectValid(handle)

### "[V2.2][Manual] Definition"
```lua
IsObjectValid(handle)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | Possible object handle `[P]` |

### Returns
true if valid, otherwise nil. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local h = Root()
if IsObjectValid(h) then
  Printf("root is valid")
end
```
- Returns nil, not false, when invalid. `[P]`

---

## See Also
[IntToHandle](IntToHandle) · [HandleToInt](HandleToInt)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_isobjectvalid.html
