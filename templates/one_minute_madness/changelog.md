[<<-home](../..)  
[<<-back](index.html)

## One Minute Madness - Changelog

### Version 0.6

[Download](./One%20Minute%20Madness%200.6.zip)

#### General settings

* Artifacts:
    * Banned the Necklace of Swiftness. This is hands down the best Treasure class artifact in the game, with the ability to trivialize some fights. Additionally, in combination with other +speed artifacts, this provides a game-warping advantage to a player, nearly winning the game on the spot.
    * Banned Charm of Mana and Talisman of Mana. The effect of these two artifacts is weak, and banning them has an additional effect of preventing the assembly of Wizard's Well.
    * Banned Endless Sack of Gold, Endless Bag of Gold and Endless Purse of Gold. These three artifacts are cluttering the pool of Major class artifacts, while being an unappealing objective to go for. While they can provide an advantage in case of a long game, they don't provide a power boost the Major class artifacts are supposed to do.
    * Banned Ring of Vitality. The +hp effect is actually a strong effect on this template, due to the size and scaling of tier 1 and tier 2 powerstacks - a bit strong for a Treasure class artifacts. In itself it would be fine though, but the possibility of assembling a game-warping Elixir of Life forces a ban on at least one of its elements.
    * Banned Rib Cage. The sole purpose of this ban is to prevent the possibility of assembling Armor of the Damned.
* Objects:
    * Banned Refugee Camps from spawning. They were the only additional army-giving object that I have missed. While these don't really provide that big of an advantage most of the time, they are still able to provide a player with an extra Archangel or Black Dragon, which is massive boost for relatively low opportunity cost. There is also an issue with their RNG state not being preserved through saves. If a crash happens during 121, and the save from 117 has to be loaded, on the next week the unit in the camp will be different.
    * Banned Warrior's Tombs. They are objects with an extremely random effect, sometimes even resulting in a relic artifact drop.
* Spells:
    * Fixed the lack of ban on the Disguise spell.
    * Banned the spells Destroy Undead, Hypnotize, Mirth and Misfortune. Most of the Tier 3 spells are extremely weak and/or situational, but they also house important to the metagame Antimagic and Protection From Earth. This change should also help out the Fortress and Stronghold, which are limited to the Tier 3 guild.
* Heroes:
    * Banned Straker, Ulfretin and Piquedram. These three heroes, if they will show up as the second hero, put the player at a massive disadvantage, effectively punishing player for being unlucky.
* Adjusted the Zones Sparseness setting again in hopes to improve the zone placement.
* Slightly reworded the template description.

#### Zone connections
* The connections leading from the starting zone (5-9, 6-9, 7-10, 8-10) have their value reduced to 2000.

#### Zones 1 and 2

* Modified the treasure values to (3000-6000, 8), (10000-15000, 8), (15000-20000, 3). It is just a simple minor adjustment to improve the quality of this zone's generation.
* Removed Windmills and Warehouses of any kind from this zone. They were a close to being just an interactive obstacle in this zone.
* Increased the frequency of the Major class artifacts to 800, while decreasing the frequency of the Minor artifacts of 250. Major class artifacts were a little bit too rare, and this change is set to improve this.
* Banned Wood and Ore from spawning in this zone, while reducing the frequency of each magical resource and Gold to 50. Additionally, the frequency of Campfires was reduced to 75. In exchange, the frequency of Treasure Chests was increased to 1500. The extra resources were cluttering the treasure zones effectively reducing the amount of interesting objectives.
* Increased the frequency of Treasure Chests to 1500. While it is close to being "just another resource", the amount of gold given by this is noticeable - and it can be exchanged into XP. As such, it is an interesting objective to aim for when going through the desert.

#### Zones 6 and 8

Most of the changes in this zone are designed towards differentiating it from the grass zone. After this update, the wasteland zone will be far more focused on stats and XP, while having a significiantly reduced amount of resources.
* Disabled Windmills, Prospectors, and Warehouses of any kind in this zone.
* Increased the frequency of the School of Wars to 500, and increased its value to 1500.
* Increased the frequency of Schools of Magic to 300, and increased their value to 1500.
* Increased the amount of 5000 XP Pandora's Boxes to 2.
* Reduced the frequency of all resources to 40, and the Random Resource object to 100.
* Learning stones, Mercenary Camps, Marletto Towers, Star Axes and Gardens of Revelation have all their frequency increased to 700 each.
* Increased the frequency of Minor class artifacts to 400, and the Treasure class artifacts to 275.
* Because of the previous restrictions causing the RMG to suddenly overdo on the shrines and scrolls, the amount of Spell Scrolls and Shrines spawning in this zone is limited to the following:
    * Level 1 scrolls: 3
    * Level 2 scrolls: 2
    * Level 3 scrolls: 1
    * Level 1 shrines: 3
    * Level 2 shrines: 3
    * Level 3 shrines: 2
    * Other levels of both scrolls and shrines are not limited.

#### Zones 5 and 7

* Slightly bumped the treasure values to (1500-3000, 15), (3000-6000, 11), (6000-12000, 4) to slightly increase amount of resources spawned.
* Bumped up the zone's size setting to 17 in an attempt to improve the quality of generation.
* Removed Taverns. Their object value was too low to even spawn with any consistency, and even then - they would be difficult to utilize meaningfully in one minute timers.
* Increased the object value of Stables to 1000. The default value of 200 was far too low for this to spawn consistently under this zone's treasure values.
* Reduced the amount of 5000 XP Pandora's Boxes to 1. This is to keep the status quo with the amount of experience on the map after the wasteland got an extra box.
* Increased the frequency of Water Wheels to 150, and their value to 1000. This is done to provide more long-term income options.

#### Rule and text changes

* Made the 1+1+3 timer the default, and reflected this in the template description.

### Version 0.5

This release marks the start of the Beta stage of template development.

[Download](./One%20Minute%20Madness%200.5.zip)

#### General settings

* Rearranged the zones and modified the Zones Sparseness settings for higher minimal quality of generations.
* Banned Relic class artifacts from spawning. While it was almost impossible for them to spawn, there was an extremely low chance of this happening anyway. While Relics may be incorporated in a future version of the template, they currently can provide an undeserved victory by providing one of the players with an extremely powerful artifact.
* Banned War Machine Factories and Cannon Yards from spawning. They were uninteresting an expensive option, effectively turning them into an interactive obstacle.
* Updated the template description.

#### Other

* Cleaned up the redundant object rules from zones.

### Version 0.4

[Download](./One%20Minute%20Madness%200.4.zip)

#### Zone connections

* Raised the value of certain zone connections.
    * Zones 1-7, 2-5 (between grass to enemy treasure): 12000
    * Zones 1-2 (between both treasures): 9000
    * Rationale: The connections between both halves of the map were undervalued - especially the shortcut connection between grass and the enemy treasure zone. This made red rush far too appealing, while also causing the games to end unsatisfactorily early. Additionally, the low difference between the connection values often made discerning between the connection types impossible. 
* Fixed the lack of Portal Repulsion between zones 2 and 5.

#### Zones 1 and 2

* Increased the treasure values to (3000-6000, 9), (10000-15000, 6), (15000-20000, 2). It is just an attempt to provide a tiny bit more consistency.
* Removed Cyclops Stockpiles. The resources granted by this creature bank aren't really a good reward on this template for the difficulty it poses, effectively making this bank worthless.

#### Zones 5 and 7

* Removed Naga Banks. Reasoning is exactly the same as for the Cyclops Stockpiles removal listed above.

#### Zones 6 and 8

* Removed Medusa Stores. Reasoning is again the same as above.
* Capped the amount of Windmills on this zone to 4. This is set to prevent RMG literally spamming windmills all across the zone on certain rolls, while also not removing them completely.

#### General settings

* Disabled Hill Forts. They had a very minor chance to spawn, and when they did they gave a major advantage to one of the players. They may be reintroduced later on in a more controlled manner.

#### Artifacts

* Banned the following artifacts:
    * Pendant of Dispassion, Pendant of Second Sight, Pendant of Holiness, Pendant of Life, Pendant of Death, Pendant of Free Will, Sphere of Permamence - most of these are far too situational to ever matter in the gameplay. Being protected from one rarely used spell in FB is far too underwhelming. Out of these artifacts, only the Pendant of Second Sight might be reasonably used - but in practice, Blind is not threatening enough to warrant the existence of this artifact.
    * Everflowing Crystal Cloak, Ring of Infinite Gems, Everpouring Vial of Mercury, Inexhaustible Cart of Ore, Eversmoking Ring of Sulfur, Inexhaustible Cart of Lumber - there is more than enough of resources that can be found on the ground. All these artifacts are serving just as a clutter.
    * Orb of the Firmament, Orb of Silt, Orb of Tempestuous Fire - the damage from spells isn't often the game-winning factor, and in the rare cases where it is, these orbs provide an unjust advantage that is hard to counter.
    * Bow of Elven Cherrywood, Bowstring of the Unicorn's Mane, Angel Feather Arrows - the archery bonus granted by these artifacts is ridicolously inconsequential. While they could be fine if they all were Treasure class artifacts, they are not - the Bowstring is Minor class, while the Arrows are Major class.

#### Minor Text Changes
* Updated the description to reflect the changes in road and timer recommendations.

### Version 0.3

[Download](./One%20Minute%20Madness%200.3.zip)

#### Zones 6 and 8

* Fixed the issue of Derricks not actually being disabled.
* Removed the Town Gate. While this object was placed to allow for higher mobility and far easier supply chains, it was not fulfilling this role properly.
* Changed the treasure values to (2500-3500, 9), (3000-5000, 16), (8000-12000, 4). After the removal of Town Gate, this zone was made barren and uninteresting. This is a temporary measure to offset this change.
* School of War and School of Magic both have their frequency increased to 200.

#### Zones 9 and 10

* Added the Town Gate to this zone.

#### Zones 1 and 2

* Mansions are completely removed - they were risky an unappealing choice, effectively making them more of a guarded obstacle instead of a point of interest they were meant to be.
* Added three 3 Churchyards with their object value increased to 2500. They are simple, consistent creature banks that are a good source of experience and artifacts - and as such they are an interesting addition to the desert. They perfectly fill the niche that Mansions were supposed to fill.
* Increased the frequency of both Minor and Major class artifacts to 400. They were simply not spawning enough.
* Added 2 Town Gates to this zone. They provide the much needed mobility to the starting town. They are also guarded, meaning you have to deliberately fight for access to this option.

### Version 0.2

[Download](./One%20Minute%20Madness%200.2.zip)

#### General

* Adjusted the values of Rock Block Radius and Zone Sparseness parameters.

#### Zones 6 and 8

* The value of Town Gate has been reduced to 4000 from the default value of 10000. The value of the Imp Cache was also reduced to 2500 from the default value of 5000. Both changes are introduced to increase the consistency of both objects spawning without massively increasing the amount of treasure, and as such the strength of guards on this zone.  
* Disabled the Trailblazer and Derrick in this zone. The Trailblazer wasn't a very interesting addition and made it harder for the RMG to fit all other objects that should spawn, while the Derricks were overwhelmingly common and were essentially littering this zone.  
* Removed the Trading Post rule, since it can't spawn on Wasteland anyway and as such it was redundant.  
* Increased the treasure values to (1500-3000, 9), (3000-5000, 12), (8000-12000, 3) from (1500-3000, 8), (3000-5000, 12), (8000-12000, 3).

#### Artifacts

* Banned the following artifacts: Vampire's Cowl, Dead Man's Boots, Amulet of the Undertaker, Ambassador's Sash, Diplomat's Ring, Statesman's Medal, Orb of Driving Rain, Bird of Perception, Stoic Watchman, Emblem of Cognizance, Legs of Legion, Loins of Legion, Torso of Legion, Arms of Legion and Head of Legion. The Necromancy boosting artifacts are banned because they favour Necropolis - which is regarded as one of the best factions in the game - while being nearly completely useless for all other factions. All other artifacts are banned because they are plain too weak and ineffective.

#### Spells

* Banned the following spells: Protection from Water, View Air, View Earth, Remove Obstacle, Earthquake, Land Mine, Fire Shield, Slayer and Magic Mirror. Most of these spells are far too niche and situational, and are effectively a waste of a precious spell slot in the Mage's Guild. The excaption are View Air and View Earth spells, which are banned because of two reasons - they are relatively slow to use, and they are giving a large amount of information for a low mana cost. There is also an exploit that allows to inspect the generated map even after the timer ends. This exploit is a non-issue on longer time controls, but on the one minute timer setting it is definitely unhealthy.

#### Heroes:

* Banned Ayden. This hero starts with View Earth spell, for which the ban rationale was listed above. Other heroes that start with the banned spells will aren't currently banned because their low impact on the game. If they will be deemed unviable, they will be banned.

### Version 0.1

[Download](./One%20Minute%20Madness%200.1.zip)

First version ever released!