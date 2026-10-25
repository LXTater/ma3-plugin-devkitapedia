# GetRTChannels() [AI]
Lists the RT channels of a (sub)fixture, as indexes or as object handles. `[P]`

---

## GetRTChannels(integer[, boolean]) / GetRTChannels(handle[, boolean])

### "[V2.2][Manual] Definition"
```lua
GetRTChannels(integer[, boolean])
GetRTChannels(handle[, boolean])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer or handle | integer / handle | Index of the (sub)fixture, or a handle to it `[P]` |
| boolean | boolean (optional, default false) | `true` returns handles, `false` returns integer indexes `[P]` |

### Returns
A table of RT channel indexes or handles. `[P]`

### Example `[P]`
```lua
return function()
    local fix = SelectionFirst()
    if not fix then Printf("Select a fixture") return end
    for i, h in ipairs(GetRTChannels(fix, true)) do
        Printf("%d: %s", i, tostring(h.rt_index))
    end
    Printf("index form count: %d", #GetRTChannels(fix))
end
```
- The manual gives one example per argument form. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetRTChannel](GetRTChannel) · [GetRTChannelCount](GetRTChannelCount) · [SelectionFirst](SelectionFirst)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getrtchannels.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getrtchannels.html
