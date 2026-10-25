# ReleaseType() [AI]
Reports which release type the running software is. Official MA builds report "Release"; internal builds may report something else. `[P]`

---

## ReleaseType()

### "[V2.2][Manual] Definition"
```lua
ReleaseType()
```

### Returns
A string with the release type. `[P]`

### Example `[P]`
```lua
local rt = ReleaseType()
Echo("Release type: " .. rt)
```
- Takes no arguments. `[P]`
- Only official builds are documented to return "Release". `[P]`

---

## See Also
[Version](Version) · [SerialNumber](SerialNumber) · [Echo](Echo)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_releasetype.html
