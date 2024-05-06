# The idea behind Celestials (name WIP)

Note that any rules regarding card behaviour outlined here
may be overwritten by the cards and phases themselves.
This will be explicitly mentioned.

## Players

There are two playable characters: `Sun` and `Moon`.
Each charater has their own theme and with that, deck, playstyle, and turn structure.

They also start out with $20$ health and 5 cards in their hand.

When a player's health is reduced to $0$, the other player wins.

## Phases

Each player will start in their initial phase.

They may advance a phase by playing a card that allows them to.
These cards may _only_ allow for _forward_ movements.
Playing one of these cards will end your turn.
Trying to advance from the final phase, will result in looping back to the inital phase.

Phases will follow the general structure of

1. Setup
2. Damage
3. Falloff

## Turns

Each turn follows the following structure:

1. Draw a card. (Max 5)
2. Play, activate, and maneuver cards who's requirements are met.
3. Play an `Advance Phase` card.
4. Discard and draw a card.

Each step is optional.

## Cards

There are different card types:

- Creatures
- Structures
- Spells

During the player's `Damage` phase, their deployed card may be activated
as long as it is not exhaused.

What this entails will be specified on the card.
If it is not specfied, the card may damage any orthogonally neighbouring card for their `Damage` stat.

Being activated always exhausts the card, unless the contrary is specified.

### Creatures

Creatures are summoned on defensively on a lane.

They may maneuver once per turn.
This exhausts them.

### Structures

Structures may only be positioned in the back of a lane.

### Spells

Spells will be activated immediately after being deployed.

## Card Piles

Each deck contains 3 `Advance Phase` cards,
and two copies of each card in their `PlayerName.md` file.

The are three card piles:

- Draw pile
- Discard pile
- Graveyard

At the start of the game, the entire deck is shuffeled, and placed onto the draw pile.

When a card is discarded, it moves to the discard pile.

When a card's health drops to $0$ or it is a played spell, it is moved to the graveyard.

When both draw piles are emptied,
the players may decide to shuffle their discard piles into their draw piles.
They must both agree to this.
The decision must be made right after the last card is drawn.
It is final.

Note that cards in the graveyard, stay in the graveyard, during this process.

When a player's draw and discard pile is empty, they can no longer draw cards.

## Health

All cards with a health value will start out with that amount of health.
This will be signaled by an amount of health cubes on the card.

There are red health cubes (worth 1),
and green ones, with a value of 5.

Damaging a card will remove an amount of health cubes from it,
while healing adds them.

If a card's health drops below 0, it dies. This happens immediately, unless the contrary is specified.

A card may be healed until above its maximum health,
unless the contrary is specified.

## Board

The board is made up of $4$ pairs of lanes.
Each lane pair has $2 \cdot 3 = 6$ locations:

1. Structure
2. Defence
3. Offence

This makes the board look like:

| Lane / position | 0           | 1         | 2         | 3         | 4         | 5           |
| --------------- | ----------- | --------- | --------- | --------- | --------- | ----------- |
| A1 + A2         | Structure 1 | Defence 1 | Offence 1 | Offence 2 | Defence 2 | Structure 2 |
| B1 + B2         | Structure 1 | Defence 1 | Offence 1 | Offence 2 | Defence 2 | Structure 2 |
| C1 + C2         | Structure 1 | Defence 1 | Offence 1 | Offence 2 | Defence 2 | Structure 2 |
| D1 + D2         | Structure 1 | Defence 1 | Offence 1 | Offence 2 | Defence 2 | Structure 2 |

By default, a card can only attack cards orthagonally adjacent. (`Range`)

A creature in the opponent's defending position,
in a lane that does not have a structure,
may choose to attack their opponent directly.

Creatures can, by default, only maneuver orthogonally
Or, if they are in friendly territory,
they may move to any lane, without changing their position within the lane. (`Movement`)

Creatures may not maneuver to occupied locations.
