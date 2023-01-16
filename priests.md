## Mass Dispell, Purify, and Dispell, Oh My!

This is a handy macro that will use your spec's version of `Purify` and `Dispel Magic` on friendly and enemy targets, respectively. This one macro will change the spells used depending on the spec you are in. 💯💯

Shoutout to [Elevenbane's](https://us.forums.blizzard.com/en/wow/t/useful-macro-templates/42937) post on the WOW forums for this one.

```lua
#showtooltip
/cast [mod:alt] !Mass Dispel; [spec:3,@mouseover,help,nodead] Purify Disease; [@mouseover,help,nodead] Purify; [@mouseover,harm,nodead] [harm] Dispel Magic; [spec:3] Purify Disease; Purify
```

This macro will:
1. cast `Mass Dispell` if `alt` is held
2. cast `Purify` on friendly target
3. cast `Dispel Magic` on enemy target

## Suspect Shadowform and Fortitude

This macro will also work in all `Priest` specs.

```lua
#showtooltip
/cast [spec:3,noform] !Shadowform
/cast [@player] Power Word: Fortitude
```

This macro will:
1. Enter `Shadowform` if it's not on and you're playing shadow.
2. Cast `Power Word: Fortitude` on yourself.