# ShowData() [AI]
Gives you a handle to the ShowData object at Root/ShowData. `[P]`

---

## ShowData()

### "[V2.2][Manual] Definition"
```lua
ShowData()
```

### Returns
A handle to the ShowData object. `[P]`

### Example `[P]`
```lua
Printf("-- ShowData begin --")
ShowData():Dump()
Printf("-- ShowData end --")
```
- Takes no arguments. `[P]`

---

## In the Wild: Reaching the Scribbles pool `[onPC]`
```lua
local pool = ShowData().Scribbles
local frame = pool:Ptr(101)   -- nil if the slot is empty
```
Used to check every target slot before touching anything, so the plugin never overwrites a Scribble that is not its own. `[P]`

*Excerpt from the Steamboat Willie Player plugin, CC BY 4.0, Badass Lighting Tools. [Source](https://github.com/badasslighting/R-D-Lab/tree/main/MA3-Scribble-Animator/releases/steamboat-willie).*

See [Steamboat Willie Player](Steamboat-Willie-Player).

---

## See Also
[ShowSettings](ShowSettings) · [Root](Root)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_showdata.html
