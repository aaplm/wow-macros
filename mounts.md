## Versace Violet Mounting Macro

It's a little too long (260-ish characters) in this format, but adapt it to your needs.

```
#showtooltip
/cast [mod:alt] Mighty Caravan Brutosaur
/cast [mod:ctrl] Grand Expedition Yak
/dismount [mounted]
/stopmacro [mounted]
/run if IsUsableSpell(368896) then C_MountJournal.SummonByID(1563) end
/cast [flyable] Prestigious Bronze Courser
/cast [noflyable] Bloodgorged Crawg
 ```
 
```
1589: Renewed Proto-Drake
1590: Windborne Velocidrake
1591: Cliffside Wylderdrake
1563: Highland Drake
```

This macro will:
1. dismount you if you are mounted.
2. summon the spcified mount when holding alt
2. summon the specified dragon riding mount if dragon riding is available.
3. summon the specified flying mount if normal flying is available.
4. summon the specified mount if dragon riding and normal flying are unavailable.
