# Time() [AI]
Returns how many seconds the application has been running, as a float (not time of day). `[P]`

---

## Time()

### "[V2.2][Manual] Definition"
```lua
Time()
```

### Returns
A number: seconds since the grandMA3 application started. `[P]`

### Example `[P]`
```lua
local t = Time()
local d = math.floor(t / 86400)
local h = math.floor(t % 86400 / 3600)
local m = math.floor(t % 3600 / 60)
local s = math.floor(t % 60)
Printf("Up for %dd %02d:%02d:%02d", d, h, m, s)
```
- Works like a stopwatch started at application launch. `[P]`

---

## In the Wild: Timing an animation without drifting `[onPC]`
```lua
local now = Time or os.clock
local start = now()
local k = math.floor((now() - start) * FPS)   -- frame index from elapsed time
```
Deriving the frame from elapsed time, not from a counter, keeps the speed steady if a loop iteration runs late. `[P]`

*Excerpt from the Steamboat Willie Player plugin, CC BY 4.0, Badass Lighting Tools. [Source](https://github.com/badasslighting/R-D-Lab/tree/main/MA3-Scribble-Animator/releases/steamboat-willie).*

See [Steamboat Willie Player](Steamboat-Willie-Player).

---

## See Also
[Timer](Timer) · [SerialNumber](SerialNumber) · [Version](Version)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_time.html
