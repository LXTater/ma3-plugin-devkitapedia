# GetAttributeByUIChannel() [AI]
Maps a UI channel index to the attribute handle behind it. `[P]`

---

## GetAttributeByUIChannel(integer)

### "[V2.2][Manual] Definition"
```lua
GetAttributeByUIChannel(integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | UI channel index (see the Parameter List) `[P]` |

### Returns
A handle to the attribute linked to that UI channel. `[P]`

### Example `[P]`
```lua
return function()
    local fix = SelectionFirst()
    if not fix then Printf("Select a fixture first") return end
    local ui = GetUIChannelIndex(fix.FID, 0)
    local attr = GetAttributeByUIChannel(ui)
    if attr then Printf("Attribute: " .. attr:AddrNative()) end
end
```
- Look up indexes in the Parameter List. `[P]`
- Since version 2.2 per the manual. `[P]`

---

## See Also
[GetUIChannelIndex](GetUIChannelIndex) · [SelectionFirst](SelectionFirst) · [GetAttributeIndex](GetAttributeIndex)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getattributebyuichannel.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getattributebyuichannel.html
