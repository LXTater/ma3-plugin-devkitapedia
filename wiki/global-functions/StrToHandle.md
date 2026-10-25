# StrToHandle() [AI]
Converts a hexadecimal handle string back into a handle. `[P]`

---

## StrToHandle(string)

### "[V2.2][Manual] Definition"
```lua
StrToHandle(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | String | Hexadecimal handle number; it must correspond to a real handle. `[P]` |

### Returns
The matching handle. `[P]`

### Example `[P]`
```lua
local seq = SelectedSequence()
local hex = HandleToStr(seq)
local again = StrToHandle(hex)
Printf("Back again: " .. again.name)
```
- The string must match an actual handle. `[P]`

---

## See Also
[HandleToStr](HandleToStr) · [SelectedSequence](SelectedSequence) · [ToAddr](ToAddr)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_strtohandle.html
