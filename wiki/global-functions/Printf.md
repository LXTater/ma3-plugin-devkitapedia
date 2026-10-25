# Printf() [AI]
Writes text to the Command Line History and the System Monitor. `[P]`

---

## Printf(string)

### "[V2.2][Manual] Definition"
```lua
Printf(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Text to output `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
Printf("plugin started")
```
- Output appears in both windows. `[P]`

---

## In the Wild: Reporting a refusal to the user `[onPC]`
```lua
Printf(NAME .. ': Macro ' .. MACRO .. ' is in use ("' .. tostring(m.name) .. '"). Nothing was changed.')
```
Every early exit prints a one-line reason, so a refused run is visible in the command line history. `[P]`

*Excerpt from the Steamboat Willie Player plugin, CC BY 4.0, Badass Lighting Tools. [Source](https://github.com/badasslighting/R-D-Lab/tree/main/MA3-Scribble-Animator/releases/steamboat-willie).*

See [Steamboat Willie Player](Steamboat-Willie-Player).

---

## See Also
[MessageBox](MessageBox)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_printf.html
