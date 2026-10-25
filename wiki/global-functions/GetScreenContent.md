# GetScreenContent() [AI]
Returns the screen content object that belongs to a screen configuration. `[P]`

---

## GetScreenContent(handle)

### "[V2.2][Manual] Definition"
```lua
GetScreenContent(handle)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | A screen configuration `[P]` |

### Returns
A handle to the screen content. `[P]`

### Example `[P]`
```lua
return function()
    local cfg = CurrentUser().ScreenConfig
    local content = cfg and GetScreenContent(cfg)
    if content then Dump(content) else Printf("No screen content") end
end
```
- Use the current user's screen configuration as the input, as the manual's example does. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[CurrentUser](CurrentUser) · [GetDisplayCollect](GetDisplayCollect)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getscreencontent.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getscreencontent.html
