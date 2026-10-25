# GetUIChannels() [AI]
Returns a table of UI channels for a fixture, as indexes or as object handles. `[P]`

---

## GetUIChannels(integer[, boolean] or handle[, boolean])

### "[V2.2][Manual] Definition"
```lua
GetUIChannels(integer[, boolean] or handle[, boolean])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer or handle | integer / handle | Fixture (subfixture) index or object handle `[P]` |
| boolean | boolean | Optional, default false. True returns handles instead of indexes `[P]` |

### Returns
A table of UI channel indexes or handles. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local list = GetUIChannels(1)
for _, idx in ipairs(list) do
  Printf("channel " .. idx)
end
local objs = GetUIChannels(1, true)
Printf("handles: " .. #objs)
```
- Handles let you read channel properties directly. `[P]`

---

## See Also
[GetUIChannelIndex](GetUIChannelIndex) · [GetUIChannelCount](GetUIChannelCount)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getuichannels.html
