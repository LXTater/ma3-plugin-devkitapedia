# Importing Plugins [AI]
How a plugin library gets from disk into the Plugins pool, and the import syntax that works. Everything on this page is `[P]` until probed on hardware.

---

## Where plugin files live `[P]`

Plugin libraries are read from the `gma3_library` tree, in the `datapools/plugins` folder. On a Windows onPC install this is under `C:\ProgramData\MALightingTechnology\gma3_library\datapools\plugins\`.

Putting files anywhere else is a `[SBX]` practice and is not covered here.

---

## Import syntax `[P]`

```
Import Plugin Library "MyLibrary" At Plugin 3 /nc
```

| Part | Use |
|------|-----|
| `Import Plugin Library` | Loads a plugin library (`.xml` plus its Lua files) from the plugins folder |
| `"MyLibrary"` | Library name, quoted |
| `At Plugin 3` | Destination pool slot |
| `/nc` | No-confirm. Skips the overwrite popup, useful in scripted installs |

### Gotchas

1. A plain `Import "MyLibrary" At Plugin 3` creates an **empty UserPlugin** in the slot instead of loading the library. Use `Import Plugin Library`.
2. Importing into an occupied slot prompts unless `/nc` is given. Delete the old plugin first if you want a clean replacement.
3. Back up whatever is already installed before replacing it. It may not be the version you expect.

---

## From Lua `[P]`

The command line can be driven from a plugin with `gma.cmd`:

```lua
gma.cmd('Import Plugin Library "MyLibrary" At Plugin 3 /nc')
```

---

## See Also
[Command Syntax Basics](Command-Syntax-Basics) · [Simple Plugin Template](Simple-Plugin-Template)

*Generated with Claude Sonnet 5.5 with Medium effort. Not verified on hardware; no Verified badge claimed.*
