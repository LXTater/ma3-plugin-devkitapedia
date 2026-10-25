# StopProgress() [AI]
Removes an existing progress bar. `[P]`

---

## StopProgress(handle)

### "[V2.2][Manual] Definition"
```lua
StopProgress(handle)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | Handle | The progress bar to remove, from StartProgress. `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
local function finish(bar)
  StopProgress(bar)
end
```
- The bar must already exist. `[P]`

---

## See Also
[StartProgress](StartProgress) · [SetProgress](SetProgress)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_stopprogress.html
