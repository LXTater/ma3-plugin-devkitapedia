# CheckDMXCollision() [AI]
Tests whether a DMX address range is free, sized from the channel count of a given DMX mode. `[P]`

---

## CheckDMXCollision(handle, string[, integer[, integer]])

### "[V2.2][Manual] Definition"
```lua
CheckDMXCollision(handle, string[, integer[, integer]])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | DMX mode whose channel count sets the range size. |
| string | string | Start address, e.g. "1.1". |
| count | integer | Optional, default 1. Extra consecutive modes to include. |
| break_index | integer | Optional, default 0. Which DMX break to use. |

### Returns
true if the start address is usable for the computed channel count, false otherwise. `[P]`

### Example `[P]`
```lua
-- is universe 2 address 50 free for the first selected fixture's mode?
local fix = SelectionFirst()
if fix == nil then
  Printf("Select a fixture first")
  return
end
local free = CheckDMXCollision(fix.DMXMode, "2.50", 1)
Printf(free and "Address free" or "Address taken")
```
- That the selected fixture exposes its DMX mode as shown above is an assumption `[?]`.

---

## See Also
[CheckFIDCollision](CheckFIDCollision) · [AddFixtures](AddFixtures)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_checkdmxcollision.html
