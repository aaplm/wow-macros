# wow-macros

Welcome to my collection of macros that I use or found interesting.  
Use the links to naviagte to whichever pages you're interested in.

## Arenas

The classic target arena players 1, 2, and 3.

```
#showtooltip
/cast [@arena1,nodead] [@mouseover,harm,nodead] [@focus,harm,nodead,exists] [] Shadow Word: Pain
```

```
#showtooltip
/cast [@arena2,nodead] Shadow Word: Pain
```

```
#showtooltip
/cast [@arena3,nodead] Shadow Word: Pain
```

## Mounts

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

## Priest

### Fortitude and Shadowform

This macro will also work in all `Priest` specs.

```lua
#showtooltip
/cast [spec:3,noform] !Shadowform
/cast [mod:shift,@Mouseover,help] Resurrection; [mod:shift] Mass Resurrection
/cast [@player] Power Word: Fortitude
```

This macro will:
1. Enter `Shadowform` if it's not on and you're playing shadow.
2. Cast Mass Resurection if
2. Cast `Power Word: Fortitude` on yourself.

### Dark Ascension vs Void Eruption

```lua
#showtooltip
/cast [@mouseover, known: Dark Ascension] [known:Dark Ascension] Dark Ascension; [@mouseover, known: Void Eruption] [known:Void Eruption] Void Eruption
```

This macro will:
1. cast `Dark Ascension` if talented; or
2. cast `Void Eruption` if talented


## Stop Mind Searing Friends

```lua
#showtooltip
/cast [@mouseover, harm, nodead] [harm, nodead] Mind Sear
```
