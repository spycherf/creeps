# Creeps (card game)

_Creeps_ is a single-player card game inspired by Warcraft III. It borrows several gameplay elements from [Duel 52](https://juddmadden.com/duel52/) (designed by Judd Madden and Nina Riddell) and from [Mercenaries](https://github.com/spycherf/mercenaries). It requires a standard 52-card French-suited deck, plus 2-3 jokers (or any small household objects as substitutes). A game typically lasts about 20 minutes.

## Setting

The game is set on Azeroth, shortly before the Third War. In the human kingdom of Lordaeron, scattered bands of marauders—dubbed _creeps_ by frightened citizens—have been sighted roaming the countryside, pillaging towns and villages. Troubled by these incursions, King Terenas dispatches his forces to restore order and defend the realm from this growing menace...

## Cards

### Suits

- **Hearts** (♥) = player
- **Diamonds** (♦) = level
- **Spades** (♠)= creeps
- **Clubs** (♣) = resources

Exceptions: A♥, A♠, and A♣ represent lootable items (see § [Rewards](#rewards) and [Items](#items)).

### Ranks

See § [Playing](#playing) and [Abilities](#abilities) for more information on what cards do.

#### Player (♥)

_Units_

- **2/3/4** = peasants
- **6** = footman
- **7** = rifleman
- **8** = priest
- **9** = sorceress

_Heroes_

- **J** = paladin
- **Q** = archmage
- **K** = mountain king

_Buildings_

- **5** = barracks
- **10** = blacksmith

#### Creeps (♠)

- **2/3/4** = murlocs
- **5** = trapper
- **6** = bandit
- **7** = assassin
- **8** = magi
- **9** = geomancer
- **10** = golem
- **J/Q/K** = bosses

### Values

The _value_ of a player card corresponds to the cost of acquiring it, based on its rank:

- **Units** = the card's number
- **Heroes** = 10

For all other suits, values are as follows:

- **Number cards** = the card's number
- **J** = 11
- **Q** = 12
- **K** = 13

The value of creep cards is used to calculate the damage dealt to the player. The value of resource cards represents currency. Finally, level cards, ranging from A♦ (lowest) to K♦ (highest), indicate the player's level from 1 to 13.

Buildings and items have no value.

### Health and mana

Cards that take part in combat have _health_, or _hit points_ (HP), representing the amount of _damage_ they can take before being defeated (1 damage = 1 HP). Face cards have 3 HP and number cards have 2 HP—except peasants, which have only 1 HP.

Cards with abilities that cost mana also have 1 _mana point_ (MP).

Some abilities can increase a card's total HP or MP, but no card may exceed 4 HP or 2 MP. If a bonus is removed, current health or mana is only reduced if it exceeds the new total. For example, a hero with a +1 HP bonus drops from 4/4 HP to 3/3 HP when the bonus is removed. The same card at 3/4 HP would remain at 3/3 HP after the bonus is lost.

## Setup

The play area is divided into sections:

- **Base** (in front of the player):
    - **Buildings** (center). The blacksmith (10♥) and the barracks (5♥) are placed side by side, face up.
    - **Gold mine** (slightly to the left, about 3 inches wide)
    - **Training grounds** (slightly to the right, about 3 inches wide)
    - **Reserve** (to the player's right). Remaining player cards are laid out face up, sorted by rank.
- **Battlefield** (above the base, sized for two rows of five cards)
- **Creeps** (above the battlefield). Creep cards are shuffled and placed face down.
- **Rewards** (to the player's left):
    - **Level** (bottom). Level cards are sorted and placed face up, with A♦ on top.
    - **Resources** (center). Resource cards are shuffled and placed face down.
    - **Items** (top). Item cards are shuffled and placed face down.
- **Inventory** (above the reserve)

Jokers are set aside for later use.

From the reserve, the player draws the footman (6♥), the rifleman (7♥), and one hero of their choice. These form the starting hand.

## Playing

The game is played in rounds. Each round follows the same sequence of phases, each with a clear objective:

1. **Preparation**. Use resources to develop both army and economy.
2. **Recon**. Dispatch forces to the battlefield to locate a creep camp.
3. **Combat**. Defeat the creeps.
4. **Rewards**. Level up and collect resources and items dropped by the creeps.

The player starts the game with no resources.

### Preparation

The player can engage in three activities during this phase: _training_, _upgrading_, _gathering_.

#### Training

The player may use available resources to train heroes and units. The total value of resources spent must be equal to or greater than the combined cost of the selected cards; any excess is lost. Spent resources are discarded face up to the left of the resource pile.

To begin training, selected cards are placed face down on the training grounds. Peasants are placed face down in the gold mine instead, each slightly offset to the right so all cards remain visible.

Cards in training cannot be used. Training ends at the start of the next preparation phase, at which point the cards are flipped face up. Trained cards are added to the hand, except peasants, which stay in the gold mine.

#### Upgrading

The blacksmith (10♥) and the barracks (5♥) can research _upgrades_ for certain units. Blacksmith upgrades cost 10 resources each; barracks upgrades, 5. The rules for spending resources are the same as during training. Each building can research more than one upgrade at a time. While research is in progress, the relevant building is flipped face down. The card is flipped again when research is completed, at the start of the next preparation phase.

The following upgrades are available:

_Blacksmith_

- **Steel Plating**. Grants footmen +1 total HP.
- **Reinforced Leather Armor**. Grants riflemen +1 total HP.

_Barracks_

- **Defend**. Teaches footmen the [Defend](#player) ability.
- **Long Rifles**. Teaches riflemen the [Long Rifles](#player) ability.

#### Gathering

While in the gold mine, each trained peasant (2/3/4♥) generates 1 additional resource per preparation phase. This _resource bonus_ does not accumulate between rounds if unused.

### Recon

In this phase, the player selects a _squad_ of up to three trained cards and places them face up in a row on the battlefield. Peasants are also eligible. Only one hero may be deployed.

If no creeps remain from the previous combat phase, a number of cards determined by the player's level (see below) are drawn from the creep pile and placed face up on the battlefield, in a row starting from the left, facing the player’s squad. If the draw pile is empty, discarded creeps are shuffled to form a new pile.

Number of creeps to draw by level:

- **Level 1** = 2 cards
- **Levels 2-3** = 3 cards
- **Levels 4-7** = 4 cards
- **Level 8+** = 5 cards

### Combat

Combat consists of a repeating cycle of two steps: the player's _attack_ and the creeps' _retaliation_ (see relevant sections below). Both player and creep cards have [abilities](#abilities) that affect combat.

When a card takes damage, it is rotated clockwise for each HP lost—by 90° for cards with 2 total HP, and by 45° otherwise. The card is flipped when defeated. This also removes any positive or negative effects (known as _buffs_ and _debuffs_ respectively).

Combat ends when all cards on one side have been defeated. There are two possible outcomes:

- **Victory**. The player proceeds to the rewards phase.
- **Defeat**. The player returns to the preparation phase.

Regardless of the outcome, surviving cards replenish their HP and MP, and the battlefield is cleaned up as follows:

_Heroes and units_

- Defeated cards go back to the reserve.
- Surviving cards return to the player's hand. Peasants, however, are placed face down in the gold mine instead. They do not contribute to the resource bonus in the next preparation phase. The player must wait until the end of the next round before flipping them again.

_Creeps_

- Defeated cards are discarded face down in a horizontal pile to the left of the creep pile.
- Surviving cards remain on the battlefield.

#### Attack

When combat starts, the player chooses a card to attack with (the _attacker_). A different card must be chosen for each subsequent attack until all cards have attacked once. The same attack rotation must then be followed for the remainder of combat, skipping any cards that have been defeated.

On its turn, a card has one _action_, which must be used either to activate an ability or to perform a _basic attack_ dealing 1 damage. Regardless of the action taken, heroes deal +1 damage to targets with a value of 4 or lower.

[Player abilities](#player) are divided into three types: _active_, _passive_, and _ultimate_. Active and ultimate abilities consume an action, whereas passive ones do not. Ultimate abilities are unlocked at level 8 and may be used only once per game.

At any time during their turn, heroes may also use one [item](#items) from the inventory. This does not consume their action. Used items are discarded face up to the left of the item pile. There are three items in total; once all have been used, the discard pile is shuffled to form a new item pile.

#### Retaliation

In response to the player's attack, creeps retaliate for 1 damage. If the combined value of the remaining creeps is 20 or more, they deal +1 damage. When defeated or _disabled_ (by abilities like Polymorph), creeps cannot retaliate and are therefore excluded from this value check.

By default, retaliation damage targets the attacker. However, if the player targeted a boss without defeating or disabling it, the damage is directed at the card with the highest value instead.

[Creep abilities](#creeps) may trigger during retaliation under certain conditions. Defeated or disabled creeps cannot use their ability.

### Rewards

After a victory, the player may earn three types of rewards:

* **Level**. The player levels up by moving the current level card to the bottom of the pile.
* **Resources**. The player draws one resource card.
* **Items**. For each boss they defeated, the player draws one item card and places it face up in the inventory. If the item pile is empty, the player may not draw from the discard pile. If bosses were defeated during an earlier combat phase but the creeps were only fully cleared later, the player should not forget to draw the corresponding item cards at that time.

## End of the game

To win the game, the player must reach level 13 (K♦). The game is lost if the player is unable to deploy a squad during the recon phase.

### Hard mode

In this optional mode, the game continues until the player loses. To level up beyond level 13, the level pile is reset, with A♦ now representing level 14. The player no longer gains resources during rewards phases.

## Abilities

See § [Combat](#combat) first to fully understand the ability descriptions below (especially concepts like ability types, retaliation, and disabling). 

The type (active, passive, or ultimate) and the mana cost (if any) are specified for each player ability. Some abilities have additional attributes, such as:

- **Magical**. They cannot be used against magic-immune targets. Magical buffs and debuffs can be dispelled by creeps.
- **Area**. They affect multiple creeps within a designated area. All affected creeps are considered targets.

To visually track the effects of abilities marked with an asterisk (*), it is recommended to place jokers on the affected cards. Any small household objects (such as coins, bottle caps, or rubber bands) can serve as substitutes.

### Player

#### Peasant (2/3/4♥)

_Years of war have taught the people of Lordaeron to take up arms in the kingdom's hour of need, joining the regular army as militia._

- **Call to Arms** (passive). Grants peasants +1 total HP.

#### Footman (6♥)

_Backbone of the Lordaeron army, seasoned footmen quickly raise their shield to fend off vicious attacks._

- **Defend** (passive, unlocked at the barracks). Grants immunity to abilities triggered the first time creeps retaliate.

#### Rifleman (7♥)

_Improved blunderbusses give the stout dwarven riflemen enough range to strike before the enemy can react._

- **Long Rifles** (passive, unlocked at the barracks). If the rifleman attacks first, creeps cannot retaliate.

#### Priest (8♥)

_Hailing from Quel'Thalas, holy priests bless their allies before battle and heal them during combat._

- **Inner Fire** (passive, magical buff). Before combat starts, grants an ally or the priest +1 total HP.
- **Heal** (active, 1 MP). Heals an ally or the priest for 2 HP.

#### Sorceress (9♥)

_Elven sorceresses harness arcane energy to bind their enemies in heavy chains—or turn them into sheep._

- **Slow** (passive, magical debuff). On the sorceress's first turn, disables a creep of the player's choice.
- **Polymorph** (active, 1 MP, magical debuff) (*). Disables the targeted creep until it is damaged.

#### Paladin (J♥)

_Calling on the Light, paladins empower their allies with divine vigor and shield themselves from harm. When the hour is most dire, they bring their fallen comrades back from the dead._

- **Devotion Aura** (passive). Grants the squad +1 total HP while the paladin lives.
- **Divine Shield** (passive). The first time the paladin attacks, grants immunity to retaliation damage and creep abilities targeting the paladin.
- **Resurrection** (ultimate, 1 MP). Revives up to 2 defeated units with full health and no mana. Resurrected units re-enter the attack rotation in their original order.

#### Archmage (Q♥)

_The archmagi from Dalaran boost their allies' mana reserves and call down ice shards from the skies. As a last resort, they can teleport the troops back to safety._

- **Brilliance Aura** (passive). Grants the squad +1 total MP while the archmage lives.
- **Blizzard** (active, 1 MP, magical, area). Deals 1 damage to each creep in an area up to 3 cards wide.
- **Mass Teleport** (ultimate, 1 MP). Moves the archmage and all surviving units back to the player's hand, ending combat in defeat. [End-of-combat rules](#combat) apply.

#### Mountain king (K♥)

_The dwarven thanes of Khaz Modan wield enchanted weapons to crush their foes. When channeling their ancestral heritage, they enter a state of unstoppable fury._

- **Bash** (passive). Basic attacks also disable the targeted creeps.
- **Storm Bolt** (active, 1 MP, magical). Deals 2 damage and disables the targeted creep.
- **Avatar** (ultimate, 1 MP). Deals 2 damage and disables the targeted creep. For the remainder of combat, the mountain king's basic attacks deal +1 damage.

### Creeps

#### Trapper (5♠)

_Troll trappers have mastered the art of pinning down their prey with heavy nets._

- **Ensnare** (*). When damaged, the trapper casts a net on the attacker. On its next turn, that card cannot attack or use abilities but still suffers retaliation damage. Heroes may still use items while ensnared.

#### Bandit (6♠)

_Bandits lurk in the shadows, striking when least expected._

- **Hide**. The bandit cannot be targeted until the first time creeps retaliate, at which point he deals 1 damage to the attacker. This damage can be prevented by revealing the bandit early with area abilities.

#### Assassin (7♠)

_Gnoll assassins coat their bolts with a lethal toxin before battle._

- **Envenomed Weapons** (*). The first time creeps retaliate, the assassin shoots a poisoned bolt at the attacker, killing it at the end of its next turn unless combat ends first.

#### Magi (8♠)

_The two-headed ogre magi incite their comrades to violence by imbuing them with supernatural speed._

- **Bloodlust**. Creeps retaliate twice if two or more are not at full health (including defeated cards).

#### Geomancer (9♠)

_Kobold geomancers call upon the power of earth to strip magic from foes and allies alike._

- **Abolish Magic**. At the start of each retaliation, the geomancer dispels 1 magical effect applied by the player, prioritizing as follows: long-lasting debuffs, turn-long debuffs, buffs.

#### Golem (10♠)

_The rocky constitution of golems protects them from magic._

- **Spell Immunity**. Grants the golem immunity to magical abilities.

## Items

Each item has an associated tier. Higher tiers offer greater power and utility.

- Tier 1: **Potion of Healing** (A♥). Heals the hero for 1 HP.
- Tier 2: **Ankh of Reincarnation** (A♣). Brings the hero back to life with 2 HP and no mana. If the hero was defeated during another card's turn, this item may be used at the start of the hero's next turn.
- Tier 3: **Book of the Dead** (A♠). Summons a skeleton with 1 HP (cannot be modified by bonuses). It immediately deals 1 damage to a target. If summoned before the hero’s attack, the hero avoids retaliation. If summoned after, the skeleton avoids retaliation on its initial strike, then joins the attack rotation, following the usual [attack](#attack) and [retaliation rules](#retaliation). The skeleton is discarded at the end of combat if it survives.
