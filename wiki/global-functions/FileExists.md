# FileExists() [AI]
Tells you whether a file is present at a given path. `[P]`

---

## FileExists(string)

### "[V2.2][Manual] Definition"
```lua
FileExists(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Full path including file name `[P]` |

### Returns
A boolean: `true` when the file exists, `false` otherwise. `[P]`

### Example `[P]`
```lua
return function()
    local path = GetPath(Enums.PathType.Library) .. GetPathSeparator() .. "settings.json"
    if FileExists(path) then
        Printf("Found " .. path)
    else
        Printf("Missing " .. path)
    end
end
```
- Pass a full path, not just a file name. `[P]`
- Available since version 2.2 per the manual. `[P]`

---

## See Also
[GetPath](GetPath) · [ExportJson](ExportJson) · [GetPathSeparator](GetPathSeparator)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_fileexists.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_fileexists.html
