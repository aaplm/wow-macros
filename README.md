# General

### Dragon Riding/Mount Macro

```lua
    #showtooltip  
    /dismount [mounted]  
    /stopmacro [mounted]  
    /run if IsUsableSpell(368896) then C_MountJournal.SummonByID(1563) end  
    /cast [flyable] Prestigious Bronze Courser
    /cast [noflyable] Bloodgorged Crawg  
 ```
 
This macro will:
1. dismount you if you are mounted.
2. mount the specified dragon riding mount if dragon riding is available.
3. mount the specified flying mount if normal flying is available.
4. mount the specified mount if dragon riding and normal flying are unavailable.

You can remove the last `/cast` command and the `[flyable]` condition on line 5 the if you want to use your flying mount in instance where mounts cannot fly.

# Priest
### Purify/Dispell Macro

```
#showtooltip
/cast [mod:alt] !Mass Dispel; [spec:3,@mouseover,help,nodead] Purify Disease; [@mouseover,help,nodead] Purify; [@mouseover,harm,nodead] [harm] Dispel Magic; [spec:3] Purify Disease; Purify
```

This macro will:
1. cast `Mass Dispell` if used with `alt`.
2. cast `Purify` on friendly target
3. cast `Dispel Magic` on enemy target

### Shadowform

```
#showtooltip
/cast !Shadowform
```

This macro will:
1. ensure shadowform is on, even through multiple presses.
2. will not remove shadowform (you can click the buff away though).
