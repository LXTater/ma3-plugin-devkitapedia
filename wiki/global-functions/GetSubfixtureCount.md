# GetSubfixtureCount() [AI]
Counts all fixtures patched in the show file. `[P]`

---

## GetSubfixtureCount()

### "[V2.2][Manual] Definition"
```lua
GetSubfixtureCount()
```

### Returns
One integer: the number of patched fixtures across all stages. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local total = GetSubfixtureCount()
Printf("Patched fixtures: " .. total)
for i = 1, total do
  local f = GetSubfixture(i)
  -- inspect f here
end
```
- Takes no arguments. `[P]`

---

## See Also
[GetSubfixture](GetSubfixture)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getsubfixturecount.html
