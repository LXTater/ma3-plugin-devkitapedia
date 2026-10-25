# GetUIChannelIndex() [AI]
Finds the UI channel index for a given fixture and attribute. `[P]`

---

## GetUIChannelIndex(integer, integer)

### "[V2.2][Manual] Definition"
```lua
GetUIChannelIndex(integer, integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | Patch index of the fixture `[P]` |
| integer | integer | 0-based attribute index (see attribute definitions) `[P]` |

### Returns
An integer UI channel index, usable with channel functions. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local idx = GetUIChannelIndex(1, 0)
if idx then
  Printf("UI channel index: " .. idx)
else
  Printf("No such channel")
end
```
- Can return nil; check before use. `[P]`

---

## See Also
[GetUIChannels](GetUIChannels) · [GetUIChannelCount](GetUIChannelCount) · [GetSubfixture](GetSubfixture)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getuichannelindex.html
