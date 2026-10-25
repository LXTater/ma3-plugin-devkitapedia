# HostType() [AI]
Names the type of the host device. `[P]`

---

## HostType()

### "[V2.2][Manual] Definition"
```lua
HostType()
```

### Returns
One string such as Console or onPC. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
if HostType() == "onPC" then
  Printf("onPC session")
end
```
- Takes no arguments. `[P]`

---

## See Also
[HostSubType](HostSubType) · [HostOS](HostOS)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_hosttype.html
