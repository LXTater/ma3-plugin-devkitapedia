# DefaultDisplayPositions() [AI]
Returns the handle holding the conventional default display layout, with the first seven screens as children. `[P]`

---

## DefaultDisplayPositions()

### "[V2.2][Manual] Definition"
```lua
DefaultDisplayPositions()
```

### Returns
One handle. The manual calls it the command line object, which contradicts its own description `[?]`. `[P]`

### Example `[P]`
```lua
local displays = DefaultDisplayPositions()
local d1 = displays[1]
d1:Dump()
d1.ShowMainMenu = not d1.ShowMainMenu  -- flip the control bar
```
- ShowMainMenu toggles the Control Bar according to the manual `[P]`.

---

## See Also
[CurrentScreenConfig](CurrentScreenConfig) · [DrawPointer](DrawPointer)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_defaultdisplaypositions.html
