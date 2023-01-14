## Dragon Riding/Mounting

```
#showtooltip
/dismount [mounted]
/stopmacro [mounted]
/cast [mod:alt] Mighty Caravan Brutosaur
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

You can remove the last `/cast` command and the `[flyable]` condition on line 5 the if you want to use your flying mount in instance where mounts cannot fly.

## Purify/Dispell Macro

```
#showtooltip
/cast [mod:alt] !Mass Dispel; [spec:3,@mouseover,help,nodead] Purify Disease; [@mouseover,help,nodead] Purify; [@mouseover,harm,nodead] [harm] Dispel Magic; [spec:3] Purify Disease; Purify
```

This macro will:
1. cast `Mass Dispell` if used with `alt`.
2. cast `Purify` on friendly target
3. cast `Dispel Magic` on enemy target

## Shadowform

```
#showtooltip
/cast [noform] !Shadowform
/cast [@player] Power Word: Fortitude
```

This macro will:
1. ensure that you art in `Shadowform`.
2. cast `Power Word: Fortitude` if you're already in `Shadowform`.

## Targeting

```
#showtooltip
/cast [@mouseover,harm,nodead][@focus,harm,nodead,exsists][] Shadow Word: Pain
```

This macro will:
1. cast the spell at your mouseover target.
2. cast the spell at your focus target, if none of the above
3. cast the spell at your selected target, if none of the above
