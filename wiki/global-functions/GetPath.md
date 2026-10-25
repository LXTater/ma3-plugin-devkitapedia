# GetPath() [AI]
Returns the full path of a grandMA3 folder, chosen by name or by path-type number. `[P]`

---

## GetPath(string[, boolean] | integer)

### "[V2.2][Manual] Definition"
```lua
GetPath(string[, boolean])
GetPath(integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Folder name `[P]` |
| boolean | boolean (optional, string form only) | `true` creates the folder if missing `[P]` |
| integer | integer | Index into `Enums.PathType` `[P]` |

### Returns
A string with the first matching full path. `[P]`

### Example `[P]`
```lua
return function()
    Printf("by enum: " .. GetPath(Enums.PathType.Library))
    Printf("by name: " .. GetPath("showfiles", true))
end
```
- Pass `true` as the second argument to create a missing folder. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetPathOverrideFor](GetPathOverrideFor) · [GetPathSeparator](GetPathSeparator) · [GetPathType](GetPathType)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpath.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpath.html
