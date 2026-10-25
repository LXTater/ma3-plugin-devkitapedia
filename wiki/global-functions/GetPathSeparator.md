# GetPathSeparator() [AI]
Returns the folder separator character used by the operating system the software runs on. `[P]`

---

## GetPathSeparator()

### "[V2.2][Manual] Definition"
```lua
GetPathSeparator()
```

### Returns
A one-character string. `[P]`

### Example `[P]`
```lua
return function()
    local sep = GetPathSeparator()
    Printf("Separator is '" .. sep .. "'")
    Printf("Joined: " .. "a" .. sep .. "b")
end
```
- Differs between Windows and Linux/macOS, so use it when building paths. `[P]`
- The manual's page address spells it `getpathseparater`. `[P]`

---

## See Also
[GetPath](GetPath) · [FileExists](FileExists)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpathseparater.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getpathseparater.html
