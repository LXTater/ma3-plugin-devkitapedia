# Macro Object References [AI]
Since the 2.0 line, command lines and macro lines can refer to objects by a handle reference instead of a plain pool number. `[P]`

---

## Plain vs. referenced `[P]`

| Style | Example | Behaviour |
|-------|---------|-----------|
| Plain | `Go Sequence 5` | Breaks if the sequence is moved or renumbered |
| Referenced | `Go #[Sequence 5]` | Tracks the object when it is moved or renamed |

### Notes

1. The reference form is written `#[...]` around the object's address.
2. The macro editor can convert existing plain lines to references. The exact button and syntax need a probe, so treat the conversion as `[?]`.
3. When generating command strings from Lua, prefer the referenced form for anything that must survive a show reorganisation.

---

## Open questions `[?]`

- Does `#[...]` resolve inside `gma.cmd` strings the same way as in macro lines?
- How are references stored when a library is exported and re-imported?

---

## See Also
[Command Syntax Basics](Command-Syntax-Basics)

*Generated with Claude Sonnet 5.5 with Medium effort. Not verified on hardware.*
