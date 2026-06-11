# LXTater's MA3 Plugin Devkitapedia
Unofficial devkit and wiki for **grandMA3 plugin development**. This wiki is **Under Development**

MA3's Lua plugin API is powerful but not entirley documented. I have been so tired of scrounging Google's third or fourth page to see if someone has the right keyword. My CTRL + F keys have worn completely out. This is still being built. Althoug it is planned to be a wiki that goes through updates, I plan on keeping the under development label until all of the MA3 Global Functions that MA has examples on the manual are created into wiki pages.

---

## What's in here

**Wiki** - Still Trying to build everything out.

**Probes** : Test plugins meant to build on one another. For example, Probe 1: Dumps Sequences, Probe 2: takes info from probe 1, tries to change a setting from the sequence dump, Probe 3: Find and dump children of Sequecnes. Etc etc.

**Dev Tools** : development tools for testing, parsing, scraping, pulling, grubbing, etc. These are not official dev tools. These can be plugins, external plugins, or online tools that help with development and testing.

---

## Trust tiers

Everything should include one of these tags

| Badge | Meaning |
|-------|---------|
| `[Vx.x.x][y] VERIFIED` | Tested on hardware, log output confirmed. Build on this. x.x = MA3 Big Version (2.4.2). [y] can be pulled from the next entry below. |
| `[HW]` | Verified on offical MA3 Hardware with a built-in os (command wing xt is acceptable here.) . [HW], any MA3 hardware with built-in OS (Console, command wing XT, etc.);|
| `[onPC.X]`| [onPC], standalone onPC with no MA hardware in session; [onPC.X] VK/CW/DMX/Other(viz-key, command wing, DMX-Key, Other = onPC with PU, node, etc in the network) | 
| `[Mac/Windows]` | If using onPC, add a Mac or windows tag next to it. |
| `[P] PROVISIONAL` | Reasoned from MA source or partial testing. Probably right, verify before depending on it. |
| `[?] UNKNOWN` | Pulled from an API dump, or similar. Needs a probe/testing. |

If an entry doesn't have a badge, treat it as `PROVISIONAL`.

---
## Boundary markers

If we are stretching the abilities of the LUA sandbox, or there's a less-than-normal method to do something, please include one of these tags:
| Marker | Meaning |
|--------|---------|
| `[UND] UNDOCUMENTED` | Uses real API surfaces that MA hasn't publicly documented. Works, but not fully understood. |
| `[SBX] SANDBOX` | 	Pushes against sandbox boundaries (editing `lib_menus`, injecting files into anywhere besides the datapool/gma3_library folders (colorthemes,media, etc) Understand that this should never go on a lighting console without extreme testing, as it can potentially lead you to reinstalling MA. |
| `[AI] AI Involvement` |  If a certain task, plugin, etc has been created entirely by AI, or if generative AI was utilized, it should have this tag.  |

---
## Template for hardware/software noting for Verified tags:

**OnPC**
**Software/Hardware/OS:**
- OnPC Version:
- MA Hardware in Session:
- Other onPC hardware in Session:
- OS and version:
- CPU, GPU, and RAM:
- GPU Driver Version:

  
**MA Hardware**
- MA Version:
- MA Hardware in Session
- OnPC hardware in Session:
- if applicable, Relevant OnPC info:


---
## Who

**LXTater** — Lighting Design, Programmer, and very very tired of guessing.

---
---
## AI Declreation

AI has been utilized in this project. For the sake of transparency, a [AI] label will be added to anything that generative AI was used for.
The current use of AI in this project has been limited to: Data Parsing (Scanning through MA UI Files/Backend), and with help organizing and creating the MDs for this wiki.

---
## Disclaimer
This is an unofficial community resource. Not affiliated with or endorsed by MA Lighting.
 
Use at your own risk. Don't crash the show ;-)
