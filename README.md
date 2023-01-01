### Mount Macros

    #showtooltip  
    /run if IsUsableSpell(368896) then C_MountJournal.SummonByID(1563) end  
    /cast [flyable,nomounted] Prestigious Bronze Courser
    /cast [noflyable,nomounted] Bloodgorged Crawg  
    /dismount [mounted]  

### Priest Purify/Dispells

    #showtooltip
    /cast [mod:alt] !Mass Dispel; [spec:3,@mouseover,help,nodead] Purify Disease; [@mouseover,help,nodead] Purify; [@mouseover,harm,nodead] [harm] Dispel Magic; [spec:3] Purify Disease; Purify
