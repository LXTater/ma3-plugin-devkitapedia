# GetTokenName() [AI]
Expands a short keyword form to the full keyword, or returns nil if none matches. `[P]`

---

## GetTokenName(string)

### "[V2.2][Manual] Definition"
```lua
GetTokenName(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Short form of a keyword `[P]` |

### Returns
The full keyword as a string, or nil when nothing matches. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local full = GetTokenName("go")
if full then
  Printf("go expands to " .. full)
else
  Printf("No keyword for that abbreviation")
end
```
- Always check for nil. `[P]`

---

## See Also
[GetTokenNameByIndex](GetTokenNameByIndex)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_gettokenname.html
