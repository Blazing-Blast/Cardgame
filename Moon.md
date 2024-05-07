# Moon

`Moon`, on the other hand, tends towards destruction.

## Phases

### Waxing

This signals incoming destruction.
During this phase he can tag enemy creatures and buildings for destruction.

### Plenilune

The peak of his power.
Now is his moment to dish out damage to tagged enemies.

### Waning

Now, is the time for restoration.
The tagged enemies that survived, will heal $1$ hitpoint.

## Tagging

Any card with `Tagging = Enabled` will tag the card it attacks.
This is indicated by placing a blue Tag Cube onto the card.

When entering the Waxing phase, clear all tags.

## Cards

### Creatures

#### Spy

| Key          | Value              |
| ------------ | ------------------ |
| Health       | $1$                |
| Attack       | $3$                |
| Summon phase | Waxing + Plenilune |
| Active phase | Waxing + Waning    |
| Tagging      | First hit          |
| Hidden       | First hit          |

The Spy is hidden (unable to be targeted by the enemy),
until he performs his first attack, or is damaged.

This de-cloaking attack tags the enemy.

The Spy can only attack during `Active Phase`.

#### Blutsauger

| Key          | Value              |
| ------------ | ------------------ |
| Health       | $2$                |
| Defence      | $1$                |
| Attack       | $1$                |
| Summon phase | Waxing + Plenilune |
| Active phase | Waxing             |
| Tagging      | Enabled            |

When Blutsauger kills a creature: restore $1$ health.
This may go above its maximum health.

#### Rock Thrower

| Key          | Value              |
| ------------ | ------------------ |
| Health       | $3$                |
| Attack       | $1$                |
| Range        | $2$                |
| Summon phase | Waxing + Plenilune |
| Active phase | Waxing             |
| Tagging      | Enabled            |

You may only attack cards that can be reached via two orthogonal moves.

#### Kessler

| Key          | Value           |
| ------------ | --------------- |
| Health       | $2$             |
| Attack       | $1$             |
| Energy       | $2$             |
| Summon phase | Waxing + Waning |
| Active phase | All             |
| Target       | Tagged only     |

Kessler may attack or maneuver `Energy` times before getting exhausted.

When killing a card: Kessler's can make another `Energy` moves, this turn.

### Structures

#### Cheese

| Key          | Value              |
| ------------ | ------------------ |
| Health       | $4$                |
| Damage       | $1$                |
| Summon phase | Plenilune + Waning |
| Active phase | All                |

When activated: Pick any adjacent card. It is now called `Consumer`.
The `Consumer` will heal for `Damage`, and Cheese will take that much Damage.
The consumer cannot heal above its initial health.
No exhaust.

#### Death Ray

| Key          | Value              |
| ------------ | ------------------ |
| Health       | $2$                |
| Damage       | $1$                |
| Summon phase | Waxing             |
| Active phase | Waxing + Plenilune |

When activated: Deal `Damage` damage
to all cards in the lane pair the Death Ray is located in, except itself.

If Death Ray has not been activated, by the end of the turn,
it takes $1$ self-damage.

#### Altar

| Key            | Value |
| -------------- | ----- |
| Health         | $1$   |
| Shield         | $1$   |
| Defence        | $1$   |
| Damage         | $1$   |
| Summon Phase   | All   |
| Activate Phase | All   |

The Altar may be activated by any card in the defending position front of it.
This card does not have to be allied.
This card will not get exhausted by this, but the Altar will.

##### When activated during Waxing

Tag the first `Damage` cards in the altar's lane pair.

Determine these by casting a ray,
from the altar's location,
towards the opposing structure position,
the first `Damage` cards encountered will be tagged.

##### When activated during Plenilune

Deal `Damage` damage to the **last** `Damage` enemies opposing it.

##### When activated during Waning

Heal the **last** `Damage` enemies opposing it for `Damage` hitpoints.

##### When hit

First, the damage will be reduced by `Defence`.
Then, the first `Shield` damage will be ignored, each turn.

It has no shielding during the `Waning` phase.

### Spells

#### Terminal Impact

| Key          | Value        |
| ------------ | ------------ |
| Damage       | $2$          |
| Range        | $3 \times 3$ |
| Target       | Tagged only  |
| Active phase | All          |

Deal `Damage` damage to all tagged enemies in a `Range`-sized area of your choice.

#### Bounce

| Key          | Value            |
| ------------ | ---------------- |
| Target       | All tagged cards |
| Active phase | All              |

Push all `Target`s one tile towards a direction of your choice.
All other cards stay still.

If a `Target` collides with a non-`Target` card, neither will move.

#### Ebb and Flow

| Key          | Value |
| ------------ | ----- |
| Active phase | All   |

Pick a card with non-zero `Health` and `Damage` stats, and swap them.

#### Erupt

| Key          | Value              |
| ------------ | ------------------ |
| Active phase | Waxing + Plenilune |

Summon a `Mare` in any allied location.

##### Mare

| Key    | Value |
| ------ | ----- |
| Health | $1$   |
| Damage | $2$   |
| Target | Enemy |

Deals `Damage` points of damage to any enemy card that attempt to maneuver to its location.
This deals $2$ self-damage.

If both the Landmine and enemy survive,
the enemy moves back to where it came from.
