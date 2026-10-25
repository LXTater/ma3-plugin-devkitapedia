# Export() [AI]
Writes a Lua table to an XML file; the counterpart of the object-free Import. `[P]`

---

## Export(filename, export_data)

### "[V2.2][Manual] Definition"
```lua
Export(filename, export_data)
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
local ok = Export(GetPath(Enums.PathType.Library) .. "/info.xml", BuildDetails())
Printf(ok and "Exported" or "Export failed")
```
- An object-based Export also exists `[P]`.
- The Library path enum is from general knowledge `[?]`.

---

## See Also
[ExportCSV](ExportCSV) · [BuildDetails](BuildDetails)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_export.html
