# SelectedSequence() [AI]
Gives you a handle to the sequence that is currently selected. `[P]`

---

## SelectedSequence()

### "[V2.2][Manual] Definition"
```lua
SelectedSequence()
```

### Returns
A handle to the selected sequence. `[P]`

### Example `[P]`
```lua
local seq = SelectedSequence()
if seq then
  Printf("Selected sequence: " .. seq.name)
else
  Printf("No sequence selected")
end
```
- Takes no arguments. `[P]`
- Pass the handle to functions like ToAddr or HandleToStr to turn it into text. `[P]`

---

## See Also
[SelectedLayout](SelectedLayout) · [SelectedTimecode](SelectedTimecode) · [ToAddr](ToAddr) · [HandleToStr](HandleToStr)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_selectedsequence.html
