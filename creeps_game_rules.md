# Creeps (card game)

_Creeps_ is a single-player card game inspired by Warcraft III. It borrows several gameplay elements from [Duel 52](https://juddmadden.com/duel52/) (designed by Judd Madden and Nina Riddell) and from [Mercenaries](https://github.com/spycherf/mercenaries). It requires a standard 52-card French-suited deck, plus 2-3 jokers (or any small household objects as substitutes). A game typically lasts about 30 to 45 minutes (depending on the player's experience).

## Setting

The game is set on Azeroth, shortly before the Third War. In the human kingdom of Lordaeron, scattered bands of marauders—dubbed _creeps_ by frightened citizens—have been sighted roaming the countryside, pillaging towns and villages. Troubled by these incursions, King Terenas dispatches his forces to restore order and defend the realm from this growing menace...

## Cards

### Suits

- **Hearts** (♥): player
- **Clubs** (♣): resources
- **Diamonds** (♦): level
- **Spades** (♠): creeps

Exceptions: A♥, A♠, and A♣ represent lootable items (see § [Rewards](#rewards) and [Items](#items)).

### Ranks

See § [Playing](#playing) and [Abilities](#abilities) for more information on what cards do.

#### Player (♥)

_Units_

- **2/3/4**: peasants
- **6**: footman
- **7**: rifleman
- **8**: priest
- **9**: sorceress

_Heroes_

- **J**: paladin
- **Q**: archmage
- **K**: mountain king

_Buildings_

- **5**: arcane sanctum
- **10**: blacksmith

#### Creeps (♠)

- **2/3/4**: murlocs
- **5**: trapper
- **6**: bandit
- **7**: assassin
- **8**: magi
- **9**: geomancer
- **10**: golem
- **J/Q/K**: bosses

### Values

Each rank has a corresponding _value_:

- **Number cards**: the card's number
- **Heroes**: 10
- **Other face cards**: J = 11, Q = 12, K = 13

What this value represents depends on the suit:

- **Player cards** (♥): their cost; for buildings, the cost of the upgrades they provide
- **Resource cards** (♣): the amount of currency used to acquire player cards and upgrades
- **Level cards** (♦): the player's level, from 1 (A) to 13 (K)
- **Creep cards** (♠): the number used to calculate damage dealt to the player

Items have no value.

### Health and mana

Cards that take part in combat have _health_, or _hit points_ (HP), representing the amount of _damage_ they can take before being defeated (1 damage = 1 HP). Without bonuses, face cards have 3 HP and number cards have 2 HP—except peasants, which only have 1 HP.

Cards with abilities that cost mana also have 1 _mana point_ (MP).

These numbers can be increased by various means, up to a maximum of 4 HP and 2 MP.

Some abilities increase maximum HP or MP only temporarily. When a card gains or loses such a bonus in combat, its current HP or MP is unaffected unless it exceeds the new maximum. In that case, the current value is reduced to match the maximum. For example: a unit with a +1 MP bonus drops from 2/2 MP to 1/1 MP when the bonus is removed, while the same unit at 1/2 MP would remain at 1/1 MP.

## Setup

The play area is divided into sections:

- **Base** (in front of the player):
    - **Buildings** (center). The arcane sanctum (5♥) and the blacksmith (10♥) are placed side by side, face up.
    - **Gold mine** (to the left, about 3 inches wide)
    - **Reserve** (to the right). Remaining player cards are laid out face up, sorted by rank.
- **Battlefield** (above the base, sized for two rows of six cards)
- **Creeps** (above the battlefield). Creep cards are shuffled and placed face down.
- **Rewards** (to the player's left):
    - **Level** (bottom). Level cards are sorted and placed face up, with A♦ on top.
    - **Resources** (middle). Resource cards are shuffled and placed face down.
    - **Items** (top). Item cards are shuffled and placed face down.

Jokers are set aside for later use.

To form the starting hand, the player draws the top resource card, three non-peasant units, and one hero. The units and hero may be chosen freely or selected at random.

## Playing

The game is played in rounds. Each round follows the same sequence of phases, each with a clear objective:

1. **Preparation**. Use resources to develop both army and economy.
2. **Recon**. Dispatch forces to the battlefield to locate a creep camp.
3. **Combat**. Defeat the creeps.
4. **Rewards**. Level up and collect resources and items dropped by the creeps.

### Preparation

The player can engage in three activities during this phase: _training_, _upgrading_, _gathering_.

#### Training

The player may use available resources to train heroes and units from the reserve. The total value of resources spent must be equal to or greater than the combined cost of the selected cards; any excess is lost. Spent resources are discarded face up to the left of the resource pile.

Reserve cards selected for training are added to the player's hand face down. Peasants are placed face down in the gold mine instead, each slightly offset to the right so all cards remain visible.

Cards in training cannot be used. Training ends at the start of the next preparation phase, at which point the cards are flipped face up.

#### Upgrading

The arcane sanctum (5♥) and the blacksmith (10♥) can research _upgrades_ for units. Each upgrade has a cost equal to the building’s value. The rules for spending resources are the same as during training. A building can research more than one upgrade at a time.

While research is in progress, the building is flipped face down; if multiple upgrades are being researched, it is also rotated by 90°. It returns to its previous orientation when research is complete, at the start of the next preparation phase.

The following upgrades are available:

_Arcane sanctum_

- **Priest Master Training**. Teaches priests the [Inner Fire](#player) ability.
- **Sorceress Master Training**. Teaches sorceresses the [Polymorph](#player) ability.

_Blacksmith_

- **Steel Plating**. Permanently grants footmen +1 maximum HP.
- **Reinforced Leather Armor**. Permanently grants riflemen +1 maximum HP.

As a visual aid, the player can mark upgraded cards with paper clips.

#### Gathering

While in the gold mine, each face-up peasant (2/3/4♥) provides 1 additional resource during the preparation phase. This _resource bonus_ does not accumulate between rounds if unused.

### Recon

In this phase, the player selects a _squad_ of up to three cards and places them face up in a row on the battlefield. Peasants are also eligible. Only one hero may be deployed.

If no creeps remain from the previous combat phase, a number of cards determined by the player's level (see below) are drawn from the creep pile and placed face up in a row on the battlefield, facing the player’s squad. If the pile is empty, discarded creeps are shuffled to form a new pile.

Number of creeps to draw by level:

- **Level 1**: 2 cards
- **Levels 2-3**: 3 cards
- **Levels 4-7**: 4 cards
- **Levels 8-10**: 5 cards
- **Level 11+**: 6 cards

### Combat

Combat consists of a repeating cycle of two steps: the player's _attack_ and the creeps' _retaliation_ (see relevant sections below). Both player and creep cards have [abilities](#abilities) that affect combat.

Cards enter combat with full health and mana, after all bonuses from upgrades and passive abilities have been applied. When a card takes damage, it becomes _injured_ and is rotated clockwise for each HP lost—by 90° for cards with 2 maximum HP, and by 45° otherwise. The card is flipped face down when defeated. This also removes any positive or negative effects (known as _buffs_ and _debuffs_ respectively).

Combat ends when all cards on one side have been defeated and cannot be revived. There are two possible outcomes:

- **Victory**. The player proceeds to the rewards phase.
- **Defeat**. The player returns to the preparation phase (training and upgrade research are completed as usual).

Regardless of the outcome, surviving cards have their HP and MP replenished, and the battlefield is cleaned up as follows:

_Heroes and units_

- Defeated cards go to the reserve.
- Surviving peasants are placed face down in the gold mine. They do not contribute to the resource bonus in the next preparation phase; the player must wait until the end of the next round before flipping them again.
- The remaining cards return to the player's hand.

_Creeps_

- Defeated cards are discarded face down in a horizontal pile to the left of the creep pile.
- Surviving cards remain on the battlefield. They are shifted to the left to close any gaps left by defeated creeps.

#### Attack

When combat starts, the player selects a card to attack with (the _attacker_). A different card must be chosen for each subsequent attack until all cards have attacked once. The same _attack rotation_ must be used for the remainder of combat, skipping any cards that have been defeated. It is recommended to reorder the cards to reflect this rotation.

On its turn, a card has one _action_, which must be used either to activate an ability or to perform a _basic attack_ dealing 1 damage to a creep. Regardless of the action taken, heroes deal +1 damage to targets with a value of 4 or lower.

[Player abilities](#player) are divided into three types: _passive_, _active_, and _ultimate_. Active and ultimate abilities consume an action, whereas passive ones do not. Each ultimate ability may be used only once per game. Some abilities are locked until the player reaches a certain level.

While they live, heroes may use any number of items from the player's hand, during any card's turn (see § [Items](#items) for item-specific restrictions). Used items are discarded face up to the left of the item pile. There are three items in total; once all have been used, the discard pile is shuffled to form a new pile.

Some abilities and items can _disable_ one or more creeps, preventing them from retaliating. Unless otherwise specified, this effect lasts for one retaliation.

#### Retaliation

After the player's turn, creeps that have not been defeated or disabled retaliate.

By default, retaliation targets the attacker. However, if the player attacked a boss without defeating or disabling it, the target is determined using the following priority order:

1. A card with 1 HP remaining (if multiple cards qualify, the one with the highest value is selected)
2. The hero, if already injured
3. The attacker

Retaliation deals 1 damage, +1 damage if the combined value of the remaining non-disabled creeps is 20 or more. Additionally, [creep abilities](#creeps) may trigger under certain conditions (provided those creeps are not disabled).

### Rewards

After a victory, the player may earn three types of rewards:

- **Level**. The player levels up by moving the current level card to the bottom of the pile.
- **Resources**. The player draws one resource card.
- **Items**. The player draws one item card for each boss they defeated. If the item pile is empty, the player may not draw from the discard pile. If bosses were defeated during an earlier combat phase but the creeps were only fully cleared later, the player should not forget to draw the corresponding item cards at that time.

## End of the game

The player wins the game when they reach level 13 (K♦). The game is lost if the player is unable to deploy a squad during the recon phase.

### Hard mode

In this optional mode, the game continues until the player loses. To level up beyond level 13, the level pile is reset, with A♦ now representing level 14. The player no longer gains resources during rewards phases.

## Abilities

See § [Combat](#combat) first to fully understand the ability descriptions below (especially concepts like ability types, retaliation, and disabling). 

The type (passive, active, or ultimate) and the mana cost (if any) are specified for each player ability. Some abilities have additional attributes, such as:

- **Magical**. Such abilities cannot be used against magic-immune targets. Magical buffs and debuffs can be dispelled by creeps.
- **Area**. These abilities affect multiple creeps within a designated area. All affected creeps are considered targets. The player may position the area so that part of it extends beyond the battlefield edge, thus hitting fewer creeps.

To help track the effects of abilities marked with an asterisk (*), it is recommended to place jokers on the affected cards. Any small household objects (such as coins, bottle caps, or rubber bands) can serve as substitutes.

### Player

#### Peasant (2/3/4♥)

_Years of war have taught the people of Lordaeron to take up arms in the kingdom's hour of need, joining the regular army as militia._

- **Call to Arms** (passive). Permanently grants the peasant +1 maximum HP.

#### Footman (6♥)

_Backbone of the Lordaeron army, seasoned footmen quickly raise their shield to fend off vicious attacks._

- **Defend** (passive). Grants the footman immunity to creep abilities that are triggered only on the first retaliation. The first damage taken by the footman is reduced by 1.

#### Rifleman (7♥)

_Improved blunderbusses give the stout dwarven riflemen enough range to strike before the enemy can react._

- **Long Rifles** (passive). If the rifleman attacks first, creeps cannot retaliate.

#### Priest (8♥)

_Hailing from Quel'Thalas, priests heal and infuse their allies with holy magic._

- **Heal** (passive). On the priest's turn, heals an injured hero or unit for 1 HP.
- **Inner Fire** (active, 1 MP, magical buff, unlocked at the arcane sanctum) (*). Grants a hero or unit +1 damage on its next basic attack and reduces the next retaliation damage it takes by 1.

#### Sorceress (9♥)

_Elven sorceresses harness arcane energy to bind their enemies in heavy chains—or turn them into sheep._

- **Slow** (passive, magical debuff). On the sorceress's turn, disables a creep of the player's choice.
- **Polymorph** (active, 1 MP, magical debuff, unlocked at the arcane sanctum) (*). Disables the targeted creep until it is damaged.

#### Paladin (J♥)

_Calling on the Light, paladins empower the troops with divine vigor and shield themselves from harm. When the hour is most dire, they bring their fallen comrades back from the dead._

- **Divine Shield** (passive). On the paladin's first turn, grants the paladin immunity to retaliation damage and creep abilities.
- **Devotion Aura** (passive, unlocked at level 4). While the paladin lives, the threshold for the retaliation damage bonus is raised from 20 to 25.
- **Resurrection** (ultimate, 1 MP, unlocked at level 6). Revives up to 2 defeated units with full health and no mana. Resurrected units re-enter the attack rotation in their original order.

#### Archmage (Q♥)

_The archmagi from Dalaran boost their allies' mana reserves and call down ice shards from the skies. As a last resort, they can teleport the troops back to safety._

- **Blizzard** (active, 1 MP, magical, area). Deals 1 damage to each creep in an area 3 cards wide.
- **Brilliance Aura** (passive, unlocked at level 4). While the archmage lives, grants each card in the squad +1 maximum MP.
- **Mass Teleport** (ultimate, 1 MP, unlocked at level 6). Moves the archmage and all surviving units back to the player's hand, ending combat in defeat. [End-of-combat rules](#combat) apply.

#### Mountain king (K♥)

_The dwarven thanes of Khaz Modan wield enchanted weapons to crush their foes. When channeling their ancestral heritage, they enter a state of unstoppable fury._

- **Storm Bolt** (active, 1 MP, magical). Deals 2 damage and disables the targeted creep.
- **Bash** (passive, unlocked at level 4). Basic attacks also disable the targeted creeps.
- **Avatar** (ultimate, 1 MP, unlocked at level 6). Deals 2 damage and disables the targeted creep. For the remainder of combat, the mountain king's basic attacks deal +1 damage.

### Creeps

#### Trapper (5♠)

_Troll trappers have mastered the art of pinning down their prey with heavy nets._

- **Ensnare** (*). When damaged, the trapper casts a net on the attacker. On its next turn, that card cannot attack or use abilities, but still suffers retaliation damage.

#### Bandit (6♠)

_Bandits lurk in the shadows, striking when least expected._

- **Hide**. When combat starts, the bandit is hidden and can only be targeted with area abilities. If not revealed by such an ability, the bandit becomes visible on the first retaliation and deals 1 damage to the attacker (separate from retaliation damage).

#### Assassin (7♠)

_Gnoll assassins coat their bolts with a lethal toxin before battle._

- **Envenomed Weapons** (*). On the first retaliation, the assassin shoots a poisoned bolt at the attacker. The affected card is defeated at the end of its next turn, unless combat ends first.

#### Magi (8♠)

_The two-headed ogre magi incite their comrades to violence by imbuing them with supernatural speed._

- **Bloodlust**. If at least two creeps are currently injured or defeated, creeps retaliate twice. The second retaliation does not trigger creep abilities.

#### Geomancer (9♠)

_Kobold geomancers call upon the power of earth to strip magic from foes and allies alike._

- **Abolish Magic**. At the start of each retaliation, the geomancer dispels 1 magical effect applied by the player, prioritizing as follows: long-lasting debuffs, turn-long debuffs, buffs (e.g., Polymorph &rarr; Slow &rarr; Inner Fire).

#### Golem (10♠)

_The rocky constitution of golems protects them from magic._

- **Spell Immunity**. Grants the golem immunity to magical abilities.

## Items

- **Potion of Healing** (A♥). Heals the hero for 2 HP. This item may only be used if the hero is injured.
- **Ankh of Reincarnation** (A♣). Once obtained, this card must be placed on the hero during recon. When defeated, the hero is immediately revived with 2 HP and no mana, and the item is discarded.
- **Infernal Stone** (A♠). Calls an infernal down from the sky, disabling creeps on impact in an area 2 cards wide. This demon has 2 HP and joins the attack rotation before the hero's turn. It is discarded at the end of combat if it survives.
