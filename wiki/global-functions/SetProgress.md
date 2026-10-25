# SetProgress() [AI]
Sets the current value of an existing progress bar. `[P]`

---

## SetProgress(handle, integer)

### "[V2.2][Manual] Definition"
```lua
SetProgress(handle, integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | Handle | The progress bar, as returned by StartProgress. `[P]` |
| integer | Integer | The new current value. `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
local bar = StartProgress("Work")
SetProgress(bar, 5)
```
- The bar must already exist. `[P]`

---

## See Also
[StartProgress](StartProgress) · [StopProgress](StopProgress) · [SetProgressRange](SetProgressRange) · [SetProgressText](SetProgressText)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_setprogress.html
