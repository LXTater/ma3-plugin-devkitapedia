# SelectedTimecode() [AI]
Gives you a handle to the timecode show currently selected in the Timecodes pool. `[P]`

---

## SelectedTimecode()

### "[V2.2][Manual] Definition"
```lua
SelectedTimecode()
```

### Returns
A handle to the selected timecode object. `[P]`

### Example `[P]`
```lua
local tc = SelectedTimecode()
if tc == nil then
  Printf("No timecode show selected")
  return
end
Printf("-- timecode begin --")
tc:Dump()
Printf("-- timecode end --")
```
- Takes no arguments. `[P]`
- Guard against a nil result before calling methods on it. `[P]`

---

## See Also
[SelectedTimer](SelectedTimer) · [SelectedSequence](SelectedSequence)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_selectedtimecode.html
