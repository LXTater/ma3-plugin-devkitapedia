# Import() [AI]
Loads a Lua table previously stored as XML; the counterpart of Export. `[P]`

---

## Import(string)

### "[V2.2][Manual] Definition"
```lua
Import(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Full path of the file, including file name `[P]` |

### Returns
The imported table. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local t = Import("C:/path/to/mytable.xml")
if t then
  for k, v in pairs(t) do Printf(tostring(k) .. " = " .. tostring(v)) end
end
```
- Check for a failed import before using the table. `[P]`

---

## See Also
[Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_import.html
