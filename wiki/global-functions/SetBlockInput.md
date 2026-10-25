# SetBlockInput() [AI]
Turns blocking of USB keyboard and mouse input on or off for the local station. The manual calls it an internal function used in system tests. `[P]`

---

## SetBlockInput(boolean)

### "[V2.2][Manual] Definition"
```lua
SetBlockInput(boolean)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| boolean | Boolean | true or 1 blocks input; false or 0 unblocks it. `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
SetBlockInput(true)
coroutine.yield(5)   -- keep input blocked for five seconds
SetBlockInput(false)
```
- Only affects the station that runs the call. `[P]`
- If a station stays blocked, the manual says pressing A, S, D and F together unblocks it. `[P]`
- Use with care: always schedule the unblock. `[P]`

---

## See Also
[Timer](Timer) · [Time](Time) · [Echo](Echo)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_setblockinput.html
