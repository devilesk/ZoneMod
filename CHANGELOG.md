## RL4D2L Changelog

### Map Changes

* **Blood Harvest**
  * Map 3
    * Horde increased from 90 to 120. Fixes infinite hordes for sizes below 120.
  * Map 4
    * Horde increased from 60 to 120. Fixes infinite hordes for sizes below 120.

* **Dead Center**
  * Map 1
    * Added extra tier 1 weapons to saferoom.

* **Death Toll**
  * Map 1
    * Added a bus to the saferoom. [Backport from ZoneMod 1.9.4.](https://hackmd.io/UtNSO9d1R-yCIdb2ifa6ug)

* **No Mercy**
  * Map 1
    * Added tank ban range to prevent early tank spawns.
  * Map 4
    * Added tank ban range to prevent elevator tank spawns.

* **The Parish**
  * Map 4
    * Removed tank ban range to allow for later tank spawns.

### Gameplay / Balance Changes

* Points are frozen while tank is alive on finales.
* Removed first tank from all finales except Dead Center and Swamp Fever. All other finales only have one tank now.

### Bug / Exploit Fixes

* Fixed tank ban ranges not being properly applied.
* Fixed tank damage announcement message showing incorrect survivor damage percentages.

### Miscellaneous

* Increased allowed lerp changes from 3 to 10.
* Stat tracking plugins
  * player_skill_stats.smx
  * l4d2_playstats.smx
* Round results posted to discord
  * discord_webhook.smx
  * discord_scoreboard.smx
* Commands for teleporting stuck tanks
  * teleport_tank.smx
* Commands for spawning axes and pistols
  * spawn_secondary.smx
* Finale fixes
  * swamp_finale_fix.smx
  * suicideblitzfinalefix.smx

[rl4d2l-plugins repository](https://github.com/devilesk/rl4d2l-plugins)