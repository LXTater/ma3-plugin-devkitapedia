# GetSample() [AI]
Reads a system metric such as CPU load or temperature by key. `[P]`

---

## GetSample(string)

### "[V2.2][Manual] Definition"
```lua
GetSample(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | One of `MEMORY`, `CPU`, `CPUTEMP`, `GPUTEMP`, `SYSTEMP`, `FANRPM` `[P]` |

### Returns
A float. The manual describes it as a percentage usage, though temperatures and fan speed are presumably in their own units. `[?]`

### Example `[P]`
```lua
return function()
    for _, key in ipairs({ "CPU", "MEMORY", "CPUTEMP", "FANRPM" }) do
        Printf("%s = %s", key, tostring(GetSample(key)))
    end
end
```
- Only the listed keys are accepted. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetDebugFPS](GetDebugFPS) · [Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getsample.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getsample.html
