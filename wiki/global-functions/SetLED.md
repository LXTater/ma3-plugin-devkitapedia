# SetLED() [AI]
Sends brightness values for the LEDs of a console module; the system takes the LEDs back after about two seconds. `[P]`

---

## SetLED(handle, table)

### "[V2.2][Manual] Definition"
```lua
SetLED(handle, table)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| handle | Handle | The module to address (the manual's example gets it from the console's USB notifier). `[P]` |
| table | Table | Indexed integers 0-255 for brightness; -1 hands that LED back to the system. `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
local leds = {}
for i = 1, 256 do leds[i] = -1 end   -- -1 = leave to the system
leds[1] = 255                        -- one LED at full brightness
SetLED(moduleHandle, leds)           -- moduleHandle obtained elsewhere
```
- Values above 0 on an index with no LED can crash and reboot the module. `[P]`
- The manual says the table should have 1024 indexes, yet its own example fills 256 `[?]`.
- The manual's parameter text says the function takes no arguments, contradicting its signature `[?]`.

---

## See Also
[Time](Time) · [Timer](Timer) · [SetBlockInput](SetBlockInput)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_setled.html
