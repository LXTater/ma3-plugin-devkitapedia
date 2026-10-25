# GetButton() [AI]
Reports which buttons on a grandMA3 hardware module are currently pressed. `[P]`

---

## GetButton(handle)

### "[V2.2][Manual] Definition"
```lua
GetButton(handle)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | The hardware module to read; the manual does not state the object type `[?]` |

### Returns
A table of 512 boolean entries, 1-indexed; `true` means pressed or fader touched. `[P]`

### Example `[P]`
```lua
return function(display_handle, module)
    local states = module and GetButton(module)
    if not states then Printf("No module state") return end
    for i, down in ipairs(states) do
        if down then Printf("Button %d is down", i) end
    end
end
```
- Check for `nil` before iterating. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getbutton.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getbutton.html
