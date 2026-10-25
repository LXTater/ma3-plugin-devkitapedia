# ProgrammerPart() [AI]
Gives you a handle to the programmer part object currently in use. `[P]`

---

## ProgrammerPart()

### "[V2.2][Manual] Definition"
```lua
ProgrammerPart()
```

### Returns
A handle to the programmer part object. `[P]`

### Example `[P]`
```lua
local obj = ProgrammerPart()
if obj then
  Printf("--- ProgrammerPart ---")
  obj:Dump()
else
  Printf("ProgrammerPart: nothing returned")
end
```
- Takes no arguments. `[P]`
- Dump() prints the object's properties and children, which is a quick way to explore it. `[P]`

---

## See Also
[Selection](Selection) · [Root](Root)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_programmerpart.html
