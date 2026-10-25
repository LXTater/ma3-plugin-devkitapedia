# Command Syntax Basics [AI]
The command line is the main bridge between a plugin and the show. This page covers the syntax rules worth knowing before calling `gma.cmd`. All entries are `[P]`.

---

## Rules of thumb `[P]`

| Rule | Example |
|------|---------|
| Quote names | `Store Sequence 1 Cue 1 "Look"` |
| Chain objects with `+`, ranges with `Thru` | `Group 1 + Group 3`, `Group 19 Thru 24` |
| Append `/nc` to destructive commands in scripts | `Delete Cue 5 /nc` |
| Numbers are more stable than names | `Group 17` rather than `Group "Front"` |
| Keywords can be abbreviated | `Sel`, `Fix`, `Seq` |

Names can be duplicated or renamed; numbers can be moved. For anything long-lived, prefer object references (see [Macro Object References](Macro-Object-References)).

---

## Calling from Lua `[P]`

```lua
gma.cmd('Fixture 1 Thru 10')
gma.cmd('At Full')
gma.cmd('Store Cue 1 /nc')
```

Each call is one command-line entry. Commands run through the same parser as typed input, so a command that would open a popup on the console will open one from a plugin too.

---

## Recipe re-evaluation `[P]`

```
Cook Sequence 1002
```

Re-evaluates recipes on the target. Works on sequences, cues and presets. A merge/overwrite/remove/cancel choice follows unless suppressed.

---

## See Also
[Importing Plugins](Importing-Plugins) · [Macro Object References](Macro-Object-References)

*Generated with Claude Sonnet 5.5 with Medium effort. Not verified on hardware.*
