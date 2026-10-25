# IncProgress() [AI]
Moves a progress bar's value by an amount; negative values go backward. `[P]`

---

## IncProgress(handle, integer)

### "[V2.2][Manual] Definition"
```lua
IncProgress(handle, integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | Progress bar created with StartProgress `[P]` |
| integer | integer | Amount to add (negative to subtract) `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
-- bar was created earlier with StartProgress
IncProgress(bar, 5)
IncProgress(bar, -2)
```
- The bar must already exist. `[P]`

---

## See Also
[Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_incprogress.html
