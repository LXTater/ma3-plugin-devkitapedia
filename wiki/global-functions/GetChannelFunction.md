# GetChannelFunction() [AI]
Returns the channel function handle for a UI channel and attribute pair. `[P]`

---

## GetChannelFunction(integer, integer)

### "[V2.2][Manual] Definition"
```lua
GetChannelFunction(integer, integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| UI channel index | integer | From the Parameter List or GetUIChannelIndex() `[P]` |
| attribute index | integer | 0-based; from Attribute Definitions or GetAttributeIndex() `[P]` |

### Returns
A handle to the channel function. `[P]`

### Example `[P]`
```lua
return function()
    local fix = SelectionFirst()
    if not fix then Printf("Nothing selected") return end
    local attr = GetAttributeIndex("Dimmer")
    local ui = GetUIChannelIndex(fix.FID, attr)
    if not (attr and ui) then Printf("No dimmer on this fixture") return end
    Dump(GetChannelFunction(ui, attr))
end
```
- Guard against empty selections and fixtures without the attribute. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetChannelFunctionIndex](GetChannelFunctionIndex) · [GetAttributeIndex](GetAttributeIndex) · [GetUIChannelIndex](GetUIChannelIndex)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getchannelfunction.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getchannelfunction.html
