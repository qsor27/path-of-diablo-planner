## Planner for Character Builds in Path of Diablo

### Getting started with Planner editing
Quick tour of the files within thie project: https://youtu.be/0GXcUw0btrA

### Features:
* all skill info up to level 60 & synergy calculations
* charm inventory
* saving/loading, URL-sharing
* equipment selection & modification (corrupting, socketing, upgrading)
* skill damage calculation
* all character stats
* mercenary selection
* snapshotting for buffs

### Controls:
* Click on the character's level or class to change them
* Use right click to remove points or items
* Shift and ctrl modify the amount added or removed (also works on items in the charm inventory)
* Corruptions may be selected via the narrow dropdowns to the left of each item dropdown
* Upgrading can be done by ctrl-clicking the equipped item (ctrl + right-click to downgrade)
* Snapshot effects by ctrl-clicking the effect's icon
* Add jewels/runes/gems to items by dragging them from the inventory to an equipment slot that has open sockets

#### Mobile Users:
If your phone doesn't have a way to emulate ctrl+click or shift+click, you can still use the URL to enter any character info. Toggle *Shareable URL* in the menu to see how it should be formatted. Example:

https://build.pathofdiablo.com/?v=2&class=sorceress&level=99&quests=1&strength=45&vitality=460

### Known Issues:
* Some spells that deal magic damage (ex: FoH, Bone Spear) are not affected by magic facets or charms; attacks (like Dashing Strike) do display properly
* Displayed damage is incorrect for skills that care about on vs off weapon ED, added minus ED
charms to compensate
* Barb combat skills remain "red" even when prerequisites are met
* "+1 (each) skills" charm isn't applied to some skills
* Charms can't be moved into a new space below the original space if those spaces overlap
* Shift + Right Click in Firefox doesn't work (and still opens the default menu)
* Socketed gems/runes/jewels sometimes aren't aligned like they should be
* Snapshotted skills may not load correctly with saved files or shared URLs
* DoT (Damage over Time) stats are added without considering their time component
* Dual-Wielding damage may be incorrect (some on-weapon damage affixes affect both weapons)
* Minion damage may be incorrect (some bonuses from auras/items aren't included)

### Notes:
* Chance to Hit (displayed after Attack Rating) is an approximation for typical enemies at the character's level - it won't be accurate for bosses or monsters at much higher/lower levels
* Effective Magic Find (displayed after Magic Find) shows how much is applied to uniques

### Future Ideas:
* party tracking (i.e. buffs from party members)
    * Some party buff effects available via "charms" 
* Add calculated damage values for CtC (chance to cast) skills in a consistent manner
* mercenary stats
* total calculated damage for minions
* IAS breakpoint info (frames per attack) for skills which don't use normal breakpoints
* breakdown of attack damage by type
* skill effectiveness (dps, area affected, movement capability)
* full GUI inventory/stash
* custom item creation & affix editing
* custom item-pool saving
* options for individual quests
* option for strict character validation (prevent invalid character states instead of just making text red)
* character importing
* monster stat calculations
* debuff tracking
* pvp info
* dynamic item/skill recommendations

### Contribute:

#### Updating Incorrect/Outdated Skill Data:

The planner automatically pulls the information from our wiki. All PoD players with a trade account have a wiki account automatically. Log in to our wiki using the same login info as trade account and edit the skill data in the following pages:

* [Amazon.js](https://pathofdiablo.com/wiki/index.php?title=Amazon.js)
* [Barbarian.js](https://pathofdiablo.com/wiki/index.php?title=Barbarian.js)
* [Assassin.js](https://pathofdiablo.com/wiki/index.php?title=Assassin.js)
* [Druid.js](https://pathofdiablo.com/wiki/index.php?title=Druid.js)
* [Necromancer.js](https://pathofdiablo.com/wiki/index.php?title=Necromancer.js)
* [Paladin.js](https://pathofdiablo.com/wiki/index.php?title=Paladin.js)
* [Sorceress.js](https://pathofdiablo.com/wiki/index.php?title=Sorceress.js)
* [Universalskills.js](https://pathofdiablo.com/wiki/index.php?title=Universalskills.js)

#### Improvements to the underlying code:
This planner is open-source, so improvements can be contributed by anyone through github. Here are the basic steps:
* Create a [fork](https://github.com/GreenDude120/path-of-diablo-planner/fork) (duplicate) of this repository
* Edit the files
* Submit a pull request (i.e. request your changes be pulled into this version)

### Credits:

Originally created by BetweenWalls, the planner was forked to allow the PoD team & community to edit and update the planner in a timely fashion and without depending on a single user.
