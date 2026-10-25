# Root() [AI]
Gives you a handle to the object at the very top of the object tree. `[P]`

---

## Root()

### "[V2.2][Manual] Definition"
```lua
Root()
```

### Returns
A handle to the Root object. `[P]`

### Example `[P]`
```lua
local obj = Root()
if obj then
  Printf("--- Root ---")
  obj:Dump()
else
  Printf("Root: nothing returned")
end
```
- Takes no arguments. `[P]`
- Dump() lists name, class, path, properties and children of the object. `[P]`

---

## See Also
[ShowData](ShowData) · [Pult](Pult)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_root.html
