# OUTBRAVE

> Case study of implementing hearthstone clone in dark fantasy style in classic, progression and rebalanced mode

## Goals

- art style should be using dark fantasy elements instead of dull fantasy as original was
- for all classes and mechanics use different names and keywords
- in classic mode implement all heroes minions and spells in same way as original latest patch of version 1.0
- do not implement Shaman hero class as it is only one that has randomized hero ability

## Roadmap

- basic rendering and target selection without dragging, no font rendering, use textures for cards (base, image portrait, text image, etc ) and numbers for health, armour and attack
- classic mode with only 2 heroes, pre-build two decks with class specific and neutral cards, selecting hero and play with bot via local server
- main menu of grid 3x3 with center square occupied by **Play** button, on diagonal squares male classes, on side squares girl classes
- implement 2 more heroes with pre-build decks up to maximum of 8 heroes
- implement other cards in steps of 20% each time up to 80% of total original card pool (leave the most difficult to the end)
- implement progression classic mode of climbing (see [progression](#progression))
- implement all remaining classic cards and ability to create custom decks
- implement dark fantasy art style
- implement rebalance mode (see [rebalanced](#rebalanced))
- graphics overhaul

## Classes

Grid row:col position on hero selector menu (2:2 **Play** button):

- `Assassin (girl, grid 3:2, original Rogue)`
- `Champion (male, grid 1:1, original Paladin)`
- `Conjurer (male, grid 3:3, original Warlock)`
- `Evocator (male, grid 3:1, original Druid)`
- `Huntress (girl, grid 2:1, original Hunter)`
- `Magician (girl, grid 2:3, original Mage)`
- `Sentinel (male, grid 1:3, original Warrior)`
- `Shepherd (girl, grid 1:2, original Priest)`

## Classic

Mode that allow to play with classic cards against bots (and later other players via server connection) something like casual play.

## Progression

Specific Ranked mode that players could choose deck only from pre-constructed decks for each class and compete with each other until they reach specific rank where they can construct own custom decks.

**Progression** is split into this categories (with pre-constructed decks limitations):

- `junior (up to 1 legendary, up to 4 epic, up to  8 rare cards)`
- `middle (up to 2 legendary, up to 6 epic, up to 12 rare cards)`
- `senior (up to 4 legendary, up to 8 epic cards)`
- `legend (up to 8 legendary cards)`
- `custom (no restrictions, custom decks)`

Ideally, each category should have 8 different pre-constructed decks per class, resulting in total of 256 decks.

## Rebalanced

A specific game mode with modified hero abilities, game rules and cards.
This format aims to make the game even quicker than the original.

Main changes:

- All hero powers cost 1 mana
- Maximum of 8 mana crystals
- Maximum of 8 cards in hand
- A player who cannot draw any more cards immediately loses
- Total card pool is 256 cards, 24 cards per hero, 64 neutral cards
- On first turn player have only 8 seconds to complete their turn; this increases by 8 seconds each turn, up to a maximum of 64 seconds when 8 mana crystals are available.

###### each folder MAY contain README with additional information about project
