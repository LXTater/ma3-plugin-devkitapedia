# FixtureType() [AI]
Returns a handle to the fixture type that the command line is currently pointed at. `[P]`

---

## FixtureType()

### "[V2.2][Manual] Definition"
```lua
FixtureType()
```

### Returns
A handle to the fixture type, or `nil` if the command line destination is not a fixture type. `[P]`

### Example `[P]`
```lua
return function()
    Cmd("ChangeDestination Root")
    Cmd("ChangeDestination 'ShowData'.'Patch'.'FixtureTypes'")
    Cmd("ChangeDestination 1")
    local ft = FixtureType()
    if ft then Dump(ft) else Printf("Not at a fixture type") end
    Cmd("ChangeDestination Root")
end
```
- Only meaningful when the destination is a fixture type. `[P]`
- Reset the destination to Root afterwards. `[P]`

---

## See Also
[Cmd](Cmd) · [Root](Root)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_fixturetype.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_fixturetype.html
