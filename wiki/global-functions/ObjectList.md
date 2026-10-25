# ObjectList() [AI]
Builds a table of object handles from a command-line style selection string. `[P]`

---

## ObjectList(string[, table])

### "[V2.2][Manual] Definition"
```lua
ObjectList(string[, table])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Text that would select a range of objects on the command line `[P]` |
| table | table | Optional: `reverse_order`, `selected_as_default` booleans `[P]` |

### Returns
A table of matching object handles. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local list = ObjectList("Group 1 Thru 5")
for _, g in ipairs(list) do
  Printf(g.name)
end
```
- The optional table accepts reverse_order and selected_as_default. `[P]`

---

## See Also
[Patch](Patch) · [Programmer](Programmer)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_objectlist.html
