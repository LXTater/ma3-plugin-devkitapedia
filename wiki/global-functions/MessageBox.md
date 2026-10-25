# MessageBox() [AI]
Shows a pop-up message box built from a table; supports buttons, inputs, toggles and selectors. `[P]`

---

## MessageBox(table)

### "[V2.2][Manual] Definition"
```lua
MessageBox(table)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| table | table | Fields such as title, message, timeout, commands, inputs, states, selectors (all optional) `[P]` |

### Returns
A table with `success`, `result`, and `inputs`/`states`/`selectors` when those were defined. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local r = MessageBox({
  title = "Confirm",
  message = "Proceed?",
  commands = {{value = 1, name = "Yes"}, {value = 0, name = "No"}}
})
Printf("picked: " .. r.result)
```
- Reading `inputs`, `states` or `selectors` on a box without them raises an error. `[P]`
- Manual text and examples differ in `blackfilter` vs `blackFilter` casing `[?]`.
- Whether it blocks the plugin until the box closes is not stated `[?]`.

---

## See Also
[GetTopModal](GetTopModal)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_messagebox.html
