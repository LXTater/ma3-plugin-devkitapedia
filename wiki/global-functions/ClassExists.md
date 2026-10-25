# ClassExists() [AI]
Tells you whether a given word is a known class name. `[P]`

---

## ClassExists(string)

### "[V2.2][Manual] Definition"
```lua
ClassExists(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | A single word that may be a class name. |

### Returns
true if the word is a class, otherwise false. `[P]`

### Example `[P]`
```lua
local word = "Display"
Printf(word .. (ClassExists(word) and " is a class" or " is not a class"))
```
- Pass a single word only `[P]`.

---

## See Also
[Echo](Echo)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_classexists.html
