# BuildDetails() [AI]
Returns a table describing the software build, such as version, compile date and host type. `[P]`

---

## BuildDetails()

### "[V2.2][Manual] Definition"
```lua
BuildDetails()
```

### Returns
A table with string keys GitDate, GitHead, GitHash, CompileDate, CompileTime, BigVersion, SmallVersion, HostType, HostSubType, CodeType and boolean IsRelease. `[P]`

### Example `[P]`
```lua
local info = BuildDetails()
Printf("Version: " .. info.BigVersion)
Printf("Host: " .. info.HostType .. " / " .. info.HostSubType)
Printf("Release build: " .. tostring(info.IsRelease))
```
- IsRelease is a boolean, so convert it with tostring() before concatenating `[P]`.

---

## See Also
[ConfigTable](ConfigTable) · [ExportCSV](ExportCSV)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_builddetails.html
