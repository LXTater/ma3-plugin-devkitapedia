# LXTater's MA3 Plugin Devkitapedia
# !!! UNDER DEVELOPMENT !!!

Unofficial devkit and wiki for **grandMA3 plugin development**.

MA3's Lua plugin API is powerful but barely documented. The official docs give you function signatures with no context, no examples, and no explanation of the dozens of undocumented capabilities buried in the engine. This repo fills that gap — every entry is tested on real hardware, includes working code, and tells you what actually happens when you call it.

---

## What's in here

**Wiki** — the main knowledge base. Organized by topic, not by alphabet. Each entry has:
- What it does (one sentence)
- Working code you can paste into a plugin
- What version it was tested on
- Screenshots where they help
- Gotchas that will waste your afternoon if you don't know them

**Probes** — minimal test plugins that verify a single behavior. Run them on your build to confirm before you build on top.

**Dev Tools** — utility plugins for inspecting the live UI tree, dumping object properties, and testing signal wiring without restarting the console.

---

## Trust tiers

Every claim in this repo is marked with one of three tiers.

| Badge | Meaning |
|-------|---------|
| `[V] VERIFIED` | Tested on hardware, log output confirmed. Build on this. |
| `[P] PROVISIONAL` | Reasoned from MA source or partial testing. Probably right, verify before depending on it. |
| `[?] UNKNOWN` | Documented as a question. Needs a probe. |

If an entry doesn't have a badge, treat it as `PROVISIONAL`.

---
# !!! UNDER DEVELOPMENT !!!
## Boundary markers

Some techniques go beyond what MA officially supports. These are marked clearly so you know what you're getting into.

| Marker | Meaning |
|--------|---------|
| `[STD] STANDARD` | Uses the documented or clearly-intended plugin API. Safe for production show files. |
| `[UND] UNDOCUMENTED` | Uses real API surfaces that MA hasn't publicly documented. Works, but could break in a future version. |
| `[SBX] SANDBOX EDGE` | Pushes against sandbox boundaries (editing `lib_menus`, using `io.*`, `os.*`, etc.). Development/lab use. Understand what you're doing before shipping this. |
| `[WEB] WEBVIEW / JS` | Involves the WebView widget, HTML, or JavaScript execution inside the MA3 process. **Exposes the developer or end-user to a browser engine with file-system access.** Read the [WebView Security](wiki/WebView-Security.md) page before using any of this in a distributed plugin. |

---
# !!! UNDER DEVELOPMENT !!!
## Tested on

- **grandMA3 onPC 2.3.2**, Windows 10/11
- Hardware testing done on an i9-13900K / RTX 4080 Super rig

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

1. Copy the probe folder to `gma3_library/datapools/plugins/`
2. Import in the console: **Menu → Plugins**
3. Run: `Plugin "TaterProbe_XX"`
4. Read the System Monitor for output (`Printf` with `[probe]` tag)

Probes are non-destructive unless explicitly noted. They create nothing, delete nothing, and leave no residue.

---
# !!! UNDER DEVELOPMENT !!!
## How to contribute

Run a probe on your build. Paste the System Monitor output into an issue. Include your MA3 version and platform (onPC/console, Windows/macOS).

If you've found an undocumented function or behavior, open an issue or PR with:
- What you called
- What it returned
- What version you tested on
- A minimal code snippet that reproduces it

---
# !!! UNDER DEVELOPMENT !!!
## Who

**LXTater** — Lighting Design, Programmer, and very very tired of guessing.

---
# !!! UNDER DEVELOPMENT !!!
## Disclaimer

This is an unofficial community resource. Not affiliated with or endorsed by MA Lighting. All findings are based on reverse-engineering the publicly installed software on the developer's own machine. No proprietary source code is redistributed — only descriptions of observed behavior and original code written against the public API surface.

Use at your own risk. Don't crash the show.

# !!! UNDER DEVELOPMENT !!!
