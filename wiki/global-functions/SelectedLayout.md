# SelectedLayout() [AI]
Gives you a handle to the layout that is currently selected in the layout pool. `[P]`

---

## SelectedLayout()

### "[V2.2][Manual] Definition"
```lua
SelectedLayout()
```

### Returns
A handle to the selected layout. `[P]`

### Example `[P]`
```lua
local obj = SelectedLayout()
if obj then
  Printf("--- SelectedLayout ---")
  obj:Dump()
else
  Printf("SelectedLayout: nothing returned")
end
```
- Takes no arguments. `[P]`
- Layouts are 2D views for arranging fixtures, macros, groups and other pool objects. `[P]`

---

## See Also
[SelectedSequence](SelectedSequence) · [SelectedTimer](SelectedTimer)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_selectedlayout.html
