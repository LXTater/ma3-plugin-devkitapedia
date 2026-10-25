# CheckFIDCollision() [AI]
Checks whether an ID, or a run of consecutive IDs, is unused for a given ID type. `[P]`

---

## CheckFIDCollision(integer[, integer[, integer]])

### "[V2.2][Manual] Definition"
```lua
CheckFIDCollision(integer[, integer[, integer]])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | First ID to test. |
| count | integer | Optional, default 1. How many consecutive IDs to test. |
| IDType | integer | Optional, default 0 (Fixture). Other values cover Channel, Universal, Marker, Multipatch. |

### Returns
true if the whole range is available, false if any ID is already used. `[P]`

### Example `[P]`
```lua
local first, count = 500, 10
if CheckFIDCollision(first, count) then
  Printf("FIDs 500-509 are free")
else
  Printf("Some of FIDs 500-509 are in use")
end
```
- Omit the third argument to check Fixture IDs `[P]`.

---

## See Also
[CheckDMXCollision](CheckDMXCollision) · [AddFixtures](AddFixtures)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_checkfidcollision.html
