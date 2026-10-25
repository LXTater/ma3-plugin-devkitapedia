# FirstDmxModeFixture() [AI]
Returns the first fixture in the show that uses a particular DMX mode. `[P]`

---

## FirstDmxModeFixture(handle)

### "[V2.2][Manual] Definition"
```lua
FirstDmxModeFixture(handle)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | handle | A DMX mode object `[P]` |

### Returns
A handle to the first fixture using that mode. `[P]`

### Example `[P]`
```lua
return function()
    local ft = Root().ShowData.Patch.FixtureTypes:Children()[1]
    local mode = ft and ft.DMXModes:Children()[1]
    if not mode then
        Printf("No fixture type or DMX mode found")
        return
    end
    Dump(FirstDmxModeFixture(mode))
end
```
- You must obtain the mode handle yourself, for example from a fixture type. `[P]`
- Available since version 2.2 per the manual. `[P]`

---

## See Also
[Printf](Printf) · [Root](Root)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_firstdmxmodefixture.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_firstdmxmodefixture.html
