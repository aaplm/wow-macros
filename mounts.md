## Versace Violet Mounting Macro

It's a little too long (260-ish characters) in this format, but adapt it to your needs. You can specify ground mounts when no flying is available or just only specify a normal flying mount that you can use in both flying and non-flying situations.

Shoutout to [Elevenbane's](https://us.forums.blizzard.com/en/wow/t/useful-macro-templates/42937) post on the WOW forums for this one. 👏

```lua
#showtooltip
/cast [mod:alt] Mighty Caravan Brutosaur
/cast [mod:ctrl] Grand Expedition Yak
/dismount [mounted]
/stopmacro [mounted]
/run if IsUsableSpell(368896) then C_MountJournal.SummonByID(1563) end
/cast [flyable] Prestigious Bronze Courser
/cast [noflyable] Bloodgorged Crawg
 ```
 
 These are the currently available dragon riding mount IDs. Replace the `SummonByID()` argument with the one you want to use.
```lua
1589: Renewed Proto-Drake
1590: Windborne Velocidrake
1591: Cliffside Wylderdrake
1563: Highland Drake
```

This macro will:
1. dismount and/or start summoning the specified mount when holding `alt`.
2. dismount and/or start summoning the specified mount when holding `ctrl`.
3. dismount if none of the above are true and stop the macro execution.
4. mount the specified dragon riding mount if dragon riding is available.
5. mount the specified flying mount if normal flying is available.
6. mount the specified mount if dragon riding and normal flying are unavailable.
