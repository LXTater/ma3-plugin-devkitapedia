# GetRTChannel() [AI]
Returns a table of details about a single RT channel. `[P]`

---

## GetRTChannel(integer)

### "[V2.2][Manual] Definition"
```lua
GetRTChannel(integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | RT channel index `[P]` |

### Returns
A table with keys: `fixture`, `subfixture`, `dmx_channel` (handles); `dmx_default`, `dmx_highlight`, `dmx_lowlight`, `ui_index_first`, `rt_index`, `freq` (integers); `info`, `patch` (tables). `[P]`

### Example `[P]`
```lua
return function()
    local fix = SelectionFirst()
    if not fix then Printf("Select a fixture") return end
    local idx = GetRTChannels(fix)[1]
    local rt = idx and GetRTChannel(idx)
    if not rt then Printf("No RT channel") return end
    for k, v in pairs(rt) do Printf("%s = %s", k, tostring(v)) end
end
```
- Check for `nil` when the fixture has no RT channels. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetRTChannels](GetRTChannels) · [GetRTChannelCount](GetRTChannelCount) · [SelectionFirst](SelectionFirst)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getrtchannel.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getrtchannel.html
