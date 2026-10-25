# GetShowFileStatus() [AI]
Reports the current state of the show file as a string. `[P]`

---

## GetShowFileStatus()

### "[V2.2][Manual] Definition"
```lua
GetShowFileStatus()
```

### Returns
A string from the `Enums.ShowFileStatus` enum (e.g. NoShow, ShowLoaded, ShowSaving). `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local status = GetShowFileStatus()
Printf("Show file status: " .. status)
if status == "ShowLoaded" then
  Printf("Ready to work")
end
```
- Takes no arguments. `[P]`
- Other values listed include ShowDownloaded and DataNegotiationActive. `[P]`

---

## See Also
[NeedShowSave](NeedShowSave)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getshowfilestatus.html
