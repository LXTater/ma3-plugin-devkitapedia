# DrawPointer() [AI]
Draws a red pointer on a display; only one pointer per station exists at a time. `[P]`

---

## DrawPointer(integer, table[, integer])

### "[V2.2][Manual] Definition"
```lua
DrawPointer(integer, table[, integer])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| integer | integer | Display index. |
| table | table | Position as { x = ..., y = ... }. |
| duration | integer | Optional. Milliseconds before it fades; omitted means it stays. |

### Returns
Nothing. `[P]`

### Example `[P]`
```lua
DrawPointer(1, { x = 400, y = 300 }, 3000)
```
- A new pointer replaces the previous one for the station `[P]`.

---

## See Also
[DefaultDisplayPositions](DefaultDisplayPositions)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_drawpointer.html
