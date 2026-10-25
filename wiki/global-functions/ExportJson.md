# ExportJson() [AI]
Writes the contents of a Lua table out to a file as JSON. `[P]`

---

## ExportJson(filename, export_data)

### "[V2.2][Manual] Definition"
```lua
ExportJson(filename, export_data)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| filename | string | Full path and name of the file to write `[P]` |
| export_data | table | Lua table to serialise `[P]` |

### Returns
A boolean: `true` if the export worked, `false` if it failed. `[P]`

### Example `[P]`
```lua
return function()
    local sep  = GetPathSeparator()
    local path = GetPath(Enums.PathType.Library) .. sep .. "my_export.json"
    local ok = ExportJson(path, { name = "demo", values = { 1, 2, 3 } })
    Printf(ok and ("Saved to " .. path) or "Export failed")
end
```
- The manual warns the output may not always be strictly valid JSON. `[P]`
- Introduced in version 2.2 per the manual. `[P]`

---

## See Also
[Printf](Printf) · [GetPath](GetPath) · [FileExists](FileExists)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_exportjson.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_exportjson.html
