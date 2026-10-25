# FindTexture() [AI]
Looks up a texture by name and gives back a handle to it. `[P]`

---

## FindTexture(string)

### "[V2.2][Manual] Definition"
```lua
FindTexture(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Texture name without its file extension `[P]` |

### Returns
A handle to the texture, or `nil` when it does not exist. `[P]`

### Example `[P]`
```lua
return function()
    local tex = FindTexture("logo")
    if tex then
        Dump(tex)
    else
        Printf("No texture called logo")
    end
end
```
- Leave off the file type in the name. `[P]`
- The manual's description misspells the function name once; the signature is FindTexture. `[P]`

---

## See Also
[Printf](Printf)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_findtexture.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_findtexture.html
