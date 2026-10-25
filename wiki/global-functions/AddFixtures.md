# AddFixtures() [AI]
Adds one or more fixtures to the patch, driven by a table of settings. `[P]`

---

## AddFixtures(table)

### "[V2.2][Manual] Definition"
```lua
AddFixtures(table)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| mode | handle | Required. The DMX mode (fixture type and mode) to patch. |
| amount | integer | Required. How many fixtures to add. |
| name | string | Optional. Name for the first fixture. |
| fid | string | Optional. Fixture ID. |
| cid | string | Optional. Channel ID; only valid when idtype is not "Fixture". |
| idtype | string | Optional. ID type name, needed only if not "Fixture". |
| patch | table | Optional. Up to eight "universe.address" strings, one per DMX break. |
| layer | string | Optional. Layer name. |
| class | string | Optional. Class name. |
| parent | handle | Optional. Parent fixture, to add a sub-fixture. |
| insert_index | integer | Optional. Insert position. |
| undo | string | Optional. Undo label. |

### Returns
true on success, nil on failure. `[P]`

### Example `[P]`
```lua
-- patch two fixtures of an existing DMX mode
local mode = Root().ShowData.DMXProfiles[1][1]  -- assumed to exist
local ok = AddFixtures({
  mode = mode,
  amount = 2,
  name = "Wash",
  fid = "301",
  patch = { "1.101" },
  undo = "Add washes"
})
Printf(ok and "Added" or "AddFixtures failed")
```
- The command line destination must already point at the patch location when this runs `[P]`.
- Free FIDs and DMX addresses are not checked for you; see the collision-check functions `[P]`.

---

## See Also
[CheckDMXCollision](CheckDMXCollision) · [CheckFIDCollision](CheckFIDCollision) · [CreateMultiPatch](CreateMultiPatch)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_addfixtures.html
