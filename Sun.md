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

| Key          | Value |
| ------------ | ----- |
| Health       | $2$   |
| Attack       | $-1$  |
| Summon phase | Dawn  |
| Active phase | Noon  |

When activated: Attack one ally for `Damage`.
Because it is negative, this will heal.
This _cannot_ heal `Sun` herself.

#### Red Giant

| Key            | Value         |
| -------------- | ------------- |
| Health         | $7$           |
| Attack         | $7$           |
| Movement       | No multi-lane |
| Movement phase | Dawn + Dusk   |
| Summon phase   | Dawn          |
| Active phase   | Noon          |

When maneuvered: Move one space orthogonally. Exhaust.

#### Defender of the Corona

| Key          | Value |
| ------------ | ----- |
| Health       | $3$   |
| Attack       | $1$   |
| Shielding    | $2$   |
| Summon phase | Dawn  |
| Attack phase | All   |
| Shield phase | Noon  |

When activated: Either attack or shield. The Defender can only shield during Noon.

When shielding: Choose one allied card.
It will made immune to the first $2$ damage that it will be dealt.
At the start of `Sun`'s next turn, this will be reduced back to $0$.
This exhausts the Defender.

When attacking: Follow the default behaivour.

### Structures

#### Ray of Life

| Key          | Value |
| ------------ | ----- |
| Health       | $3$   |
| Damage       | $-1$  |
| Summon phase | Dawn  |

Hit all allies in a straight line in the lane the Ray of Life for `Damage`.
Since this is negative, it will result in an increase of health.
This cannot heal above the maximum health of the cards.

These allies are determined by casting a ray,
from the postion of the structure, to the opposing side.
The ray only stops when an enemy card is found.
Every card in the ray (except the enemy at the end), will be healed.

#### Gravity Assister

| Key          | Value       |
| ------------ | ----------- |
| Health       | $2$         |
| Damage       | $2$         |
| Summon phase | Dawn        |
| Active phase | Noon + Dusk |

##### When activated

Take the allied card in the defensive position of the Gravity Assister's lane.
It is now called the `Ammo`
The `Ammo` will now perform a Gravity Assist
towards a position of your choice in the opposing lane.

If there is another card there, it takes `Damage` damage.
This card is now called the `Target`.

And, if it survives, the `Target` gets knocked back to any of the empty spaces next to it
(`Target`'s' owner's choice).
If there are no empty spaces, the cards trade blows, until one dies,
starting with the `Target`.

This exhausts the `Ammo`, and Gravity Assister itself.
If `Target` engaged in combat, it is exhaused, too.

#### Suspiciously Wall-shaped Pillar or Light

| Key          | Value |
| ------------ | ----- |
| Health       | $5$   |
| Defence      | $1$   |
| Summon phase | Dawn  |

When damaged: reduced damage recieved by `Defence`.
Damage cannot be reduced below $0$.

#### Mutagenic Ion Beam

| Key          | Value       |
| ------------ | ----------- |
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
| Phase         | Noon    |
| Friendly fire | Enabled |

Deal $1$ indiscriminate damage to all cards
within two adjacent or opposing lanes of your choice.

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

Ejects `Coronal Mass` in an unoccupied location of your choice.

#### Solar Wind

| Key          | Value       |
| ------------ | ----------- |
| Active phase | Noon + Dusk |

Pick a lane pair. All creatures in that lane pair, starting at the opponent's offensive position,
will be pushed one position towards the opponent,
but only if there is a free space for them to move into.

#### Light of (Re)creation

| Key          | Value |
| ------------ | ----- |
| Active phase | Dawn  |

Pick an opposing card. It is now called the `Original`.
You may clone the card, and place it anywhere in the lane opposing the `Original`.
Your clone has half the health of the `Original`, rounded down, but at least $1$.
