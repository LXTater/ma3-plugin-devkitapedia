# NeedShowSave() [AI]
Tells whether the show file has unsaved changes. `[P]`

---

## NeedShowSave()

### "[V2.2][Manual] Definition"
```lua
NeedShowSave()
```

### Returns
true if there are unsaved changes, false if it matches the last save. `[P]`

### Example `[P]`
```lua
-- illustrative, untested
if NeedShowSave() then
  Printf("Unsaved changes")
else
  Printf("All saved")
end
```
- Playback state changes do not count. `[P]`

---

## See Also
[GetShowFileStatus](GetShowFileStatus)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual; not verified on hardware.*

Manual: https://help.malighting.com/grandMA3/2.3/HTML/lua_objectfree_needshowsave.html
