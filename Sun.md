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
They finaly become useful, and fullfil their purpose.

### Dusk

The end of life.
Her creatures will decay, and structures will rot (take $1$ damage).
During this phase she will be at her most vulnerable.

## Cards

### Creatures

#### Wanderer

| Key          | Value      |
| ------------ | ---------- |
| Health       | $3$        |
| Attack       | $1$        |
| Movement     | no-exhaust |
| Summon phase | Dawn       |
| Active phase | All        |

When activated: Attack one opponent for `Damage`.

When maneuvered: Move in the default manner, without becoming exhausted.
This is only allowed once per turn.

The Wanderer must move to another tile, each turn.
Otherwise, they will take $1$ damage.
They may move by maneuvering, with spells, or via any other manner;
as long as they end the turn in a different position than last turn.
This means that they do not need to move on their first turn.

#### Healer

| Key          | Value |
| ------------ | ----- |
| Health       | $2$   |
| Attack       | $-1$  |
| Summon phase | Dawn  |
| Active phase | Noon  |

When activated: Attack one ally for `Damage`.
Because it is negative, it will heal.
This _cannot_ heal `Sun` herself.

#### Urayuli

| Key            | Value         |
| -------------- | ------------- |
| Health         | $7$           |
| Attack         | $7$           |
| Movement       | No multi-lane |
| Movement phase | Dawn + Dusk   |
| Summon phase   | Dawn          |
| Active phase   | Noon          |

When maneuvered: Move one space orthogonally. Exhaust.

#### Guardian

| Key          | Value       |
| ------------ | ----------- |
| Health       | $3$         |
| Attack       | $1$         |
| Summon phase | Dawn        |
| Active phase | Noon + Dusk |

When activated: Choose one allied card.
They will be immune to the first $2$ damage that they will be dealt, this turn.

### Structures

#### Sanctuary

| Key          | Value |
| ------------ | ----- |
| Health       | $3$   |
| Summon phase | Dawn  |

Passively heal all allies in a straight line from the Sanctuary for $1$.
This cannot heal above the maximum health of the card.

These enemies are determined by casting a ray from the Sactuary.
The ray only stops when an enemy card is found.
Every card in the ray (except the enemy at the end), will be healed.

#### Catapult

| Key          | Value |
| ------------ | ----- |
| Health       | $2$   |
| Damage       | $2$   |
| Summon phase | Dawn  |
| Active phase | Noon  |

##### When activated

Take the allied card in the defensive position of the Catapunt's lane.
It is now called the `Ammo`
Launch the `Ammo` to any position in the opposing lane.

If there is another card there, it takes `Damage` damage.
This card is now called the `Target`.

And, if it survives, it gets knocked back to any of the empty spaces next to it
(the `Target`'s' owner's choice).
If there are no empty spaces, the cards trade blows, until one dies,
starting with the `Target`.

This exhausts the `Ammo`, `Target`, and Catapult.

#### Suspiciously Wall-shaped Pillar or Light

| Key          | Value |
| ------------ | ----- |
| Health       | $5$   |
| Defence      | $1$   |
| Summon phase | Dawn  |

When damaged: reduced damage recieved by `Defence`.
Damage cannot be reduced below $0$.

#### Ray of Power

| Key          | Value       |
| ------------ | ----------- |
| Health       | $3$         |
| Summon phase | Dawn        |
| Active phase | Dawn + Noon |

When activated: Choose one allied card.
Its attack will be boosted by $1$, until a new target is chosen, or the Beacon is destroyed.

### Spells

#### Heat Stroke

| Key           | Value   |
| ------------- | ------- |
| Phase         | Noon    |
| Friendly fire | Enabled |

Deal $1$ indiscriminate damage to all cards within two adjacent lanes.

#### Coronal Mass Ejection

| Key          | Value |
| ------------ | ----- |
| Summon phase | All   |
| Active phase | All   |

##### Coronal Mass

| Key          | Value |
| ------------ | ----- |
| Health       | $2$   |
| Attack       | $1$   |
| Active phase | All   |

Ejects `Coronal Mass` in an unoccupied position in a lane of your choice.

#### Solar Wind

| Key          | Value       |
| ------------ | ----------- |
| Active phase | Noon + Dusk |

Pick a lane. All creatures in that lane, starti`ng at the opponent's offensive position,
will be pushed one position towards the opponent,
but only if there is a free space for them to move into.

#### Virility Beam

| Key          | Value |
| ------------ | ----- |
| Active phase | Dawn  |

Pick an opposing card. It is now called the `Original`.
You may clone the card, and place it anywhere in the lane opposing the `Original`.
Your clone has half the health of the `Original`, rounded down, but at least $1$.
