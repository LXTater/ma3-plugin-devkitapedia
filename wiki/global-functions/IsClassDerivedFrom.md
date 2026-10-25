# IsClassDerivedFrom() [AI]
Tests whether one class derives from another. `[P]`

---

## IsClassDerivedFrom(string, string)

### "[V2.2][Manual] Definition"
```lua
IsClassDerivedFrom(string, string)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| string | string | Candidate derived class name `[P]` |
| string | string | Candidate base class name `[P]` |

### Returns
Boolean, true if the first class derives from the second. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
if IsClassDerivedFrom("Sequence", "Group") then
  Printf("derived")
else
  Printf("not derived")
end
```
- Class names here are illustrative only. `[P]`

---

## See Also
[IsObjectValid](IsObjectValid)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_isclassderivedfrom.html
