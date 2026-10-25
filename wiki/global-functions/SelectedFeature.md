# SelectedFeature() [AI]
Gives you a handle to the feature that is currently selected. `[P]`

---

## SelectedFeature()

### "[V2.2][Manual] Definition"
```lua
SelectedFeature()
```

### Returns
A handle to the selected feature. `[P]`

### Example `[P]`
```lua
local obj = SelectedFeature()
if obj then
  Printf("--- SelectedFeature ---")
  obj:Dump()
else
  Printf("SelectedFeature: nothing returned")
end
```
- Takes no arguments. `[P]`
- Check the result before use in case nothing is selected `[?]`.

---

## See Also
[SelectedSequence](SelectedSequence) · [SelectedLayout](SelectedLayout)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_selectedfeature.html
