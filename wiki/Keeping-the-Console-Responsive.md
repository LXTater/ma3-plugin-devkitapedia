# Keeping the Console Responsive [AI]
Lua plugins share the console's UI thread. Work done in a callback can stall the surface for as long as it runs. `[P]`

---

## Guidelines `[P]`

| Do | Avoid |
|----|-------|
| Precompute and cache assets once, ideally to disk before they are needed | Generating or encoding assets inside an input or per-frame handler |
| Keep per-event work to showing, hiding or moving existing objects | Large loops or repeated imports during an event |
| Yield with `gma.sleep` in long loops so the UI can refresh | Tight loops with no yield |
| Time a feature on onPC before calling it done | Assuming a fast PC reflects console hardware |

Even a stall of about two seconds is noticeable on the surface and should be treated as a bug.

---

## Measuring `[P]`

```lua
local t0 = os.clock()
-- work under test
gma.echo(string.format("took %.3f s", os.clock() - t0))
```

Run the same test on console hardware where possible, since onPC timings are optimistic.

---

## See Also
[Simple Plugin Template](Simple-Plugin-Template)

*Generated with Claude Sonnet 5.5 with Medium effort. Not verified on hardware.*
