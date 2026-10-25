# Confirm() [AI]
Shows a simple OK/Cancel confirmation pop-up and returns the choice. `[P]`

---

## Confirm(title, [text], [integer], [boolean])

### "[V2.2][Manual] Definition"
```lua
Confirm(title, [text], [integer], [boolean])
```

### Parameters
| Field | Type | Use |
|-------|------|-----|
| title | string | Heading of the pop-up. |
| text | string | Optional. Message body. |
| integer | integer | Optional, ignored (pop-up shows on all screens); may be nil. |
| boolean | boolean | Optional, default true. false hides Cancel and shows only OK. |

### Returns
true (or 1) for OK, false (or 0) for Cancel. `[P]`

### Example `[P]`
```lua
if Confirm("Reset?", "Clear the programmer now?") then
  Printf("User accepted")
else
  Printf("User cancelled")
end
```
- Cancel can only be returned when the Cancel button is shown `[P]`.

---

## See Also
[CloseAllOverlays](CloseAllOverlays) · [Echo](Echo)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_confirm.html
