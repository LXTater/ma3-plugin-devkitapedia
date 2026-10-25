# AddonVars() [AI]
Gets a handle to the variable set tied to a named addon. `[P]`

---

## AddonVars(string)

### "[V2.2][Manual] Definition"
```lua
AddonVars(string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Name of the addon. |

### Returns
A handle to the addon variable set. `[P]`

### Example `[P]`
```lua
local vars = AddonVars("MyAddon")
if vars == nil then
  ErrPrintf("no variable set for that addon")
else
  vars:Dump()
end
```
- The manual notes a restriction: the addon variable set is not currently useful `[P]`.

---

## See Also
[DelVar](DelVar) · [DataPool](DataPool)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_addonvars.html
