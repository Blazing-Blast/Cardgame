# Sun

`Sun`, she is based on the idea of creation and life.

## Phases

### Dawn

The start of life.
Here she gets to summon creatures, build structures,
and generally become more powerful.

### Noon

The continuation of life.
In this one, she may now activate her creatures.
They finally become useful, and fulfil their purpose.

### Dusk

The end of life.
Her creatures will decay, and structures will rot (take $1$ damage).
During this phase she will be at her most vulnerable.

## Cards

### Creatures

#### Voyager

| Key          | Value      |
| ------------ | ---------- |
| Type         | Creature   |
| Health       | $3$        |
| Attack       | $1$        |
| Movement     | no-exhaust |
| Summon phase | Dawn       |
| Active phase | All        |

When activated: Attack one opponent for `Damage`.

When maneuvered: Move in the default manner, without becoming exhausted.
This is only allowed once per turn.

The Voyager must move to another tile, each turn.
Otherwise, it will take $1$ damage.
It may move by maneuvering, with spells, or via any other manner;
as long as it ends the turn in a different position than last turn.
This means that the Voyager does not need to move on its first turn.

#### Helioler

| Key          | Value    |
| ------------ | -------- |
| Type         | Creature |
| Health       | $2$      |
| Attack       | $-1$     |
| Summon phase | Dawn     |
| Active phase | Noon     |

When activated: Attack one card for `Damage`.
Because it is negative, this will heal.
This _cannot_ heal `Sun` herself, nor the Helioler itself.

#### Red Giant

| Key            | Value       |
| -------------- | ----------- |
| Type           | Creature    |
| Health         | $7$         |
| Attack         | $7$         |
| Movement phase | Dawn + Dusk |
| Summon phase   | Dawn        |
| Active phase   | Noon        |

#### Defender of the Corona

| Key          | Value    |
| ------------ | -------- |
| Type         | Creature |
| Health       | $3$      |
| Attack       | $1$      |
| Shielding    | $2$      |
| Summon phase | Dawn     |
| Attack phase | All      |
| Shield phase | Noon     |

When activated: Either attack or shield. The Defender can only shield during Noon.

When shielding: Choose one allied card.
It will made immune to the first $2$ damage that it will be dealt.
At the start of `Sun`'s next turn, this will be reduced back to $0$.
This exhausts the Defender.

When attacking: Follow the default behavior.

### Structures

#### Ray of Life

| Key          | Value     |
| ------------ | --------- |
| Type         | Structure |
| Health       | $3$       |
| Damage       | $-1$      |
| Summon phase | Dawn      |

Hit all allies in a straight line in the lane the Ray of Life for `Damage`.
Since this is negative, it will result in an increase of health.
This cannot heal above the maximum health of the cards.

These allies are determined by casting a ray,
from the position of the structure, to the opposing side.
The ray only stops when an enemy card is found.
Every card in the ray (except the enemy at the end), will be healed.

#### Gravity Assister

| Key          | Value       |
| ------------ | ----------- |
| Type         | Structure   |
| Health       | $2$         |
| Damage       | $2$         |
| Summon phase | Dawn        |
| Active phase | Noon + Dusk |

##### When activated

Take the card in the defensive position of the Gravity Assister's lane.
It may be exhausted.
It is now called the `Ammo`.
The `Ammo` will now perform a Gravity Assist
towards a offensive position of your choice
in the Gravity Assister's lane.

If there is another card there, it takes `Damage` damage.
This card is now called the `Target`.

The cards trade blows, until one dies.
`Target` gets one free hit if it is not exhausted.
`Target` gets another one if `Ammo` is exhausted.
After these hits, `Ammo` starts trading blows.

This exhausts the `Ammo`, `Target`, and Gravity Assister itself.

#### Suspiciously Wall-shaped Pillar or Light

| Key          | Value     |
| ------------ | --------- |
| Type         | Structure |
| Health       | $5$       |
| Defence      | $1$       |
| Summon phase | Dawn      |

When damaged: reduced damage received by `Defence`.
Damage cannot be reduced below $0$.

#### Mutagenic Ion Beam

| Key          | Value       |
| ------------ | ----------- |
| Type         | Structure   |
| Health       | $3$         |
| Summon phase | Dawn        |
| Active phase | Dawn + Noon |

At the start of your turn, pick a `Target`.
The `Target` will be hit by the Mutagenic Ion Beam, and mutate so that
its attack will be boosted by $1$.
This lasts as long as `Target` is the target of the Beam, and the Beam lives.

### Spells

#### Heat Stroke

| Key           | Value   |
| ------------- | ------- |
| Type          | Spell   |
| Phase         | Noon    |
| Friendly fire | Enabled |

Deal $1$ indiscriminate damage to all cards
within two adjacent or opposing lanes of your choice.

Ignores defence.

#### Coronal Mass Ejection

| Key          | Value |
| ------------ | ----- |
| Type         | Spell |
| Summon phase | All   |
| Active phase | All   |

Ejects `Coronal Mass` in an unoccupied location of your choice.

##### Coronal Mass

| Key          | Value    |
| ------------ | -------- |
| Type         | Creature |
| Health       | $2$      |
| Attack       | $1$      |
| Active phase | All      |

#### Solar Wind

| Key          | Value       |
| ------------ | ----------- |
| Type         | Spell       |
| Active phase | Noon + Dusk |

Pick a lane pair.
All creatures in that lane pair, starting at the opponent's offensive position,
will be pushed one position towards the opponent,
but only if there is a free space for them to move into.

#### Light of (Re)creation

| Key          | Value |
| ------------ | ----- |
| Type         | Spell |
| Active phase | Dawn  |

Pick an opposing card. It is now called the `Original`.
You may clone the card, and place it anywhere in the lane opposing the `Original`.
Your clone has half the health of the `Original`, rounded down, but at least $1$.
