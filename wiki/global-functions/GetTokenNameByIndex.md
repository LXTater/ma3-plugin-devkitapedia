# GetTokenNameByIndex() [AI]
Returns the keyword that sits at a given index. `[P]`

---

## GetTokenNameByIndex(int)

### "[V2.2][Manual] Definition"
```lua
GetTokenNameByIndex(int)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| index | integer | Keyword index; the manual notes no obvious pattern to the numbering `[P]` |

### Returns
The keyword string, or nil when the index has no keyword. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
for i = 1, 50 do
  local word = GetTokenNameByIndex(i)
  if word then Printf(i .. " = " .. word) end
end
```
- Many indexes map to nothing and return nil. `[P]`
- The manual's own scan runs up to index 443. `[P]`

---

## See Also
[GetTokenName](GetTokenName)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_gettokennamebyindex.html
