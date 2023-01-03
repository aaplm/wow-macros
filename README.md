# General

### Dragon Riding/Mount Macro

This macro will:  
1. Dismount you if you are mounted  
2. Mount the specified dargon riding mount  
3. If dragon riding is unavailble and you can fly, mount the specified flying mount  
4. If dragon riding and normal flying are unavailble, mount the specified ground mount  

```lua
    #showtooltip  
    /dismount [mounted]  
    /stopmacro [mounted]  
    /run if IsUsableSpell(368896) then C_MountJournal.SummonByID(1563) end  
    /cast [flyable] Prestigious Bronze Courser
    /cast [noflyable] Bloodgorged Crawg  
 ```
 
# Priest
### Purify/Dispell Macro

    #showtooltip
    /cast [mod:alt] !Mass Dispel; [spec:3,@mouseover,help,nodead] Purify Disease; [@mouseover,help,nodead] Purify; [@mouseover,harm,nodead] [harm] Dispel Magic; [spec:3] Purify Disease; Purify
