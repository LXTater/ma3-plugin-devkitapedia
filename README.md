# LXTater's MA3 Plugin Devkitapedia
# !!! UNDER DEVELOPMENT !!!

Unofficial devkit and wiki for **grandMA3 plugin development**.

MA3's Lua plugin API is powerful but barely documented. The official docs give you function signatures with no context, no examples, and no explanation of the dozens of undocumented capabilities buried in the engine. This repo fills that gap — every entry is tested on real hardware, by real humans. I have been so tired of scrounging Google's third or fourth page to see if someone has the right keyword. My CTRL + F keys have worn completely out.

---

## What's in here

**Wiki** - Still Trying to build everything out.
- What version it was tested on
- Screenshots where they help
- Gotchas that will waste your afternoon if you don't know them

**Probes** — minimal test plugins that verify a single behavior. Run them on your build to confirm before you build on top.

**Dev Tools** — utility plugins for inspecting the live UI tree, dumping object properties, and testing signal wiring without restarting the console.

---

## Trust tiers

Everything should include one of these tags

| Badge | Meaning |
|-------|---------|
| `[V] VERIFIED` | Tested on hardware, log output confirmed. Build on this. |
| `[P] PROVISIONAL` | Reasoned from MA source or partial testing. Probably right, verify before depending on it. |
| `[?] UNKNOWN` | Documented as a question. Needs a probe. |

If an entry doesn't have a badge, treat it as `PROVISIONAL`.

---
# !!! UNDER DEVELOPMENT !!!
## Boundary markers

If we are stretching the abilities of the LUA sandbox, or there's a less-than-normal method to do something, please include one of these tags:
| Marker | Meaning |
|--------|---------|
| `[UND] UNDOCUMENTED` | Uses real API surfaces that MA hasn't publicly documented. Works, but we're only guessing. |
| `[SBX] SANDBOX` | Pushes against sandbox boundaries (editing `lib_menus`, etc.). Development/lab use. Understand that this should never go on a lighting console, and you can brick your entire showfile. |
| `[AI] AI Involvement` | If a certain task, plugin, etc has been created entirley by AI, or if generative AI was utilized and not 100% human vetted, it will have this tag.  |

---
# !!! UNDER DEVELOPMENT !!!
## Tested on

- **grandMA3 onPC v2.3.2.0**, Windows 111
- Hardware testing done on an i9-13900K / RTX 4080 Super
- **GrandMA3 Full Size v2.3.2.0

Results may differ on older software versions, real console hardware, or MA3 onPC on macOS. Version-specific notes are included where known.

---
# !!! UNDER DEVELOPMENT !!!
## Repo structure

```
ma3-plugin-devkitapedia/
├── wiki/                    # All knowledge base entries
├── probes/                  # Minimal test plugins (one hypothesis each)
├── devtools/                # Utility plugins and HTML dev panels
├── assets/                  # Screenshots, diagrams
├── prompts/                 # AI session prompts used during research
└── README.md
```

---
# !!! UNDER DEVELOPMENT !!!
## How to use the probes

Each probe is a standalone MA3 plugin. Install like any plugin:


---
# !!! UNDER DEVELOPMENT !!!
## Who

**LXTater** — Lighting Design, Programmer, and very very tired of guessing.

---
---
# !!! UNDER DEVELOPMENT !!!
## AI Declreation

AI has been utilized in this project. For the sake of transparency, a [AI] label will be added to anything that generative AI was used for.
The current use of AI in this project has been limited to: Data Parsing (Scanning through MA UI Files/Backend), and with help organizing and creating the MDs for this wiki.

---
# !!! UNDER DEVELOPMENT !!!
## Disclaimer

This is an unofficial community resource. Not affiliated with or endorsed by MA Lighting. All findings are based on reverse-engineering the publicly installed software on the developer's own machine. No proprietary source code is redistributed — only descriptions of observed behavior and original code written against the public API surface.

Use at your own risk. Don't crash the show.

# !!! UNDER DEVELOPMENT !!!
