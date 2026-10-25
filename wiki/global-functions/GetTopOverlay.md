# GetTopOverlay() [AI]
Returns a handle to the top overlay (the internal term for pop-ups and menus). `[P]`

---

## GetTopOverlay()

### "[V2.2][Manual] Definition"
```lua
GetTopOverlay()
```

### Returns
A handle to the top overlay, or nil if there is none. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local ov = GetTopOverlay()
if ov then
  ov:Dump()
end
```
- The manual says there are no arguments, but its example passes `1` and the text mentions an index `[?]`.

---

## See Also
[GetTopModal](GetTopModal) · [GetUIObjectAtPosition](GetUIObjectAtPosition)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_gettopoverlay.html
