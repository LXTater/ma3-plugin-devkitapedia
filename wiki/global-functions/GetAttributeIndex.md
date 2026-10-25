# GetAttributeIndex() [AI]
Gives the zero-based index of an attribute from its system name. `[P]`

---

## GetAttributeIndex(string)

### "[V2.2][Manual] Definition"
```lua
GetAttributeIndex(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | System name of the attribute `[P]` |

### Returns
An integer index (0-based). `[P]`

### Example `[P]`
```lua
return function()
    local i = GetAttributeIndex("Gobo1")
    if i then Printf("Gobo1 is attribute #%d", i) else Printf("Not found") end
end
```
- The manual's return text mentions fixture counts, which does not fit the function; treat the integer index as the real result. `[?]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetAttributeCount](GetAttributeCount) · [GetChannelFunction](GetChannelFunction) · [GetUIChannelIndex](GetUIChannelIndex)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getattributeindex.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getattributeindex.html
