# Pult() [AI]
Gives you a handle to the Pult object, which keeps display and device information (found under Root/GraphicsRoot/PultCollect). `[P]`

---

## Pult()

### "[V2.2][Manual] Definition"
```lua
Pult()
```

### Returns
A handle to the pult object. `[P]`

### Example `[P]`
```lua
local obj = Pult()
if obj then
  Printf("--- Pult ---")
  obj:Dump()
else
  Printf("Pult: nothing returned")
end
```
- Takes no arguments. `[P]`
- The manual places the object at Root/GraphicsRoot/PultCollect. `[P]`

---

## See Also
[Root](Root) · [ShowData](ShowData)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_pult.html
