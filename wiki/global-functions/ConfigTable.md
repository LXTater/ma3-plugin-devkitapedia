# ConfigTable() [AI]
Returns an unsorted, informational table of configuration values. `[P]`

---

## ConfigTable()

### "[V2.2][Manual] Definition"
```lua
ConfigTable()
```

### Returns
A table of key-value pairs; it contains no functions. `[P]`

### Example `[P]`
```lua
for key, value in pairs(ConfigTable()) do
  Printf(tostring(key) .. " = " .. tostring(value))
end
```
- Informational only and in no particular order `[P]`.

---

## See Also
[BuildDetails](BuildDetails)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_configtable.html
