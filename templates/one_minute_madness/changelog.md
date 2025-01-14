---
title: HoMM3 Template Vault | One Minute Madness changelog
---

[<<-home](../..)  
[<<-back](index.html)

## One Minute Madness - Changelog

### Version 2.3a

[Download](./One%20Minute%20Madness%202.3a.h3t)

* Fixed the missing combo artifact bans. Apparently HotA Crew screwed up and somehow didn't add every single combo artifact to the template editor, and as such Ironfist of the Ogre was possible to assemble. Now it is fixed.

### Version 2.3

[Download](./One%20Minute%20Madness%202.3.h3t)

* Thanks to the new functionality in the template and map formats, the possibility of assembling any of the combination artifacts are disabled.
* Because of the above, the following artifacts were unbanned:
    * Targ of the Rampaging Ogre
    * Rib Cage
* Previously, I have implemented resource pile caps on all zones. When it comes to wood, ore and precious resources, the values seem all fine. When it comes to gold though... well, the caps were a bit too much, to say the least. For this reason the caps are changed as follows:
    * Starting zone:
        * Gold: max. 5 -> max. 16
        * Campfire: max. 4 -> max. 8
        * Random resource: max. 4 -> max. 6
    * Grass zone:
        * Gold: max. 13 -> max. 15
        * Campfire: max. 8 -> max. 12
        * Random resource: max. 8 -> max. 10
    * Wasteland zone:
        * Treasure Chest: max. 7 -> max. 10
        * Gold: max. 8 -> max. 14
        * Campfire: max. 12 -> max. 11
        * Random resource: max. 4 -> max. 3
* The max road block value is set as following:
    * Grass zone: 2000
    * Wasteland zone: 2000
    * Desert zone: 5000
* Unbanned First Aid, Learning and Eagle Eye. These skills have been buffed considerably - and in case of Learning, maybe even too considerably. These skills will have to be monitored down the line.
* Did another set of technical adjustments to zone generation in vain hopes that it will make the gameplay more sane.

### Version 2.2

[Download](./One%20Minute%20Madness%202.2.h3t)

Just before the start of the next season's signups, there is a need for a yet another update. This time, it is mostly about getting the amount of resources under control, cause at this point there were simply too many of them, and the sides of map got really unequal in this context.

* Slightly lowered treasure count on Wasteland, to make it a bit less rich in gold.
* Implemented the caps on resource piles on all zones except for the Desert ones.. The exact numbers would be just noise in the documentation and hence are ommited. The reason for this is to avoid utterly rich map rolls where you get so much gold that you can double build even the most expensive builds without literally any care for economy - and it should help at least little bit to equalize the sides of the map. Desert zones are excluded from the cap because they already have a minuscule amount of resources in them, and as such the cap is unnecessary.
* Heavily increased treasure count on - with every single object having its count capped, this makes starting zones more stable, and provides some way to detect the effective map size.
* Added a Nomad dwelling on the Desert zone. Players have noted the need to alleviate the necessity of Pathfinding due to increased sizes of the Desert zones - and honestly, needing to do something makes sense. I do not know if a Nomad dwelling will help much in this case, but it was a common suggestion, and after giving it a bit of thought, it does make sense to include it.

### Version 2.1

[Download](./One%20Minute%20Madness%202.1.h3t)

Version 2.1 is simultaneously a massive update and a tiny one at the same time. There is no revolution in vein of the 1MM 1.7, which reworked Conflux's gameplan and removed the Chain Lightning spell from the pool - and yet, compared to the previous version, it will be a whole new experience... all because I have finally found a way to make the maps generate much wider on average.

* **Changed the map generation parameters in various ways to widen the map rolls.** The changes from HotA 1.7.0 took away a tool from the template makers' repertoire, and as such it took me quite a while to figure out a way to fix the template after what can only be summed up to be a bad incident. The exact changes are kinda too boring and too technical to list them there, but main one of them was massively bumping the zone sparseness value, which ended up biasing the RMG towards the “butterfly” shaped maps. The reason why this works is completely arcane to me, but at this point I'll just happily take this result.
* **Increased the object value of 5000 XP Pandora's Boxes back to the default of 6000** on both Wasteland and Grass zones. This is a change meant mostly to force the boxes to spawn in separate object groups. The change is expanded to the Grass zone Pandora for consistency.
* **Added a Mansion on the Desert zone.** I do think that it might be an interesting addition to the game, considering the difficulty of this creature bank and the pretty darn solid reward. It is a bit of an experiment whether it will work out to be a good addition or not, but it shouldn't break anything at this point.
* **Changed the treasure values on both Wasteland and Desert zones.** These are just some minor adjustments to accomodate the changes above, as well as complete the "split the 5k XP Pandoras into two object groups" task.
* **Removed the object rule for Gardens of Revelation on the Wasteland zone.** Gardens of Revelation can't spawn on Wasteland anyways, so the rule turns out to be extraneous. Yes, nobody noticed this before version 2.0c.
* **Increased the maximum Schools of Magic on Wasteland to 3, and lowered the maximum Star Axes on Wasteland to 2.** I want to make knowledge stat a bit more accessible here without bumping the "free" spell power.
* **Unbanned Murdoch.** Murdoch is a solid hero that can work fine as a potential main hero.
* **Banned Frederick.** As Murdoch would be a 17th hero, someone has to go - and Frederick, as a problematic hero, is the one to go. Getting him as a second or third hero in tavern provides an insane advantage - an average of 12 automatons is basically an entire army that can singlehandedly clear even the hardest encounters on grass one after another.

Additionally, I checked the current documentation and fixed a few mistakes and inconsistencies I've found there. 

### Version 2.0c

[Download](./One%20Minute%20Madness%202.0c.h3t)

* Restored the missing object rule allowing the gold to spawn on the starting zone. I have no idea whether this was caused by an editor bug or my own misclick - but it is a thing that happened and requires a hotfix.

### Version 2.0b

[Download](./One%20Minute%20Madness%202.0b.h3t)

As maddening as it is, the HotA update completely shifted the way how the random maps generate... in an undocumented way. Yeah. Fun. The result of these changes is how ridicolously unstable the map rolls are, and how biased they are towards the excessively tight and poor rolls. The degree of this phenomena is unacceptable, and for this reason a mid-season emergency patch to the template to adress these issues is released.

* The zone IDs have been shifted. Now, the zones 5 and 6 are the grass zones (wass 5 and 7), and zones 7 and 8 are the wasteland zones (was 6 and 8).
* The size values of the zones have been slightly shifted around to aid getting
* The treasure values of the desert zones have been increased.

Additionally, from the documentation the exact treasure values of the zones have been removed, as they provide nothing much else than just noise for the players. People wishing to check the exact values can easily just check the template in the editor.

### Version 2.0a

[Download](./One%20Minute%20Madness%202.0a.h3t)

* Restored the 100 turn battle limit that was removed due to a regression in the template editor.

### Version 2.0

[Download](./One%20Minute%20Madness%202.0.h3t)

Welp, Factory is finally somehow out, and with it some really important changes that necessiate a quick update to this template.

* Changed the extension of the template file to `.h3t`, as required by the new version of HotA.
* Banned Agar. Reason - he has the View Earth spell, which I do believe to be incompatibile with the format.
* Unbanned Frederick - he is a campaign hero with a reasonable starting army and skillset, and matches the class with the freshly banned Agar.
* First Aid skill has been unbanned. With the changes it got it is now a skill that has a proper niche, and I can see it being used especially for the Grass zone farming. The currently banned First Aid specialists will not be unbanned just yet, but the possibility of it happening is on the table.

### Version 1.7b

[Download](./One%20Minute%20Madness%201.7b.zip)

* Adjusted the zone positioning - the attempt from 1.7 at biasing the RMG towards wider map rolls did not work, and this is the another attempt at this.
* Bumped the treasure values in the starting zone to (500-3000, 25), (5000-9000, 6). The changes needed to handle the addition of the Elemental Conflux caused a significiant reduction of Gold spawned - which was very much not the intention of this change. This aims to counteract this a bit.
* Increased the frequency of Gold spawns from 8 to 9 on the starting zone.

### Version 1.7a

[Download](./One%20Minute%20Madness%201.7a.zip)

* Implemented the missing change that bans the Charm of Eclipse and Seal of Sunset artifacts. With so many changes on the list this just slipped through.

### Version 1.7

[Download](./One%20Minute%20Madness%201.7.zip)

The 1.7 update to the One Minute Madness is comparatively huge, and it is a little bit more experimental than I would normally be comfortable with. For this reason, I wouldn't be surprised if a 1.8 release will be necessary before the start of the next season of 1MM League.

#### Unchaining the meta

* **Banned the Chain Lightning spell.** This spell was massive since the early days of One Minute Madness. Most final battles revolve around the use of this spell, and usually the counterplay against it is limited. The spell itself is also very accessible, meaning that you will see it in nearly every single game, and the time and resource cost of obtaining it is not that high. Ultimately, the combination of very high power level and ease of access makes this spell problematic, and despite the ripple effects it may have on the metagame I've made the decision to let this spell go. That being said, I am not against rolling back this change if it will be necessary, though I feel that it will be a net positive for the health of the metagame.
* **Banned Protection from Earth.** With Chain Lightning being removed, casting Protection from Earth at the Expert level would result in your army being effectively walled from most magical damage.
* **Banned Protection from Air.** With no Chain Lightning to protect from, this spell simply doesn't do enough to warrant further inclusion in the pool of spells.
* **Removed Charm of Eclipse and Seal of Sunset artifacts.** Combined with the Interference skill, they provide up to 50% reduction of opponent's spell power. Even with Chain Lightning in the game, that was simply way too much.
* **Increased the maximum amount of Schools of Magic to 2 and Star Axes to 3 on Wasteland zone.** Chain Lightning was the main reason why these objects were limited in such an aggressive manner, and - combined with the changes above - this should slightly relax things and give a tiny bit more breathing room for the mages.

#### Conflux restoration

* **Added Elemental Conflux dwelling to the starting zone.** This faction is the least liked one out of all 10 available on the One Minute Madness. It has weak army and strong mages, pushing this faction to pretty much a single strategy - Chain Lightning rush. During the early seasons of the 1MM League, this strategy was incredibly strong - but nowadays, people have adapted, and the wild rush that bets everything on a single card is far too fragile now wile also being hard to execute - not to mention that it also relies on having good RNG rolls to reach your opponent in time. With Chain Lightning banned, this faction is left with practically nothing, and to avoid the need to ban this faction, this composite external dwelling is given to Conflux in hopes that it will help this faction to, well, do anything.
* **Adjusted the treasure values of the starting zones due to the need to accommodate the Elemental Conflux.** The amount of resources available from this zone should not change much - but the change is still necessary to make room for such high value dwelling to spawn. Note that the object value of dwellings is currently impossible to change via an object rule.

#### Heroic Shuffle

* **Unbanned Mutare, Xeron and Kilgor.** I have been requested many, many times to add some of the campaign heroes, and these three are the ones that may provide something interesting to the gameplay while also not being terribly broken. Granted, it would be possible to also add Mutare Drake and Haart Lich to the template, the fact that these two are alternate versions of other heroes does create a bit of weird dissonance.
* **Banned Gird.** Since adding Kilgor to the pool of heroes would cause the amount of Stronghold heroes to equal 17 - one over the cap of 16 selectable starting heroes per faction. I expect Gird's removal to have a low enough impact to not cause any significiant change.
* **Banned Corkes.** This hero is by far the strongest and the most game-changing hero available on this template. While in Cove it does not break the game, for other factions getting Corkes may be a bit too much of an advantage over the opponent. Even if you are playing Necropolis, who doesn't have that much use of Corkes, you will still be happy to see him in tavern, because this means your opponent doesn't have him available.

#### Other changes

* **Removed Witch Huts.** In most games, Witch Huts have very little impact on the game and are a somewhat boring of an object... until you find out that you got Estates - an incredibly powerful skill on this template - for free, and you can give it to every single non-main hero you have. This gives you an incredibly stupid economic advantage to the point of breaking down the game and potentially causing a non-game. This huge disparity of effects that this object can have is undesirable for this template, and hence this object is removed from this template.
* **Removed Universities.** University is an object that may fix up the secondary skills of your hero for free, and can still house Estates skill. While having to pay for Estates makes it less problematic than getting it for free from a Witch Hut, I still don't like the idea of this happening - especially combined with how much space on the map University takes, which in turn may cause map generation issues down the line.
* **Adjusted the positioning of the zones to bias them towards wide rolls.** The most extreme of the narrow map rolls were a bit too tight with resources and navigating space. This change hopefully will make the situation a bit better, even though it does not eliminate the problem completely.
* **Unbanned Earthquake.** I wanted to add this spell to the pool for a long, long time as a potentially interesting option for use in sieges, but couldn't do so to not overpopulate the tier 3 spell pool. Removing Protection from Earth gave back that little bit of room to allow me to introduce Earthquake back into the fray.
* **Banned Protection from Fire.** When looking through the spell list, I have noticed that Protection from Fire, which is far from a valuable spell, is still available. Taking this into account, and the fact that other Protection spells are now banned too, this one is now also removed.
* **Slightly increased the frequency of Wood resource spawns.** Building up towns requires more Wood than Ore, and this change is done to accommodate for this.

### Version 1.6

[Download](./One%20Minute%20Madness%201.6.zip)

* Banned Rion and Verdish. The possibility of losing tier 2 stacks from the tavern hero in exchange for a first aid tent just feels bad for Castle and Fortress. 
* Banned Orb of Tempestous Fire. This artifact was an experimental addition to this template, and the experiment simply failed. This artifact had little to no use and was far, far too niche to justify keeping it in the major artifact pool.
* Changed the timer recommendation from 1+1+3 to 1+1+2. The combat timer was extremely long, and allowed for more abuse than it is normally expected and acceptable. With support from the community, this timer was shortened to a more appropriate value.

### Version 1.5a

[Download](./One%20Minute%20Madness%201.5a.zip)

* Actually implemented the missing changes for 1.5 version.

### Version 1.5

[Download](./One%20Minute%20Madness%201.5.zip)

* Banned Targ of the Rampaging Ogre. Ironfist of the Ogre, while it was cool at first, was shown to be a significiant issue when it comes to the balance of the template. It was left in the game as an unlikely late game goal meant for stallbreaking, but it has become a thing that players may specifically hunt out and sometimes even assemble it as early as 121-122. This affects the metagame of this template to an unacceptable level, causing major disparities between both sides of the map with a surprisingly high frequency. As for why specifically the Targ, and not any other element of this set: there is one extra shield in the form of the Dragon Scale Shield available in the pool of major artifacts - which makes removing the Targ less of a practical issue.
* Banned Cape of Velocity. Over the course of the Season 2 of the One Minute Madness League it was shown that this was way too high of a speed boost - especially when combined with Ring of the Wayfarer it was affecting the game in a way too strong manner to be acceptable, even if it wasn't an autowin find.
* Unbanned Orb of Tempestous Fire. It is a somewhat experimental addition to this template, but hopefully it may be an interesting option which allows for stronger Magic Arrows and possible push to make Fireballs and Infernos at least a bit more viable opions for use in combat.

### Version 1.4

[Download](./One%20Minute%20Madness%201.4.zip)

This is most likely the final update of this template, at least until the next HotA release. I am currently very satisfied with both the balance and design of this template - and it is really hard to come up with any way to actually improve this template at this point. Of course, this doesn't mean I will stop supporting this template - of course not! The 1MM league will continue, and I will intervene with an update in case of any issues requiring one.

* Banned Cape of Silence. This artifact has been found to be broken by virtue of invalidating two factions barred from high level spell use, namely Fortress and Stronghold - and as such it was extremely unhealthy to the metagame, effectively dictating the result of the game in many cases.

### Version 1.3a

[Download](./One%20Minute%20Madness%201.3a.zip)

* Fixed the occasional issue where the green monolith color was taken by one of the offroad connections between zones 1 and 2.

### Version 1.3

[Download](./One%20Minute%20Madness%201.3.zip)

#### General Settings

* Banned Leena. While she wasn't winning the games by herself, she was an autobuy hero - even at level 1, she contributes to the economy immensely, instantly making the game significiantly easier for the player who buys her. Other gold generating heroes, along with the Finance skill is currently put on a watchlist - depending on the data gathered from games and player opinion they may be banned too in a future version.
* Minor improvements to the stability of zone generation.

#### Zones 5 and 7

* Forced the amount of Trees of Knowledge on this zone to 2. This object provides interesting decisions to the players, especially in lategame - and as such, they contribute positively to the map. Additionally, they may become important enough in some games that they should spawn in a more controlled manner.

#### Zones 1 and 2

* Reworked connections between these zones - now the road connection should always be the green two-way monolith, and there shouldn't be an offroad connection spawning in a way that completely blocks the expansion into the desert zone anymore.

### Version 1.2

[Download](./One%20Minute%20Madness%201.2.zip)

#### Zones 1 and 2

* Increased the treasure value to (3000-6000, 9), (10000-16000, 15), (12000-20000, 9). This is done to stabilize the amount of the major artifacts on the map - the games had too high of a chance to become unbalanced just because of one player getting all two major artifacts on the entire map.

#### Zones 6 and 8

* The amount of stat boosting objects have been hard capped to prevent ridiculous generations with faaaaar too many stat points. The stat boosting objects all have their frequency changed and their amount limited:
    * School of War
        * frequency 500
        * max per zone 2
    * School of Magic
        * frequency 300
        * max per zone 2
    * Marletto Tower
        * frequency 700
        * max per zone 3
    * Mercenary Camp
        * frequency 700
        * max per zone 3
    * Star Axis
        * frequency 600
        * max per zone 2
    * Garden of Revelation
        * frequency 600
        * max per zone 3
    * Arena
        * frequency 200
        * max per zone 1
    * Colosseum of the Magi
        * frequency 200
        * max per zone 1
    * Library of Enlightenment
        * Disabled
* For the same reason, the amount of Learning Stones has been capped to 5.

### Version 1.1a

[Download](./One%20Minute%20Madness%201.1a.zip)

#### Zones 9 and 10

* As an attempt to reduce the chance of a missing Town Gate in this zone, the following changes were applied:
    * Increased the value of Town Gate to 750
    * Decreased the frequency of every other object available on this zone by 80%.

### Version 1.1

[Download](./One%20Minute%20Madness%201.1.zip)

#### General Settings

* Banned Armageddon, Counterstrike, and Sorrow spells. Armageddon is nearly impossible to counter on this template - the only reasonable way to do so is to kill the opposing armageddon-resistant units, or preemptively cast Antimagic or Mass Protection from Fire. Each of these options requires outspeeding the opponent and having a strong starting placement - and even then, you have to deal with the fact that opponent has many other options. Counterstrike and Sorrow are simply far too weak to warrant polluting the pool of tier 4 spells.

#### Zones 1 and 2

* Performed a minor bump of the treasure value, up to (3000-6000, 7), (10000-16000, 12), (12000-20000, 6). This was done to add a very slightly higher amount of artifacts on this map.
* Put a cap of 3 Shrines of Magic Thoughts (tier 3 spells) per desert. In some cases, the generated amounts of these shrines was ridicolous, and this cap is put in place to prevent the most extreme generations.

#### Zones 6 and 8

* Reduced the frequency of Star Axes and Gardens of Revelation to 600 to slightly reduce the typical amount of magic stats you can usually reach.

### Version 1.0

This update marks the end of the beta phase. Starting from this version, this template is considered fully viable for competitive play.

[Download](./One%20Minute%20Madness%201.0.zip)

#### General Settings

* Completely changed the hero banlist. The Eagle Eye heroes were unbanned, while Solmyr, Deemer, Aislinn and Giselle were banned. The Eagle Eye heroes aren't as bad as one might think on this template - many of them have Magic Arrow as the starting spell, resulting in being effective in the scout wars. Solmyr, Deemer and Aislinn are extraordinarily powerful from the get go - not only they are dominating as main heroes, but also picking them up in the midgame makes for waaaaaay too easy and too powerful poking heroes. Giselle can just invalidate magic heroes on the spot, making her an unhealthy addition to the metagame.
* Adjusted the Rock Blocks Radius and Zones Sparseness settings again.

#### Zones 1 and 2

* Changed the treasure values to (3000-6000, 6), (10000-16000, 12), (12000-20000, 6). This was done to help with spawning all the objects that should be guaranteed to spawn in this zone. While the numbers may suggest that desert is far richer than before, it is not the case.
* Forced the amount of the 10000 XP Pandora Boxes to 2. They are important enough objective that they need to spawn in a more stable way, and this change is meant to help with doing so.

#### Zones 5 and 7

* Reduced the size of this zone by 1. This is done to avoid bugged map generations.
* To offset the change above, the treasure values were slightly bumped to (1500-3000, 16), (3000-6000, 11), (6000-12000, 4).

#### Zones 9 and 10

* To offset the slightly smaller grass zone, the treasure values are slightly bumped to (500-3000, 38)

### Version 0.6b

[Download](./One%20Minute%20Madness%200.6b.zip)

#### Zones 5 and 7

* Reverted the size value of this zone to 16 to fix a bug introduced by this change.

### Version 0.6a

[Download](./One%20Minute%20Madness%200.6a.zip)

#### General settings

* Banned Boots of Speed. They give a far too immense bonus to movement, resulting in gamewarping advantage. They should have been already banned in 0.6, but due to a bit of forgetfulness this was missed.

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
    * Banned Straker, Ufretin and Piquedram. These three heroes, if they will show up as the second hero, put the player at a massive disadvantage, effectively punishing player for being unlucky.
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

* Banned the following spells: Protection from Water, View Air, View Earth, Remove Obstacle, Earthquake, Land Mine, Fire Shield, Slayer and Magic Mirror. Most of these spells are far too niche and situational, and are effectively a waste of a precious spell slot in the Mage's Guild. The exception are View Air and View Earth spells, which are banned because of two reasons - they are relatively slow to use, and they are giving a large amount of information for a low mana cost. There is also an exploit that allows to inspect the generated map even after the timer ends. This exploit is a non-issue on longer time controls, but on the one minute timer setting it is definitely unhealthy.

#### Heroes:

* Banned Ayden. This hero starts with View Earth spell, for which the ban rationale was listed above. Other heroes that start with the banned spells aren't currently banned because their low impact on the game. If they will be deemed unviable, they will be banned.

### Version 0.1

[Download](./One%20Minute%20Madness%200.1.zip)

First version ever released!