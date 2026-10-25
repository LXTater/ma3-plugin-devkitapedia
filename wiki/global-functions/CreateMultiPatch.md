# CreateMultiPatch() [AI]
Creates multi-patch fixtures that follow the fixtures in a table. `[P]`

---

## CreateMultiPatch({handles}, integer[, string])

### "[V2.2][Manual] Definition"
```lua
CreateMultiPatch({handles}, integer[, string])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handles | table | Fixture handles that receive the multi-patch fixtures. |
| integer | integer | How many multi-patch fixtures to create. |
| string | string | Optional. Undo text. |

### Returns
The number created, or nil on failure. `[P]`

### Example `[P]`
```lua
local fixtures = { Patch().Fixtures[1] }  -- assumed to exist
local made = CreateMultiPatch(fixtures, 3, "Add multis")
if made then Printf("Created " .. made) else ErrPrintf("multi patch failed") end
```
- The command line may need to be at the right destination beforehand `[?]`.

---

## See Also
[AddFixtures](AddFixtures) · [CheckDMXCollision](CheckDMXCollision)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_createmultipatch.html
