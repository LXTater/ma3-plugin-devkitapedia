# GetClassDerivationLevel() [AI]
Returns the derivation level index for a class given its name. `[P]`

---

## GetClassDerivationLevel(string)

### "[V2.2][Manual] Definition"
```lua
GetClassDerivationLevel(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Class name `[P]` |

### Returns
An integer derivation level index. `[P]`

### Example `[P]`
```lua
return function()
    local lvl = GetClassDerivationLevel("Sequence")
    if lvl then Printf("Sequence derivation level: %d", lvl)
    else Printf("Unknown class") end
end
```
- Returns `nil` for unknown names in the manual's example handling. `[?]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getclassderivationlevel.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getclassderivationlevel.html
