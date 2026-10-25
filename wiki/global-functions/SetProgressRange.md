# SetProgressRange() [AI]
Defines the start and end values of an existing progress bar. `[P]`

---

## SetProgressRange(handle, integer, integer)

### "[V2.2][Manual] Definition"
```lua
SetProgressRange(handle, integer, integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | Handle | The progress bar. `[P]` |
| integer | Integer | Start of the range. `[P]` |
| integer | Integer | End of the range. `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
local bar = StartProgress("Import")
SetProgressRange(bar, 1, 10)
```
- The bar must already exist. `[P]`

---

## See Also
[StartProgress](StartProgress) · [SetProgress](SetProgress) · [StopProgress](StopProgress)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_setprogressrange.html
