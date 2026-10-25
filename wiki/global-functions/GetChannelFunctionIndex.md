# GetChannelFunctionIndex() [AI]
Returns the integer index of a channel function for a UI channel and attribute pair. `[P]`

---

## GetChannelFunctionIndex(uiChannelIndex, attributeIndex)

### "[V2.2][Manual] Definition"
```lua
GetChannelFunctionIndex(uiChannelIndex, attributeIndex)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| uiChannelIndex | integer | From the Parameter List or GetUIChannelIndex() `[P]` |
| attributeIndex | integer | 0-based; from Attribute Definitions or GetAttributeIndex() `[P]` |

### Returns
An integer channel function index. `[P]`

### Example `[P]`
```lua
return function()
    local fix = SelectionFirst()
    local attr = GetAttributeIndex("Dimmer")
    local ui = fix and GetUIChannelIndex(fix.FID, attr)
    if not (attr and ui) then Printf("Lookup failed") return end
    Printf("Channel function index: %d", GetChannelFunctionIndex(ui, attr))
end
```
- The manual shows no formal signature line; the argument order comes from its example. `[?]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetChannelFunction](GetChannelFunction) · [GetAttributeIndex](GetAttributeIndex) · [GetUIChannelIndex](GetUIChannelIndex)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getchannelfunctionindex.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getchannelfunctionindex.html
