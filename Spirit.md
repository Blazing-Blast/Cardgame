# The idea behind Celestials (name WIP)

## Players

There are two playable characters: `Sun` and `Moon`.
Each charater has their own theme and with that, deck, playstyle, and turn structure.

They also start out with $20$ health.
When this is reduced to $0$, the other player wins.

## Phases

Each player will start in their inital phase.

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

1. Draw a card.
2. Play cards annotated with the active phase.
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
Usually this will be along the lines of: "Perform `ACTION` when `CONDITION` is met."

### Creatures

Creatures are summoned on defensively on a lane.

They may maneuver once per turn.
This exhausts them.

### Structures

Structures may only be positioned in the back of a lane.

### Spells

Spells will be activated immediately after being deployed.

## Health

All cards with a health value will start out with that amount of health.
This will be signaled by an amount of health cubes on the card.

Damaging a card will remove an amount of heath cubes from it,
while healing adds them.

If a card's health drops below 0, it dies. This happens immediately.

A card may be healed until above its maximum health,
unless the contrary is specified.

## Board

The board is made up of $4$ sets of lanes.
Each lane has $2 \cdot 3 = 6$ locations:

1. Structure
2. Defence
3. Offence

This makes the board look like:

| Lane / position | 0           | 1         | 2         | 3         | 4         | 5           |
| --------------- | ----------- | --------- | --------- | --------- | --------- | ----------- |
| A               | Structure 1 | Defence 1 | Offence 1 | Offence 2 | Defence 2 | Structure 2 |
| B               | Structure 1 | Defence 1 | Offence 1 | Offence 2 | Defence 2 | Structure 2 |
| C               | Structure 1 | Defence 1 | Offence 1 | Offence 2 | Defence 2 | Structure 2 |
| D               | Structure 1 | Defence 1 | Offence 1 | Offence 2 | Defence 2 | Structure 2 |

By default, a card can only attack cards orthagonally adjacent (`Range`).
A creature in the opponent's defending position,
in a lane that does not have a structure,
may choose to attack their opponent directly.

Creatures can, by default, only maneuver orthogonally,
or, if they are in friendly territory,
they may move to any lane, without changing their position within the lane (`Movement`).
