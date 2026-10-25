# SetProgressText() [AI]
Sets a changeable text label shown beside the title of an existing progress bar. `[P]`

---

## SetProgressText(handle, string)

### "[V2.2][Manual] Definition"
```lua
SetProgressText(handle, string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | Handle | The progress bar. `[P]` |
| string | String | The label text to display. `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
local bar = StartProgress("Export")
SetProgressText(bar, "Step 2 of 4")
```
- The title is fixed when the bar is created; this label can change as work proceeds. `[P]`

---

## See Also
[StartProgress](StartProgress) · [SetProgress](SetProgress) · [StopProgress](StopProgress)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_setprogresstext.html
