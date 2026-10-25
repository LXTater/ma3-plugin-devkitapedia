# Steamboat Willie Player [AI]
A small, complete grandMA3 plugin that shows how several global functions fit together: it imports 153 Scribble frames, stores a macro, and animates the macro's Scribble at 12 fps. It is released free under CC BY 4.0, credited to Badass Lighting Tools. [Release folder](https://github.com/badasslighting/R-D-Lab/tree/main/MA3-Scribble-Animator/releases/steamboat-willie)

---

## What it does `[V2.5.1][onPC]`

- Imports frames `SW001`-`SW153` into Scribble slots 101-253 and plays them on Macro 901.
- Run it once to start, run it again to stop.
- Per its release notes, it was imported and played on onPC 2.5.1 with 153/153 frames loaded. Hardware/software details for the verification template are not recorded here yet. `[?]`

---

## Patterns worth copying `[P]`

### 1. Refuse before changing anything
All slots are checked first. If a slot holds a Scribble with a different name, or Macro 901 shows a frame that is not the plugin's, it prints why and returns without modifying the show.

```lua
local s = pool:Ptr(FIRST + i - 1)
if s and s.name ~= FRAMES[i] then
  Printf(NAME .. ': Scribble ' .. (FIRST + i - 1) .. ' is "' .. tostring(s.name) .. '"...')
  return
end
```
Uses [ShowData](ShowData), [DataPool](DataPool) and [Printf](Printf).

### 2. Start/stop toggle with a heartbeat
State lives in a global table. A stop is honoured only if the heartbeat is fresh, because a loop killed by a show load or a closed terminal leaves `running = true` behind.

```lua
BLTScribPlayers = BLTScribPlayers or {}
local st = BLTScribPlayers[NAME]
if st and st.running and st.beat and now() - st.beat < 1 then
  st.running = false
  return
end
```

### 3. Time-based loop that yields
```lua
while st.running do
  local k = math.floor((now() - start) * FPS)
  -- choose idx for loop / pingpong / once, then:
  if idx ~= last then m.Scribble = frames[idx]; last = idx end
  st.beat = now()
  coroutine.yield(0)
end
```
The Scribble is only reassigned when the frame index changes, and the loop yields every pass so the console stays responsive. Uses [Time](Time).

### 4. Unique blank macro label
A blank label is used so the drawing is not covered, but a second macro with the same blank name is displayed as `#2`. The plugin therefore picks a run of spaces no other macro uses. `[P]`

---

## Known behaviour
On a Macro button the Scribble is drawn at roughly 55% brightness, per the release notes. `[P]`

---

## See Also
[Cmd](Cmd) · [ShowData](ShowData) · [DataPool](DataPool) · [Time](Time) · [Printf](Printf) · [Global Functions](Global-Functions)

*Generated with Claude Sonnet 5.5 with Medium effort. Excerpts: CC BY 4.0, Badass Lighting Tools.*
