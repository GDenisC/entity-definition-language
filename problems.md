# flags definition for now:
kinda bad
```
effects = damage, rate, motion
draw = self, border, fill
flags = acceptsScore, healthWithLevel, canBeOnLeaderboard
// disabled: independent, hasNoMaster, isImmuneToTiles, intangible, giveKillMessage, canGoOutsideRoom, dieAtLowSpeed, dieAtLowRange, clearOnMasterUpgrade, persistsAfterDeath, variesInSide, hasNoRecoil, syncWithTank, buffVsFood, obstacle, cravesAttention, necro
```

# loops
they're just bad.
```
for (a in 0..360 step 360 / 8)
    guns += mothership1 + gun { angle += a },
            mothership2 + gun { angle += a }
```