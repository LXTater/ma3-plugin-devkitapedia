# GetCurrentCue() [AI]
Returns the most recently activated cue of the selected sequence. `[P]`

---

## GetCurrentCue()

### "[V2.2][Manual] Definition"
```lua
GetCurrentCue()
```

### Returns
A handle to the current cue. `[P]`

### Example `[P]`
```lua
return function()
    local cue = GetCurrentCue()
    if cue then
        Printf("Current cue: " .. tostring(cue.name))
        Dump(cue)
    end
end
```
- Works relative to the currently selected sequence. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[Printf](Printf) · [DataPool](DataPool)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getcurrentcue.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getcurrentcue.html
