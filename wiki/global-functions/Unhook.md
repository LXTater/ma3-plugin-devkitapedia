# Unhook() [AI]
Removes a single hook, using the integer ID given when the hook was created. `[P]`

---

## Unhook(integer)

### "[V2.2][Manual] Definition"
```lua
Unhook(integer)
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | Integer | ID of the hook to remove. `[P]` |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
-- hookId was returned earlier by HookObjectChange
Unhook(hookId)
```
- DumpAllHooks does not show IDs; if you lost the ID, use UnhookMultiple. `[P]`
- Hooks are created with HookObjectChange. `[P]`

---

## See Also
[UnhookMultiple](UnhookMultiple) · [HookObjectChange](HookObjectChange) · [DumpAllHooks](DumpAllHooks)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_unhook.html
