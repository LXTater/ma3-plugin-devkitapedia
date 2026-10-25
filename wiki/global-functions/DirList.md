# DirList() [AI]
Lists files in a directory, optionally filtered by a wildcard pattern. `[P]`

---

## DirList(string[, string])

### "[V2.2][Manual] Definition"
```lua
DirList(string[, string])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| path | string | Directory to list. |
| filter | string | Optional. Pattern; `*` is a wildcard. |

### Returns
A table of entries, each with name (string), size (bytes) and time (timestamp). `[P]`

### Example `[P]`
```lua
local dir = GetPath(Enums.PathType.Showfiles)
for _, f in ipairs(DirList(dir, "*.show")) do
  Printf(f.name .. "  " .. f.size .. " bytes  t=" .. f.time)
end
```
- The enum used to get the show file path above is from general knowledge `[?]`.

---

## See Also
[Export](Export) · [ExportCSV](ExportCSV)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_dirlist.html
