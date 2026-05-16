# Changelog

## [2.0.0] - 2026-05-16

### Added

- New campaign, the Barrens, featuring orcs as the playable race and a new set of creeps and items
- "Campaign selection" subsection in the setup
- Bonus for each race, called _racial advantage_ 
- Appendix with an overview of all player, creep and item cards across campaigns
- Damage cap (2) for basic attacks with bonus damage
- Creep abilities that inflict damage before retaliation starts
    - If defeated by such an ability, the attacker cannot be the target of retaliation; the remaining player card with the highest value becomes the new target
- "Magical" attribute for some creep abilities
- Guide to reading ability descriptions

### Changed

- Document structure to facilitate the addition of new campaigns
- Human-specific content from the original game (setting, ranks, upgrades, abilities, items) now part of the Lordaeron campaign
- Call to Arms: now the humans' racial advantage (was the Peasant's ability)
- The "Ranks" section now uses campaign-neutral terminology; peasant-type units are referred to as _workers_
- Creep ranks now belong to one of three categories: _low-level_ (2-4), _mid-level_ (5-10), _high-level_ (J/Q/K); high-level creeps are no longer called "bosses"
- Battlefield width increased to 7 cards (up from 6)

### Removed

- "Campaigns" section from the README

### Fixed

- Material list in the introduction (mention of paper clips)
- Internal links to match the new document structure
- Capitalized all card names for increased readability
- Harmonized wording between campaigns
- Rewards area now direction-agnostic (can be on either side of the battlefield)
- If a card cannot attack or use abilities, it is said to "have no action" (since rules specify the action must be used, the previous wording led to unresolvable turns)
- Minor rewording in various places for clarity (no rule changes)

## [1.1.0] - 2026-04-03

### Added

- When researching multiple upgrades in the same building, the card is also rotated 90° as a visual reminder
- Suggestion to use paper clips to mark upgraded cards
- Suggestion to reorder the squad to reflect the attack rotation (to help the player remember it)
- When combat ends, surviving creeps should be shifted to close any gaps left by defeated creeps

### Changed

- The barracks are replaced by the _arcane sanctum_, which provides upgrades for priests/sorceresses instead of footmen/riflemen (see specific changes below)
- The starting hand now includes three non-peasant units (not just the footman and the rifleman); they may be selected freely or randomly
- From level 11 onward, 6 creep cards are drawn instead of 5
- Heroes can use any number of items, during any card's turn (no longer restricted to one item on the hero's turn)
- If targeted, bosses retaliate in a smarter way, prioritizing cards with 1 HP remaining, then injured heroes, then the attacker (instead of always targeting the hero)
- Area abilities now have a fixed width and can extend beyond the battlefield edge to hit fewer targets
- Footman: Defend now unlocked by default, and also reduces by 1 the first damage taken by the footman
- Rifleman: Long Rifles now unlocked by default
- Priest:
    - Heal now passive, and heals for 1 HP (used to be active and heal back to full)
    - Inner Fire now active, increases damage done and reduces damage taken by a card (used to be passive and increase maximum HP)
    - Inner Fire must now be unlocked at the arcane sanctum first
- Sorceress: Polymorph must now be unlocked at the arcane sanctum first
- Paladin: Devotion Aura only available from level 4, now raises the threshold for the retaliation damage bonus from 20 to 25 (instead of capping retaliation damage at 1)
- Archmage: Brilliance Aura only available from level 4
- Mountain king: Bash only available from level 4
- Potion of Healing: now heals for 2 HP (was 1 HP) and may be used only if the hero is injured (to prevent item dumping)
- Ankh of Reincarnation: now used automatically the next time the hero is defeated
- Book of the Dead: replaced by the _Infernal Stone_, which summons a demon with 2 HP that disables two adjacent creeps then joins the attack rotation before the hero

### Removed

- Training grounds and inventory; cards go the hand instead (players can always lay their hand on the play area if they prefer)
- Item tiers (due to item balancing)

### Fixed

- Buildings also have a value, which indicates the cost of the upgrades they provide
- Players must draw a resource card before the game starts (otherwise one card remains after the game is won)
- For better readability, cards that have been damaged (i.e., that are not at full health) are described as _injured_
- Clarified that disabling effects last only for one retaliation (unless otherwise specified)
- Combat ends only if defeated cards cannot be revived
- Bandit: improved description of Hide
- Magi: the second retaliation caused by Bloodlust does not trigger creep abilities (to avoid an infinite retaliation loop)
- Minor rewording in various places for clarity (no rule changes)

## [1.0.1] - 2025-09-10

### Added

- "Campaigns" section in the README, with information about the upcoming expansion 

### Changed

- Updated estimate of average game duration
- Ultimate abilities now unlocked at level 6 (was 8)
- Priest: Heal now restores all HP (was 2 HP)
- Sorceress: Slow now castable on each of the sorceress's turns (was only on the first)
- Paladin: Devotion Aura now caps retaliation damage at 1 (instead of granting a flat HP increase)

### Removed

- "Setting" section from the README

### Fixed

- Clarified how HP/MP bonuses affect current values when gained during combat
- Bandit: Hide damage now explicitly defined as separate from retaliation damage
- Minor rewording in various places for clarity (no rule changes)

