# ToAddr() [AI]
Turns a handle into an address string usable in commands, optionally using names rather than numbers. `[P]`

---

## ToAddr(handle[, boolean])

### "[V2.1][Manual] Definition"
```lua
ToAddr(handle[, boolean])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | Handle | The object to address. `[P]` |
| boolean | Boolean (optional) | true to use names; default false gives numbers. `[P]` |

### Returns
A string with the address. `[P]`

### Example `[P]`
```lua
local seq = SelectedSequence()
Printf("Numbers: " .. ToAddr(seq))
Printf("Names:   " .. ToAddr(seq, true))
```
- This page is versioned 2.1 in the manual. `[P]`

---

## See Also
[HandleToStr](HandleToStr) · [StrToHandle](StrToHandle) · [SelectedSequence](SelectedSequence)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_toaddr.html
