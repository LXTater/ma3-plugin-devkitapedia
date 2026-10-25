# TextInput() [AI]
Opens a text entry pop-up and returns what the user typed. `[P]`

---

## TextInput([title [, default [, x [, y]]]])

### "[V2.2][Manual] Definition"
```lua
TextInput([title [, default [, x [, y]]]])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| title | String (optional) | Pop-up title; a default "Edit" prefix is always shown. `[P]` |
| default | String (optional) | Pre-filled text. `[P]` |
| x | Integer (optional) | Horizontal position across all screens; 0 is the left edge, nil centres. `[P]` |
| y | Integer (optional) | Vertical position; 0 is the top edge, nil centres. `[P]` |

### Returns
A string with the entered text. `[P]`

### Example `[P]`
```lua
local name = TextInput("Cue name", "New cue")
Printf("You entered: " .. tostring(name))
```
- Blocks the calling plugin until the user closes the pop-up `[?]`.
- Nil x or y centres the pop-up. `[P]`

---

## See Also
[Echo](Echo) · [Printf](Printf) · [Timer](Timer)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_textinput.html
