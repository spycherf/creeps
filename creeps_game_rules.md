# Creeps (card game)

_Creeps_ is a single-player card game inspired by _Warcraft III_, set in the world of Azeroth during the Third War. It requires a standard 52-card deck, a few jokers (or any small household objects as substitutes), and optionally some paper clips to track upgrades. A game typically lasts about 30 to 45 minutes.

## Cards

### Suits

- **Hearts** (♥): player
- **Clubs** (♣): resources
- **Diamonds** (♦): level
- **Spades** (♠): creeps

Exceptions: A♥, A♣, and A♠ represent lootable items.

### Ranks

#### Player (♥)

- **2-4, 6-9**: units (2-4 referred to as _workers_)
- **5, 10**: buildings
- **J, Q, K**: heroes

#### Creeps (♠)

- **2-4**: low-level
- **5-10**: mid-level
- **J, Q, K**: high-level

### Values

Each rank has a corresponding _value_:

- **Number cards**: the card's number
- **Heroes**: 10
- **Other face cards**: J = 11, Q = 12, K = 13

What this value represents depends on the suit:

- **Player cards**: their cost; for buildings, the cost of the upgrades they provide
- **Resource cards**: the amount of currency used to acquire player cards and upgrades
- **Level cards**: the player's level, from 1 (A♦) to 13 (K♦)
- **Creep cards**: the number used to calculate damage dealt to the player

Items have no value.

### Health and mana

Cards that take part in combat have _health_, or _hit points_ (HP), representing the amount of _damage_ they can take before being defeated (1 damage = 1 HP). Without bonuses, face cards have 3 HP and number cards have 2 HP—except workers, which only have 1 HP.

Cards with abilities that cost mana also have 1 _mana point_ (MP).

These numbers can be increased by various means, up to a maximum of 4 HP and 2 MP.

Some abilities increase maximum HP or MP only temporarily. When a card gains or loses such a bonus in combat, its current HP or MP is unaffected unless it exceeds the new maximum. In that case, the current value is reduced to match the maximum. For example: a unit with a +1 MP bonus drops from 2/2 MP to 1/1 MP when the bonus is removed, while the same unit at 1/2 MP would remain at 1/1 MP.

## Setup

### Campaign selection

The player first chooses a _campaign_. Each campaign features a different race, along with its own player, creep, and item cards (for an overview, see § [Appendix: List of cards by campaign](#appendix-list-of-cards-by-campaign)).

The following campaigns are available:

- **[Lordaeron](#lordaeron-human-campaign)** (humans)
- **[The Barrens](#the-barrens-orc-campaign)** (orcs)

### Play area

The play area is divided into sections:

- **Base** (in front of the player):
    - **Buildings** (center). Both buildings are placed side by side, face up.
    - **Gold mine** (to the left, about 3 inches wide)
    - **Reserve** (to the right). Remaining player cards are laid out face up, sorted by rank.
- **Battlefield** (above the base, sized for two rows of seven cards)
- **Creeps** (above the battlefield). Creep cards are shuffled and placed face down.
- **Rewards** (on either side of the battlefield):
    - **Level** (bottom). Level cards are sorted and placed face up, with A♦ on top.
    - **Resources** (middle). Resource cards are shuffled and placed face down.
    - **Items** (top). Item cards are shuffled and placed face down.

Jokers and other objects are set aside for later use.

### Starting hand

To form the starting hand, the player draws the top resource card, three non-worker units, and one hero. The units and hero may be chosen freely or selected at random.

## Playing

The game is played in rounds. Each round follows the same sequence of phases, each with a clear objective:

1. **Preparation**. Use resources to develop both army and economy.
2. **Recon**. Dispatch forces to the battlefield to locate a creep camp.
3. **Combat**. Defeat the creeps.
4. **Rewards**. Level up and collect resources and items dropped by the creeps.

### Preparation

The player can engage in three activities during this phase: _training_, _upgrading_, and _gathering_.

#### Training

The player may use available resources to train heroes and units from the reserve. The total value of resources spent must be equal to or greater than the combined value of the selected cards; any excess is lost. Spent resources are discarded face up next to the resource pile.

Reserve cards selected for training are added to the player's hand face down. Workers are placed face down in the gold mine instead, each slightly offset so they all remain visible.

Cards in training are inactive and cannot be used. Training ends at the start of the next preparation phase, at which point the cards are flipped face up.

#### Upgrading

Buildings can research _upgrades_ for units. Each upgrade has a cost equal to the building’s value. The rules for purchasing upgrades are the same as those for training. A building can research more than one upgrade at a time.

While research is in progress, the building is flipped face down. If multiple upgrades are being researched, it is also rotated by 90°. It returns to its previous orientation at the start of the next preparation phase, when research is complete.

As a visual aid, the player can mark upgraded cards with paper clips.

#### Gathering

While in the gold mine, each face-up worker provides 1 additional resource during the preparation phase. This _resource bonus_ does not accumulate between rounds if unused.

### Recon

In this phase, the player selects a _squad_ of up to three cards and places them face up in a row on the battlefield. Workers are also eligible. Only one hero may be deployed.

If no creeps remain from the previous combat phase, a number of cards determined by the player's level (see below) are drawn from the creep pile and placed face up in a row on the battlefield, facing the player’s squad. If the pile is empty, discarded creeps are shuffled to form a new pile.

| Level | Creeps |
| :---: | :----: |
| 1     | 2      |
| 2-3   | 3      |
| 4-7   | 4      |
| 8-10  | 5      |
| 11+   | 6      |

### Combat

Combat consists of a repeating cycle of two steps: the player's _attack_ and the creeps' _retaliation_ (see relevant sections below).

Cards enter combat with full health and mana, after all bonuses from upgrades and passive abilities have been applied. When a card takes damage, it becomes _injured_ and is rotated clockwise for each HP lost—by 90° for cards with 2 maximum HP, and by 45° otherwise. When a card reaches 0 HP, it is _defeated_ and flipped face down. This also removes any positive or negative effects (known as _buffs_ and _debuffs_ respectively).

Combat ends when all cards on one side have been defeated and cannot be revived. There are two possible outcomes:

- **Victory**. The player proceeds to the rewards phase.
- **Defeat**. The player returns to the preparation phase (training and upgrade research are completed as usual).

Regardless of the outcome, surviving cards have their HP and MP replenished, and the battlefield is cleaned up as follows:

_Heroes and units_

- Defeated cards go to the reserve.
- Surviving workers are placed face down in the gold mine. They do not contribute to the resource bonus in the next preparation phase; the player must wait until the end of the next round before flipping them again.
- The remaining cards return to the player's hand.

_Creeps_

- Defeated cards are discarded face down in a horizontal pile next to the creep pile.
- Surviving cards remain on the battlefield. They are shifted to one side to close any gaps left by defeated creeps.

#### Attack

When combat starts, the player selects a card to attack with (the _attacker_). A different card must be chosen for each subsequent attack until all cards have attacked once. The same _attack rotation_ must then be used for the remainder of combat, skipping any cards that have been defeated. It is recommended to reorder the cards to reflect this rotation.

On its turn, a card has one _action_, which must be used either to activate an ability or to perform a _basic attack_. Basic attacks deal 1 damage and may not exceed 2 damage with bonuses. Regardless of the action taken, heroes deal +1 damage to low-level creeps.

##### Player abilities

Player abilities are divided into three types: _passive_, _active_, and _ultimate_. Active and ultimate abilities consume an action, whereas passive ones do not. Each ultimate ability may be used only once per game.

Some abilities have additional attributes, such as:

- **Magical**. Such abilities cannot be used against magic-immune targets. Magical buffs and debuffs can be dispelled.
- **Area**. These abilities affect multiple creeps within a designated area. All creeps in the area are considered targets. The player may position the area so that part of it extends beyond the battlefield edge, thus hitting fewer creeps.

Some abilities are unlocked only when the player reaches a certain level, or through the upgrading system.

##### Items

While they live, heroes may use any number of items from the player's hand, during any card's turn (item-specific restrictions may apply). Used items are discarded face up next to the item pile. There are three items in total; once all have been used, the discard pile is shuffled to form a new pile.

##### Disabling

Some abilities and items can _disable_ one or more creeps, preventing them from retaliating. Unless otherwise specified, this effect lasts for one retaliation only.

#### Retaliation

After the player's turn, creeps that have not been disabled or defeated retaliate.

By default, retaliation targets the attacker. However, if the attacker's action affected a high-level creep—and that creep is not disabled or defeated—the target is determined using the following priority order:

1. A card with 1 HP remaining (if multiple cards qualify, the one with the highest value is selected)
2. The hero, if already injured
3. The attacker

If the retaliation target was defeated as a result of its action before retaliation started, the remaining player card with the highest value is targeted instead.

Retaliation deals 1 damage to the target, +1 damage if the combined value of the remaining non-disabled creeps is 20 or more.

##### Creep abilities

In addition to retaliation damage, creep abilities may trigger under certain conditions—provided those creeps are not disabled or defeated. Magical creep abilities follow the same rules as magical player abilities.

### Rewards

After a victory, the player may earn three types of rewards:

- **Level**. The player levels up by moving the current level card to the bottom of the pile.
- **Resources**. The player draws one resource card.
- **Items**. The player draws one item card for each high-level creep they defeated. If the item pile is empty, the player may not draw from the discard pile. If high-level creeps were defeated during an earlier combat phase but the creeps were only fully cleared later, the player should not forget to draw the corresponding item cards at that time.

## End of the game

The player wins the game when they reach level 13. The game is lost if the player is unable to deploy a squad during the recon phase.

### Hard mode

In this optional mode, the game continues until the player loses. To level up beyond level 13, the level pile is reset, with A♦ now representing level 14. The player no longer gains resources during rewards phases.

## How to read abilities

The ability descriptions below include the following elements (when applicable):

> _Flavor text_
> 
> **Ability name** (type, mana cost, additional attributes, unlocking conditions). Effect.

Some abilities are also marked with an asterisk (*). To help track their effects, jokers should be placed on top of the affected cards or next to them (depending on the ability). Any small household objects can serve as substitutes (coins, bottle caps, rubber bands, etc.).

See § [Combat](#combat) first to understand key concepts used in the descriptions, such as retaliation and disabling.

## Lordaeron (human campaign)

_In the kingdom of Lordaeron, scattered bands of marauders—dubbed creeps by frightened citizens—have been sighted roaming the countryside, pillaging towns and villages. Troubled by these incursions, King Terenas dispatches his forces to restore order and defend the realm from this growing menace..._

### Racial advantage

_Years of war have taught the people of Lordaeron to take up arms in the kingdom's hour of need, joining the regular army as militia._

**Call to Arms**. Permanently grants Peasants +1 maximum HP.

### Upgrades

#### Arcane Sanctum (5♥)

**Priest Master Training**. Teaches Priests the [Inner Fire](#priest-8) ability.

**Sorceress Master Training**. Teaches Sorceresses the [Polymorph](#sorceress-9) ability.

#### Blacksmith (10♥)

**Steel Plating**. Permanently grants Footmen +1 maximum HP.

**Reinforced Leather Armor**. Permanently grants Riflemen +1 maximum HP.

### Player abilities

#### Footman (6♥)

_Backbone of the Lordaeron army, seasoned footmen quickly raise their shield to fend off vicious attacks._

**Defend** (passive). Grants the Footman immunity to creep abilities that are triggered only on the first retaliation. The first damage taken by the Footman is reduced by 1.

#### Rifleman (7♥)

_Improved blunderbusses give the stout dwarven riflemen enough range to strike before the enemy can react._

**Long Rifles** (passive). If the Rifleman attacks first, creeps cannot retaliate.

#### Priest (8♥)

_Hailing from Quel'Thalas, priests heal and infuse their allies with holy magic._

**Heal** (passive). On the Priest's turn, heals an injured player card for 1 HP.

**Inner Fire** (active, 1 MP, magical buff, unlocked at the Arcane Sanctum) (*). Grants a player card +1 damage on its next basic attack and reduces the next retaliation damage it takes by 1.

#### Sorceress (9♥)

_Elven sorceresses harness arcane energy to bind their enemies in heavy chains—or turn them into sheep._

**Slow** (passive, magical debuff). On the Sorceress's turn, disables a creep of the player's choice.

**Polymorph** (active, 1 MP, magical debuff, unlocked at the Arcane Sanctum) (*). Disables the targeted creep until it is damaged.

#### Paladin (J♥)

_Calling on the Light, paladins empower the troops with divine vigor and shield themselves from harm. When the hour is most dire, they bring their fallen comrades back from the dead._

**Divine Shield** (passive). Grants the Paladin immunity to all damage and creep abilities on the retaliation following the Paladin's first turn.

**Devotion Aura** (passive, unlocked at level 4). While the Paladin lives, the threshold for the retaliation damage bonus is raised from 20 to 25.

**Resurrection** (ultimate, 1 MP, unlocked at level 6). Revives up to 2 defeated units with full health and no mana. Resurrected units re-enter the attack rotation in their original order.

#### Archmage (Q♥)

_The archmagi from Dalaran boost their allies' mana reserves and call down ice shards from the skies. As a last resort, they can teleport the troops back to safety._

**Blizzard** (active, 1 MP, magical, area). Deals 1 damage to each creep in an area 3 cards wide.

**Brilliance Aura** (passive, unlocked at level 4). While the Archmage lives, grants each card in the squad +1 maximum MP.

**Mass Teleport** (ultimate, 1 MP, unlocked at level 6). Moves the Archmage and all surviving units back to the player's hand, ending combat in defeat ([end-of-combat rules](#combat) apply).

#### Mountain King (K♥)

_The dwarven thanes of Khaz Modan wield enchanted weapons to crush their foes. When channeling their ancestral heritage, they enter a state of unstoppable fury._

**Storm Bolt** (active, 1 MP, magical). Deals 2 damage and disables the targeted creep.

**Bash** (passive, unlocked at level 4). The Mountain King's basic attacks also disable the targeted creeps.

**Avatar** (ultimate, 1 MP, unlocked at level 6). Deals 2 damage and disables the targeted creep. For the remainder of combat, the Mountain King's basic attacks deal +1 damage.

### Creep abilities

#### Trapper (5♠)

_Troll trappers have mastered the art of pinning down their prey with heavy nets._

**Ensnare** (*). When damaged, the Trapper casts a net on the attacker. On its next turn, that card has no action, but still triggers retaliation.

#### Bandit (6♠)

_Bandits lurk in the shadows, striking when least expected._

**Hide**. When combat starts, the Bandit is hidden and can only be targeted with area abilities. If not revealed by such an ability, the Bandit becomes visible on the first retaliation and deals 1 damage to the attacker.

#### Assassin (7♠)

_Gnoll assassins coat their bolts with a lethal toxin before battle._

**Envenomed Weapons** (*). On the first retaliation, the Assassin shoots a poisoned bolt at the attacker. That card is defeated at the end of its next turn, unless combat ends first.

#### Magi (8♠)

_The two-headed ogre magi incite their comrades to violence by imbuing them with supernatural speed._

**Bloodlust**. If at least two creeps are currently injured or defeated, creeps retaliate twice. The second retaliation does not trigger creep abilities.

#### Geomancer (9♠)

_Kobold geomancers call upon the power of earth to strip magic from foes and allies alike._

**Abolish Magic** (magical). At the start of each retaliation, the Geomancer dispels 1 magical effect applied by the player, prioritizing as follows: long-lasting debuffs, turn-long debuffs, buffs (e.g., [Polymorph](#sorceress-9) &rarr; [Slow](#sorceress-9) &rarr; [Inner Fire](#priest-8)).

#### Golem (10♠)

_The rocky constitution of golems protects them from magic._

**Spell Immunity**. Grants the Golem immunity to magical player abilities.

### Items

#### Potion of Healing (A♥)

Heals the hero for 2 HP. This item may only be used if the hero is injured.

#### Ankh of Reincarnation (A♣)

Once obtained, this item must be placed on top of the hero during recon. When defeated, the hero is immediately revived with 2 HP and no mana, and the item is discarded.

#### Infernal Stone (A♠)

Calls an infernal down from the sky, disabling creeps on impact in an area 2 cards wide. This demon has 2 HP and joins the attack rotation before the hero's turn. It is discarded when combat ends.

## The Barrens (orc campaign)

_Following the counsel of the Prophet, Thrall leads the Horde across the Great Sea. After a perilous voyage, the orcs land upon the savage shores of Kalimdor. With their newfound troll and tauren allies, they venture inland, where the harsh wilderness and its brutal inhabitants test their strength and resolve..._

### Racial advantage

_Driven from their dying world, orcs have learned to seize whatever spoils they can find._

**Pillage**. In the preparation phase following a victory, increases the resource bonus by 1 for each Raider, Grunt, or Peon that survived combat.

### Upgrades

#### Spirit Lodge (5♥)

**Witch Doctor Master Training**. Teaches Witch Doctors the [Healing Ward](#witch-doctor-8) ability.

**Shaman Master Training**. Teaches Shamans the [Bloodlust](#shaman-9) ability.

#### War Mill (10♥)

**Thorium Weapons**. Permanently grants Raiders and Grunts +1 damage against low-level creeps.

**Thorium Armor**. Permanently grants Raiders and Grunts +1 maximum HP.

### Player abilities

#### Grunt (6♥)

_The battle-hardened grunts fight with savage fury when brought to the brink of death._

**Berserker Strength** (passive). If all high-level creeps are disabled or defeated, the first damage that would defeat the Grunt is reduced by 1. While at 1 HP, the Grunt deals +1 damage.

#### Raider (7♥)

_Raiders sweep across the battlefield astride their wolves, trapping unsuspecting enemies with nets._

**Ensnare** (passive) (*). On the Raider's turn, disables a creep of the player's choice until the start of the Raider's next turn—or, if the Raider is defeated, until that turn would occur.

#### Witch Doctor (8♥)

_These cunning trolls from the Darkspear Islands channel voodoo magic through their totems to stun foes and mend allies._

**Stasis Trap Ward** (passive, area). On the Witch Doctor's first turn, disables creeps in an area 3 cards wide.

**Healing Ward** (active, 1 MP, unlocked at the Spirit Lodge) (*). Summons a ward next to the Witch Doctor that restores 1 HP to the player card with the fewest HP remaining. If multiple cards qualify, the player chooses which one is healed. This effect triggers again at the start of the Witch Doctor's next two turns—or, if the Witch Doctor is defeated, when those turns would occur. The ward is rotated by 90° with each additional trigger and discarded when it expires.

#### Shaman (9♥)

_Having renounced fel magic, shamans draw on the elements to invigorate the Horde and disrupt their enemies._

**Purge** (passive, magical | magical debuff) (*). On the Shaman's turn, either dispels all magical debuffs from a player card, or dispels all magical buffs from the targeted creep and disables it. For the remainder of combat, that creep's value is ignored when calculating retaliation damage. If the target is a summoned creep, it is defeated.

**Bloodlust** (active, 1 MP, magical buff, unlocked at the Spirit Lodge). On their next turn, other cards in the squad get an additional action.

#### Blademaster (J♥)

_The skilled swordsmen of the Burning Blade clan move so fast they leave afterimages behind. When the battle turns dire, they unleash their rage in a whirlwind of blades._

**Mirror Image** (active, 1 MP). Performs a basic attack on the targeted creep. Two illusions of the Blademaster each deal 1 damage to a creep of the player's choice. Their target may be the same or different.

**Wind Walk** (passive, unlocked at level 4). The Blademaster's first basic attack deals +1 damage.

**Bladestorm** (ultimate, 1 MP, area, unlocked at level 6). Deals 1 damage to all creeps and grants the Blademaster immunity to magical creep abilities on the following retaliation.

#### Far Seer (Q♥)

_Close advisors to Thrall, seers cast their gaze across vast distances and harness lightning in battle. These powerful shamans can make the very earth tremble._

**Chain Lightning** (active, 1 MP, magical, area). In an area 3 cards wide, starting from either left or right, deals 2 damage to the first target, 1 damage to the next, and 1 damage to the last if it is a low- or mid-level creep.

**Far Sight** (passive, unlocked at level 4). During recon, with the Far Seer in hand, the player may draw creep cards before deploying their squad. Hidden creeps are revealed when combat starts.

**Earthquake** (ultimate, 1 MP, area, unlocked at level 6). Deals 1 damage to each low- or mid-level creep in an area 4 cards wide, and disables all creeps in that area until the start of the Far Seer's next turn—or, if the Far Seer is defeated, until that turn would occur.

#### Tauren Chieftain (K♥)

_Tauren chieftains charge their foes with crushing force. Their strong spirit allows them to cheat death once._

**Shockwave** (active, 1 MP, area). Deals 1 damage to each creep in an area 3 cards wide.

**War Stomp** (passive, area, unlocked at level 4). On the Tauren Chieftain's first turn, disables creeps in an area 3 cards wide.

**Reincarnation** (ultimate, unlocked at level 6). When defeated, the Tauren Chieftain is immediately revived with full health and mana.

### Creep abilities

#### Hunter (5♠)

_Despite their bulky frame, the elusive quillboar hunters are quick to dodge incoming blows._

**Evasion**. If not disabled, the Hunter avoids the first basic attack targeting it.

#### Medicine Man (6♠)

_The Razormane tribe's shamans conjure ghostly boars to overwhelm the enemy._

**Feral Spirit** (*). When combat starts, the Medicine Man summons a spirit pig with 1 HP and a value of 6, placed to its left.

#### Windwitch (7♠)

_Vindictive to the last, harpy witches enfeeble those who dare strike at them._

**Faerie Fire** (magical debuff) (*). When damaged, the Windwitch curses the attacker. Starting on its next turn, that card takes +1 retaliation damage.

#### Impaler (8♠)

_These elite centaur archers loose fiery arrows as they stampede across the plains._

**Searing Arrows**. On each retaliation, the Impaler deals 1 damage to the highest-value player card remaining.

#### Nightcrawler (9♠)

_When the sun sets over the Barrens, murlocs emerge from the tide to slaughter their victim._

**Hide**. When combat starts, the Nightcrawler is hidden and can only be targeted with area abilities. If not revealed by such an ability or [Far Sight](#far-seer-q), the Nightcrawler becomes visible on the first retaliation and deals 1 damage to the attacker.

**Envenomed Weapons** (*). On the first retaliation where the Nightcrawler is not disabled, the attacker is poisoned. That card is defeated at the end of its next turn, unless combat ends first.

#### Storm Wyrm (10♠)

_These thunder lizards breathe lightning and devour their prey, slowly digesting them alive._

**Devour**. When hit by a basic attack for the first time, the Storm Wyrm consumes the attacker when retaliation starts. That card is placed on top of the Storm Wyrm. Starting with the current retaliation, it takes 1 damage on each retaliation but is immune to all other damage and creep abilities. While being consumed, that card has no action on its turn, but still triggers retaliation. It is returned to its original position when the Storm Wyrm is defeated.

**Lightning Shield** (magical buff). The Storm Wyrm deals 1 damage to the attacker when hit by a basic attack. This effect triggers even if the Storm Wyrm is disabled or defeated. The damage is applied immediately after the attack, before retaliation starts.

#### Razormane Chieftain (J♠)

_When threatened, these fierce quillboar warriors erect their jagged spines._

**Thorns Aura**. If already injured, the Razormane Chieftain deals 1 damage to the attacker when hit by a basic attack. This effect triggers even if the Razormane Chieftain is disabled or defeated. The damage is applied immediately after the attack, before retaliation starts.

#### Harpy Queen (Q♠)

_With a powerful flap of their wings, harpy queens send their foes flying into the air._

**Cyclone** (magical) (*). The first time the Harpy Queen is damaged while not disabled, the attacker is thrown into the air when retaliation starts. On its next turn, that card has no action, but still triggers retaliation. Until that turn, it is immune to all damage and creep abilities, and retaliation that would target it instead follows the priority order for high-level creep targeting. If the affected card is a hero, items cannot be used during this time.

#### Centaur Khan (K♠)

_The mighty centaur leaders rise again after falling in battle._

**Reincarnation**. When defeated for the first time, the Centaur Khan is revived with 2 HP when retaliation starts.

### Items

#### Health Stone (A♥)

Heals the hero for 1 HP. This item is then placed on top of the hero. Starting on the hero's next turn, it may be consumed to restore another 2 HP. It is discarded when consumed, otherwise when combat ends. This item may only be used if the hero is injured.

#### Potion of Mana (A♣)

Restores 1 MP to the hero. This item may not be used if the hero is at full mana.

#### Scroll of the Beast (A♠)

When used, this item is placed next to the squad. The squad's next three basic attacks deal +1 damage. The item is rotated by 45° after each attack and discarded when it expires.

## Appendix: List of cards by campaign

### Player

| ♥    | Lordaeron                           | The Barrens                             |
| :--: | ----------------------------------- | --------------------------------------- |
| 2-4  | Peasants                            | Peons                                   |
| 5    | [Arcane Sanctum](#arcane-sanctum-5) | [Spirit Lodge](#spirit-lodge-5)         |
| 6    | [Footman](#footman-6)               | [Grunt](#grunt-6)                       |
| 7    | [Rifleman](#rifleman-7)             | [Raider](#raider-7)                     |
| 8    | [Priest](#priest-8)                 | [Witch Doctor](#witch-doctor-8)         |
| 9    | [Sorceress](#sorceress-9)           | [Shaman](#shaman-9)                     |
| 10   | [Blacksmith](#blacksmith-10)        | [War Mill](#war-mill-10)                |
| J    | [Paladin](#paladin-j)               | [Blademaster](#blademaster-j)           |
| Q    | [Archmage](#archmage-q)             | [Far Seer](#far-seer-q)                 |
| K    | [Mountain King](#mountain-king-k)   | [Tauren Chieftain](#tauren-chieftain-k) |

### Creeps

| ♠    | Lordaeron                 | The Barrens                                   |
| :--: | ------------------------- | --------------------------------------------- |
| 2-4  | Murlocs                   | Quillboars                                    |
| 5    | [Trapper](#trapper-5)     | [Hunter](#hunter-5)                           |
| 6    | [Bandit](#bandit-6)       | [Medicine Man](#medicine-man-6)               |
| 7    | [Assassin](#assassin-7)   | [Windwitch](#windwitch-7)                     |
| 8    | [Magi](#magi-8)           | [Impaler](#impaler-8)                         |
| 9    | [Geomancer](#geomancer-9) | [Nightcrawler](#nightcrawler-9)               |
| 10   | [Golem](#golem-10)        | [Storm Wyrm](#storm-wyrm-10)                  |
| J    | (unnamed)                 | [Razormane Chieftain](#razormane-chieftain-j) |
| Q    | (unnamed)                 | [Harpy Queen](#harpy-queen-q)                 |
| K    | (unnamed)                 | [Centaur Khan](#centaur-khan-k)               |

### Items

|      | Lordaeron                                         | The Barrens                                   |
| :--: | ------------------------------------------------- | --------------------------------------------- |
| A♥   | [Potion of Healing](#potion-of-healing-a)         | [Health Stone](#health-stone-a)               |
| A♣   | [Ankh of Reincarnation](#ankh-of-reincarnation-a) | [Potion of Mana](#potion-of-mana-a)           |
| A♠   | [Infernal Stone](#infernal-stone-a)               | [Scroll of the Beast](#scroll-of-the-beast-a) |
