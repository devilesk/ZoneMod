## RL4D2L Changelog

### Map Changes

* **Blood Harvest**
  * Map 1
    * Fixed broken model used to prevent SI from getting stuck in ditch.
  * Map 2
    * Removed clipbrushes from emergency door and moved emergency sign up a bit so SI don't have to crouch to get through the door.
  * Map 3
    * Horde increased from 90 to 120. Fixes infinite hordes for sizes below 120.
  * Map 4
    * Horde increased from 60 to 120. Fixes infinite hordes for sizes below 120.
    * Added easier way for SI to get on top of the saferoom.
  * Map 5
    * Fixed out of map exploits. Taken from [L4D2-Competitive-Rework](https://github.com/SirPlease/L4D2-Competitive-Rework)

* **Dead Air**
  * Map 1
    * Blocked access to upper rails and upper roof sections of saferoom greenhouse.
  * Map 5
    * Removed intro plane crash sound and shake. Taken from [NextMod](https://github.com/spoon-l4d2/NextMod)

* **Dead Center**
  * Map 1
    * Added extra tier 1 weapons to saferoom.

* **Death Toll**
  * Map 1
    * Added a bus to the saferoom. [Backport from ZoneMod 1.9.4.](https://hackmd.io/UtNSO9d1R-yCIdb2ifa6ug)
  * Map 4
    * Added an infected climb point at the back of the road where people commonly take the event.
    * Fixed pipe bomb potentially spawning outside the saferoom at the end of the level.

* **Diescraper Redux**
  * All Maps
    * Fixed map names in mapinfo and saferoominfo not matching v3.61 map names.
  * Map 2
    * Removed potential medkit spawn.
  * Map 4
    * Fixed potential double shotgun saferoom spawn.

* **Hard Rain: Downpour**
  * Map 5
    * Replaced alarm car with normal car because it would cause early tank spawns.

* **No Mercy**
  * Map 1
    * Added tank ban range to prevent early tank spawns.
  * Map 3
    * Warehouse door can now be shot through.
  * Map 4
    * Added tank ban range to prevent elevator tank spawns.

* **Suicide Blitz 2**
  * Map 1
    * Prevented button room from being accessible before round is live.
    * Removed button room zombie trigger and made the button trigger horde instead.
  * Map 5
    * Shortened intro by allowing radio button to be pressed a second time earlier.
    
* **Swamp Fever**
  * Map 1
    * Added one-way drop after leaving gas station to prevent survivors from returning to spawn. [Inspired by ZoneMod 1.9.4.](https://hackmd.io/UtNSO9d1R-yCIdb2ifa6ug)

* **The Parish**
  * Map 4
    * Removed tank ban range to allow for later tank spawns.
    
* **The Sacrifice**
  * Map 3
    * Fixed pipe bombs spawning instead of pills.

### Gameplay / Balance Changes

* Points are frozen while tank is alive on finales.
* Removed first tank from all finales except Dead Center and Swamp Fever. All other finales only have one tank now.
* Enabled world sounds
* Added a static tank player order plugin for league matches where tank players are determined ahead of time.

### Bug / Exploit Fixes

* Fixed tank ban ranges not being properly applied.
* Fixed tank damage announcement message showing incorrect survivor damage percentages.
* Fixed error log messages due to unused and improper cvar settings.
* Fixed Blood Harvest Stripper:Source configs not loading if lowercase map name was used to switch to maps, i.e. `!map c12m1_hilltop` instead of `!map C12m1_hilltop`.
* Fixed syntax error in Dark Carnival map 2 Stripper:Source config.
* Fixed syntax error in No Mercy map 2 Stripper:Source config.
* Fixed readyup plugin changing unbreakable doors to breakable.

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
* Added commands
  * `!tankpool` - Displays list of possible tank players
  * `!queuetank` - Adds player to list of possible tanks
  * `!dequeuetank` - Removes player to list of possible tanks
  * `!restartmap` - Restarts map and keeps current scores. Automatically restarts map when broken flow detected.

[rl4d2l-plugins repository](https://github.com/devilesk/rl4d2l-plugins)