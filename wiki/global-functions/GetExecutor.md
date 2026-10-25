# GetExecutor() [AI]
Looks up an executor by number and returns handles for it and its page. `[P]`

---

## GetExecutor(integer)

### "[V2.2][Manual] Definition"
```lua
GetExecutor(integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | Executor number `[P]` |

### Returns
Two handles: the executor and its page. `[P]`

### Example `[P]`
```lua
return function()
    local exec, page = GetExecutor(101)
    if not (exec and page) then Printf("Executor 101 not found") return end
    Dump(exec)
    Dump(page)
end
```
- Either return value can be `nil`; check both. `[P]`
- Version 2.2 per the manual. `[P]`

---

## See Also
[Printf](Printf) · [DataPool](DataPool)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual (https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getexecutor.html); not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_getexecutor.html
