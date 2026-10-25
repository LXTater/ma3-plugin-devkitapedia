# GetTopModal() [AI]
Returns the topmost open modal pop-up, which blocks the rest of the UI while shown. `[P]`

---

## GetTopModal()

### "[V2.2][Manual] Definition"
```lua
GetTopModal()
```

### Returns
A handle to the top modal, or nil if no modal is open. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local modal = GetTopModal()
if modal then
  modal:Dump()
else
  Printf("No modal is open")
end
```
- Takes no arguments. `[P]`

---

## See Also
[GetTopOverlay](GetTopOverlay) · [MessageBox](MessageBox)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_gettopmodal.html
