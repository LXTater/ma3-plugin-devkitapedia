# SelectedTimer() [AI]
Gives you a handle to the timer currently selected in the Timers pool. `[P]`

---

## SelectedTimer()

### "[V2.2][Manual] Definition"
```lua
SelectedTimer()
```

### Returns
A handle to the selected timer object. `[P]`

### Example `[P]`
```lua
local tmr = SelectedTimer()
if tmr == nil then
  Printf("No timer selected")
  return
end
Printf("-- timer begin --")
tmr:Dump()
Printf("-- timer end --")
```
- Takes no arguments. `[P]`
- Timers act as stopwatches or countdowns. `[P]`

---

## See Also
[SelectedTimecode](SelectedTimecode) · [Timer](Timer)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_selectedtimer.html
