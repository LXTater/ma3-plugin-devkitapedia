# GetSubfixture() [AI]
Looks up a fixture by its patch index and returns its handle. `[P]`

---

## GetSubfixture(integer)

### "[V2.2][Manual] Definition"
```lua
GetSubfixture(integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | Patch index (subfixture index) of the fixture `[P]` |

### Returns
A handle to the matching fixture object. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
local fix = GetSubfixture(1)
if fix then
  Printf("Fixture 1 name: " .. tostring(fix.name))
end
```
- The index is the patch index, not the fixture ID `[?]`.

---

## See Also
[GetSubfixtureCount](GetSubfixtureCount) · [GetUIChannels](GetUIChannels)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getsubfixture.html
