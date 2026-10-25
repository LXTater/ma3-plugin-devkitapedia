# DataPool() [AI]
Returns a handle to the currently selected DataPool for reading or editing its properties. `[P]`

---

## DataPool()

### "[V2.2][Manual] Definition"
```lua
DataPool()
```

### Returns
A handle to the DataPool object. `[P]`

### Example `[P]`
```lua
local pool = DataPool()
pool:Dump()
Printf("First sequence: " .. tostring(pool.Sequences[1].Name))
```
- Assumes at least one sequence exists in the pool `[P]`.

---

## In the Wild: Finding a macro slot `[onPC]`
```lua
local m = DataPool().Macros:Ptr(901)
for _, o in ipairs(DataPool().Macros:Children()) do
  if o then used[o.name] = true end
end
```
`Ptr` returns nil for an empty slot, and `Children` is iterated to collect existing names. `[P]`

*Excerpt from the Steamboat Willie Player plugin, CC BY 4.0, Badass Lighting Tools. [Source](https://github.com/badasslighting/R-D-Lab/tree/main/MA3-Scribble-Animator/releases/steamboat-willie).*

See [Steamboat Willie Player](Steamboat-Willie-Player).

---

## See Also
[CurrentExecPage](CurrentExecPage) · [CurrentUser](CurrentUser)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_datapool.html
