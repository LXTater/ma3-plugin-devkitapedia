# FromAddr() [AI]
Turns an address string into a handle that you can use in commands and Lua. `[P]`

---

## FromAddr(string[, handle])

### "[V2.2][Manual] Definition"
```lua
FromAddr(string[, handle])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Numbered or named address of the object `[P]` |
| handle | handle (optional) | Base to resolve from; defaults to root. Must lie on the path from root to the target `[P]` |

### Returns
A handle to the addressed object. `[P]`

### Example `[P]`
```lua
return function()
    local h = FromAddr("14.1.1")
    if h then
        Printf("Numbered: " .. h:AddrNative(nil, false))
        Printf("Named: " .. h:AddrNative(nil, true))
    end
    local rel = FromAddr("Sequences.Main", DataPool())
    Dump(rel)
end
```
- The optional base handle shortens relative lookups. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[DataPool](DataPool)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_fromaddr.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_fromaddr.html
