# GetPathOverrideFor() [AI]
Returns a grandMA3 folder path rebased onto another location, such as a removable drive. `[P]`

---

## GetPathOverrideFor(string|integer, string[, boolean])

### "[V2.2][Manual] Definition"
```lua
GetPathOverrideFor(string|integer, string[, boolean])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| folder | string or integer | Folder name, or an `Enums.PathType` index `[P]` |
| base path | string | Base location to build the path on `[P]` |
| create | boolean (optional) | `true` creates the folder if absent; the manual does not mark it optional in the integer form `[?]` |

### Returns
A string with the first matching full path. `[P]`

### Example `[P]`
```lua
return function()
    local drive = "E:"  -- your removable drive base path
    local p = GetPathOverrideFor("macros", drive, false)
    Printf("Macros on drive: " .. p)
end
```
- Handy for placing folders on a connected USB stick. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[GetPath](GetPath) · [GetPathType](GetPathType) · [GetPathSeparator](GetPathSeparator)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpathoverridefor.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpathoverridefor.html
