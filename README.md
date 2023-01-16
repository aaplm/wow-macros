# wow-macros

Welcome to my collection of macros that I use or found interesting.

[Arena Macros](arenas.md)
[Mount Macros](mounts.md)  
[Priest Macros](priests.md)  

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
/cast [@mouseover,harm,nodead] [@focus,harm,nodead,exists] [] Shadow Word: Pain
```

This macro will:
1. cast the spell at your mouseover target.
2. cast the spell at your focus target, if none of the above
3. cast the spell at your selected target, if none of the above

## Arenas

```
#showtooltip
/cast [@arena1,nodead,exists] [@mouseover,harm,nodead] [@focus,harm,nodead,exists] [] Shadow Word: Pain
```
```
#showtooltip
/cast [@arena2,nodead,exists] Shadow Word: Pain
```
```
#showtooltip
/cast [@arena3,nodead,exists] Shadow Word: Pain
```
