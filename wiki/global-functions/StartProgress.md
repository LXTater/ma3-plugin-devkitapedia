# StartProgress() [AI]
Creates a titled progress bar that appears on all screens and stays until you stop it. `[P]`

---

## StartProgress(string)

### "[V2.2][Manual] Definition"
```lua
StartProgress(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | String | Title shown on the bar. `[P]` |

### Returns
A handle to the progress bar; keep it for later calls. `[P]`

### Example `[P]`
```lua
local bar = StartProgress("Processing")
-- store `bar` somewhere you can reach later, then:
-- StopProgress(bar)
```
- The bar stays visible until StopProgress is called with the returned handle. `[P]`
- The manual warns that repeatedly running the call without keeping the handle leaves bars that cannot be removed. `[P]`

---

## See Also
[StopProgress](StopProgress) · [SetProgress](SetProgress) · [SetProgressRange](SetProgressRange) · [SetProgressText](SetProgressText)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_startprogress.html
