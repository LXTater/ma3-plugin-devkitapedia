# ExportCSV() [AI]
Writes a Lua table to a CSV file. `[P]`

---

## ExportCSV(filename, export_data)

### "[V2.2][Manual] Definition"
```lua
ExportCSV(filename, export_data)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| filename | string | Full path including file name. |
| export_data | table | The table to export. |

### Returns
true on success, false on failure. `[P]`

### Example `[P]`
```lua
local path = GetPath(Enums.PathType.Library) .. "/info.csv"
local ok = ExportCSV(path, BuildDetails())
Printf(ok and ("Saved " .. path) or "CSV export failed")
```
- The manual warns the output may not be formatted correctly `[P]`.

---

## See Also
[Export](Export) · [BuildDetails](BuildDetails)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_exportcsv.html
