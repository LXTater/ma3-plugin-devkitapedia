# Timer() [AI]
Calls a function repeatedly at a fixed interval for a set number of repeats. `[P]`

---

## Timer(function, integer, integer [, cleanup [, handle]])

### "[V2.2][Manual] Definition"
```lua
Timer(function, integer, integer [, cleanup [, handle]])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| function | Function | The function to call each time. `[P]` |
| integer | Integer | Seconds between calls. `[P]` |
| integer | Integer | How many times to call it. `[P]` |
| cleanup | Function or nil (optional) | Called when the timer finishes. `[P]` |
| handle | Handle (optional) | Object passed to the called function. `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
local count = 0
local function tick()
  count = count + 1
  Printf("tick " .. count)
end
local function done()
  Printf("finished")
end
Timer(tick, 1, 3, done)
```
- The manual's signature lists the first argument as a string, but its parameter list says function `[?]`.

---

## See Also
[Time](Time) · [Unhook](Unhook) · [SetBlockInput](SetBlockInput)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_timer.html
