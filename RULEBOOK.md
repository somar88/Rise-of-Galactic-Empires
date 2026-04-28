# RoGEs — Rule Book

> *A space-empire strategy board game of exploration, conflict, production, and galactic domination.*

---

## Table of Contents

1. [Overview](#overview)
2. [Victory Conditions](#victory-conditions)
3. [Components](#components)
   - [Cards](#cards)
   - [Space Units](#space-units)
   - [Ground Units](#ground-units)
   - [Structures](#structures)
   - [Dice](#dice)
4. [Game Setup](#game-setup)
   - [Galaxy Setup](#galaxy-setup)
   - [Player Setup](#player-setup)
5. [The Game Round](#the-game-round)
6. [Player Action Phase](#player-action-phase)
   - [Production](#production)
   - [Mobilization](#mobilization)
   - [Civilian Actions](#civilian-actions)
   - [Exchange](#exchange)
7. [Conflict Phase](#conflict-phase)
   - [Space Battle](#space-battle)
   - [Landing](#landing)
   - [Ground Battle](#ground-battle)
   - [Retreat from Conflict](#retreat-from-conflict)
   - [Between Battles](#between-battles)
8. [Maintenance Phase](#maintenance-phase)
9. [Exploration & Colonization](#exploration--colonization)
10. [Politics & Alliances](#politics--alliances)
11. [Hand Size](#hand-size)
12. [Design Notes & To Do](#design-notes--to-do)

---

## Overview

RoGEs is a galactic empire-building board game for multiple players. Each player controls an interstellar empire competing to dominate the galaxy through exploration, colonization, production, diplomacy, and military conquest. Empires expand across a randomly generated hexagonal galaxy map, managing resources, fleets, and ground forces across multiple star systems.

The game is played in rounds, each consisting of a **Player Action Phase**, a **Conflict Phase**, and a **Maintenance Phase**, until one or more victory conditions are met.

---

## Planet & System Control

Before the win conditions, it is important to understand how **control** works in RoGEs.

### Planet Control
A planet is controlled by the player who has its **planet card on their tableau**. A player gains a planet card by successfully colonizing that planet. A player loses a planet card when an enemy wins a ground battle on that planet and has surviving units remaining there — the card transfers to the victor's tableau.

### Star System Control
A star system is **fully controlled** by a player if:
- They hold **all** planet cards from that system on their tableau, and
- No enemy units remain on any planet in that system.

Partial control does not count — if an enemy still occupies even one planet in a system, that system is contested and belongs to no one.

### Anomaly Hexes
**Space Anomaly** hexes (nebulae, black holes, etc.) contain no planets and cannot be controlled. They are excluded from all control calculations. Having units in an anomaly hex does not count as controlling it.

---

## Victory Conditions

There are three ways to win:

### Moral Win
Have the **Nepiru planet card** on your tableau at the end of **3 consecutive Maintenance Phases**.

- Nepiru is the central galactic planet and is present on the map from the start of the game.
- Any player can contest control at any time by attacking and winning a ground battle there.
- If your hold is broken before 3 consecutive rounds are completed, the counter resets.

#### Nepiru — The Ancient World

Nepiru is no ordinary planet. An ancient, long-dead civilization once inhabited it, leaving behind extraordinarily efficient automation and infrastructure that still functions to this day. No one knows what happened to them — but their legacy makes Nepiru the most powerful and coveted world in the galaxy.

**Golden Districts:**
- Nepiru has a fixed number of **Golden Districts** — advanced, self-sustaining production zones left by the ancient civilization.
- Each Golden District is **flexible** — the controlling player chooses what resource type it produces (CG, IG, or Eco) and may change this when they gain control of the planet.
- All production from Nepiru's Golden Districts is **multiplied by two** — the ancient automation makes them twice as efficient as any normal district.

> **⬜ TODO:** Define the number of Golden Districts on Nepiru — how many does it have?

**The Nepiru Arc:**
- Nepiru has a unique **exclusive Story Arc** that can only be accessed by the player who holds its planet card.
- The arc represents uncovering the mystery of the ancient civilization and unlocking the secrets they left behind.
- When a player first gains control of Nepiru, they draw the Nepiru Arc Starter card and may choose to begin the arc.
- **If Nepiru is conquered**, the arc transfers to the new owner — they continue from exactly where the previous player left off. Earlier choices made by the previous owner are locked in and cannot be changed.
- This means conquering a well-progressed Nepiru arc could put you close to a powerful ending — or leave you inheriting the consequences of someone else's bad choices.

> **⬜ TODO:** Design the Nepiru Story Arc — what is the narrative of the ancient civilization? How many steps does the arc have? What are the possible endings and rewards?

### Strategic Win
**Fully control one-third or more** of all star system hexes in the galaxy (rounded up).

- This condition is only **checked at the end of a Maintenance Phase** in which all hex tiles have been explored, or only anomaly tiles remain unexplored.
- The total number of colonizable systems is not known until the galaxy is fully revealed — so the one-third threshold shifts as exploration progresses.
- Only **fully controlled** systems count (see Planet & System Control above).
- Anomaly hexes are excluded from the total system count.

> **⬜ TODO:** Define how anomaly tiles are set up and identified — are they distinguishable from the back of the tile stack at game start, or are they only discovered when explored? This affects when players know the final galaxy size.

### Annihilation Win
Your empire (and any allies) are declared winners when **no non-allied empire holds any planet cards**.

**Elimination:**
- A player is eliminated the moment they lose their **last planet card** — regardless of how many fleets or units they still have on the map.
- Remaining fleets and units of an eliminated player persist on the map but have no territory and the player is out of the game.

**Conquered Planets:**
- When a player wins a ground battle, they take the planet card immediately and the enemy population is halved (rounded down), removed in order of most expensive first: IG → Eco → CG. Surviving pops stay and produce for the new owner. See *After a Ground Battle is Won* under Ground Battle for full details.

**Shared Victory:**
- The Annihilation Win belongs to the **entire alliance**, not a single player. If you and your allies together hold all remaining planet cards and no non-allied empire has any planets left, all allied players win together.
- A solo player with no allies wins alone if they annihilate all other empires.

---

### Simultaneous Victory Conditions

If multiple players meet a victory condition in the same Maintenance Phase:

- **Annihilation Win always takes priority** — if a player or alliance has eliminated all non-allied empires, the game ends immediately and they are the sole winners, regardless of any other conditions being met simultaneously.
- **All other win conditions** — if two or more players meet a Moral or Strategic Win condition in the same Maintenance Phase, all qualifying players are declared **joint winners** and the game ends.
- **Optional continuation** — if the players prefer a single winner and are willing to keep playing, they may mutually agree to continue the game rather than accept a joint victory.

---

## Components

### Cards

#### Empire Cards
An Empire Card deck is the combination of all starting **Action Cards** and any **Lore Cards** collected throughout the game. It is used as the player's action deck each round.

> Note: Planet, Moon, and Giant Planet cards are **not** considered Empire Cards.

#### Starting Action Cards
Each player begins with a starting deck of **12 cards**:

- **4× Mobilization** cards
- **3× Production** cards
- **4× Civilian** cards
- **1× Exchange** card

Plus additional **Lore Cards** depending on the empire chosen.

#### Planet Cards
Each star system contains habitable or industrial planets represented by cards. There are three types:

- **Planets** — Standard habitable/industrial worlds
- **Moons** — Smaller bodies with their own properties
- **Giant Planets** — Large planets with unique effects

When a star system is explored, the discovering player draws cards from the corresponding planet-type decks and places them face-up next to the galaxy map. Each card may trigger reveal effects, apply permanent events, or add resources to the planet.

> **⬜ TODO:** Define **Moon** card properties — what makes moons different from regular planets? Do they have districts? Can they be colonized? What unique effects can they have?

> **⬜ TODO:** Define **Giant Planet** card properties — what are their unique effects? Can they be colonized? Do they have special strategic value?

> **⬜ TODO:** Define how many cards are in each planet deck (Planets, Moons, Giant Planets). What is the total deck size per type?

#### Other Card Types

- **Lore Cards** — Empire-specific cards collected during the game
  > **⬜ TODO:** Define the full set of Lore Cards for each empire. How are they acquired? Are they purchased, drawn, or earned through play? How many lore cards does each empire start with?

- **Chaos Cards** — Drawn when maintenance costs cannot be paid
  > **⬜ TODO:** Define the full set of Chaos Card effects. What kinds of consequences can chaos events produce?

- **Resources**
  > **⬜ TODO:** Define the three resource types in detail — Consumer Goods (CG), Industrial Goods (IG), and Eco. What are their exact roles in the economy? Are there Rare Resources? What are Extra Deposits?

---

#### Event Cards

Event cards are drawn during **planet exploration**. They all come from a single unified Event Card deck. Each card is self-contained and tells you exactly what type it is and what your options are.

There are three types of event card outcomes:

**1. Immediate Event**
Resolve it right away — no choice involved. The effect simply happens (gain resources, lose a unit, trigger a battle, etc.) and the card is discarded.

**2. Choice Event**
The card presents two or more options. Each option has a cost or consequence. Pick one, resolve it, discard the card. For example:
- *Option 1: Lose 2 IG — gain 1 extra Scout unit*
- *Option 2: Pay nothing — gain nothing, discard*

**3. Arc Starter**
The card begins a **Story Arc** — a branching narrative sequence unique to your empire. When you draw an Arc Starter, the card gives you a choice:
- **Commit to the Arc** — meet the entry condition (pay resources, have a required unit, etc.) and place the card at your tableau. The card references a numbered group of Arc cards you pull from the box.
- **Take the quick reward** — take a small immediate benefit and discard the card without starting the arc.
- **Decline** — pay a small penalty or simply discard with no benefit.

---

#### Story Arcs

A Story Arc is a private branching narrative your empire pursues over multiple rounds. It is separate from your empire deck and tracked next to your tableau.

**Progressing an Arc:**
- Advancing a Story Arc is one of the options available under the **Civilian Action**.
- Each time you progress, you read the current Arc card, pick an option, pay the cost, and move to the next referenced card number.
- You draw the next card from the Arc's dedicated group (pulled from the box at the start of the arc) — these cards are not part of any normal draw deck.

**Branching Choices:**
Each Arc card presents a choice, for example:
- *Option 1: Pay 3 IG → go to Arc Card #14*
- *Option 2: Sacrifice 1 ground unit → go to Arc Card #17*

Your choices determine which path through the arc you take. Two players running the same arc can end up on completely different branches.

**Completing an Arc:**
The final card in your path presents one or more **Endings**. Each ending is a permanent reward or consequence based on the choices you made. Examples:
- Gain a unique permanent card added to your empire deck forever
- Unlock a special ability for your population or fleets
- Transform a star system (e.g. convert it to a black hole for a massive research boost)
- Suffer a consequence if your choices led to a bad ending

**Permanent Arc Reward Cards:**
Cards gained from completing a Story Arc are added directly to your empire deck and stay there permanently. They represent what your empire learned or achieved through that story. These cards can be one-time use, recurring, or grant passive permanent effects — it depends on the specific ending earned.

> **⬜ TODO:** Design the full Event Card deck — how many cards total? What is the split between Immediate, Choice, and Arc Starter types?

> **⬜ TODO:** Design the Story Arc card groups — how many arcs exist? How long is each arc (how many cards deep)? How many branching endings does each arc have?

> **⬜ TODO:** Can a player run multiple Story Arcs simultaneously, or only one at a time?

> **⬜ TODO:** Are Story Arcs visible to other players, or kept secret until completed?

---

### Space Units

All ships use a D6 to resolve combat. Prices are listed in resources: **CG** (Consumer Goods), **IG** (Industrial Goods), **Eco** (Economic Points).

#### Hero Flag Ship *(once per game per player)*
- **Price:** 3 CG, 3 IG, 3 Eco
- **Health:** 6
- **Hit [D6 1–4]:** 4 damage
- **Direct Hit [D6 5–6]:** 5 damage
- **Special Attack:** 2× D6 [5, 7, 11]: success
  > **⬜ TODO:** Clarify the Hero Flagship's Special Attack — "2× D6 [5, 7, 11]: success" is ambiguous. What does success mean? What does the special attack do when it succeeds vs. fails?

#### Flag Ship
- **Price:** 2 CG, 3 IG, 2 Eco
- **Health:** 5
- **Miss [D6 1]:** 0 damage
- **Hit [D6 2–4]:** 3 damage
- **Direct Hit [D6 5–6]:** 5 damage

#### Cruiser

| Tier | Price | Health | Miss | Hit | Direct Hit |
|------|-------|--------|------|-----|------------|
| I – Basic | 1 CG, 2 IG | 3 | 1–2 | 3–5: 2 dmg | 6: 3 dmg |
| II – Advanced | 2 CG, 2 IG, 1 Eco | 4 | 1 | 2–4: 3 dmg | 5–6: 4 dmg |

#### Destroyer

| Tier | Price | Health | Miss | Hit | Direct Hit |
|------|-------|--------|------|-----|------------|
| I – Basic | 1 CG, 1 IG | 2 | 1–3 | 4–5: 1 dmg | 6: 2 dmg |
| II – Advanced | 1 CG, 1 IG, 1 Eco | 2 | 1 | 2–4: 2 dmg | 5–6: 3 dmg |
| III – Advanced | 1 CG, 2 IG, 1 Eco | 3 | 1 | 2–4: 2 dmg | 5–6: 4 dmg |

#### Fighting Carrier

| Tier | Price | Health | Carry | Miss | Hit | Direct Hit |
|------|-------|--------|-------|------|-----|------------|
| I – Basic | 1 CG, 1 IG | 2 | 2 | 1–3 | 4–5: 1 dmg | 6: 1 dmg |
| II – Advanced | 1 CG, 2 IG | 2 | 3 | 1–2 | 3–5: 1 dmg | 6: 2 dmg |

> **⬜ TODO:** Carriers have a carry capacity — define what "carry capacity" means mechanically. What units can be carried, and how are they deployed during Landing?

#### Fighter
- **Price:** 1 IG
- **Health:** 1
- **Hit [D6 4–6]:** 1 damage vs. Fighters and Destroyers only; no damage to others

#### Colony Ship / Civilian Carrier
- **Price:** 2 CG, 2 IG
- **Health:** 4
- **Carry Capacity:** 1 population
- Cannot explore star systems
- Cannot initiate battle
- Considered a civilian ship

#### Scout
- **Price:** 1 CG, 1 IG, 1 Eco
- **Health:** 2
- **Hit [D6 4–6]:** 1 damage (any target)
- Used to explore new star systems
- Cannot initiate battles
- Considered a civilian ship

> **⬜ TODO:** Define **Lore-Based Fleet Ships** — there is a placeholder for empire-specific ships. What ships exist per empire and what are their stats?

---

#### Fleet Rules

- Each player may have up to **3 space fleets**.
- Each fleet is represented by a **fleet marker with a flag**.
- A fleet must always contain at least one **Flagship**.
- Each fleet may have up to **3 Flagships**.
- Each fleet has its own **fleet board/card**.

> **⬜ TODO:** There is a design idea to limit fleet capacity based on empire level. Define whether this is a rule — if so, what are the capacity thresholds per empire level?

> **⬜ TODO:** Define the **fleet board/card** — what information does it track? How are ships assigned to fleets in play?

**Flagless Fleets:**
- Stay in their current planet and act as defending power.
- May join ongoing space battles in **neighboring star systems**.
- Cannot initiate battles.
- Can bring ground reinforcements to ongoing ground battles in neighboring systems.
- Ships in flagless fleets are placed on the planet cards they occupy.

---

### Ground Units

Ground units use colored dice to resolve combat. Damage varies by target type.

#### Hero Unit *(once per game per player)*

> **⬜ TODO:** Define the Hero Ground Unit — stats, price, special abilities, and dice type are not yet defined. This is referenced in the notes but has no content.

#### Space Marines

| Tier | Price | Health | Miss | Hit | Direct Hit |
|------|-------|--------|------|-----|------------|
| I | 1 Blue Pop + 1 IG | 2 | D6 1–3 | 4–5: 1 vs Marines, 0 vs AV | 6: 2 vs Marines, 2 vs AV |
| II – Special Forces | 1 Blue Pop + 2 IG + 1 Eco | 3 | D6 1–2 | 3–5: 2 vs Marines, 2 vs AV | 6: Total vs all |

#### Armored Vehicle (AV)

| Tier | Price | Health | Miss | Hit | Direct Hit |
|------|-------|--------|------|-----|------------|
| I | 1 Blue Pop + 2 IG + 1 Eco | 4 | D6 1–3 | 4–5: 2 vs Marines, 1 vs AV | 6: Total vs Marines, 2 vs AV, 1 vs Arty |
| II – Advanced | 1 Blue Pop + 3 IG + 3 Eco | 5 | D6 1–2 | 3–5: Total vs Marines, 3 vs AV | 6: Total vs Marines & AV, 2 vs Arty |

#### Mobile Artillery
- **Price:** 1 Blue Pop + 1 IG + 1 Eco
- **Health:** 2
- **Hit [D6 4–5]:** 2 vs Marines, 1 vs AV, 1 vs Arty
- **Direct Hit [D6 6]:** Total vs Marines, 1 vs AV, 2 vs Arty

> **⬜ TODO:** Define **Lore-Based Ground Units** — empire-specific ground units are referenced but have no stats or rules.

> **⬜ TODO:** What does "total damage" mean precisely — is it the full health pool of the target unit, or the maximum damage of the attacking unit?

> **⬜ TODO:** Define the colored dice system — which color die does each unit type use (Red, Blue, Green, Black, Yellow are referenced in the notes)? Are these standard D6s or custom dice?

---

### Structures

#### Space Structures

**Star Dock**
- **Price:** 1 CG, 2 IG, 1 Eco
- **Health:** 5
- **Limit:** One per every 3 controlled star systems (rounded up)
- **Requirements:** Must be built in a star system with a populated IG district
- **Effects:**
  - Docked fleets do not pay maintenance costs
  - Enables production of space units
  - Enables production of space defense systems in its own system

> **⬜ TODO:** Define the **Docking Area** more precisely — does only a Star Dock count as a docking area? Can a player's home planet count as one at the start?

**Mega Structures** *(future development)*

> **⬜ TODO:** Define all Mega Structure rules, costs, and effects:
> - **Dyson Swarm** — resource production? health? requirements?
> - **Space Defense System (SDS)** — what does it defend against and how?
> - **Habitats** — population expansion? special districts?
> - **Lore Mega Structures** — empire-specific mega structures?

#### Ground Structures

**Defense Artillery System**
- **Price:** 2 IG, 1 Eco
- **Health:** 3
- **Effect:** Occupies one reinforcement slot on the ground battle card; fires each ground battle stage (D6 4–5: 1 dmg any; D6 6: 1 dmg any)

**Planetary Shield System**
- **Price:** 6 IG, 8 Eco
- **Health:** None
- **Requirements:** Can only be built on a star system with a mega structure or the empire's home planet
- **Effects:**
  - Blocks all deployments to the planet unless removed
  - Can only be destroyed by a special hero attack (Ground Force or Capital Ship)
  - Can only be attacked during the deployment phase after a space battle

**Medical Barracks**
- **Price:** 1 IG, 1 CG, 1 Eco
- **Health:** None
- **Effect:** Heals every marine unit by 1 damage between ground battle rounds

> **⬜ TODO:** Define **Theme/Lore Structures** — referenced in the notes as a category but no structures are defined.

> **⬜ TODO:** Can structures be destroyed by space bombardment, or only during ground battle? Clarify attack rules for ground structures from space.

---

### Dice

RoGEs uses two custom dice designed to replace multi-die rolls with single, purpose-built results.

---

#### 🎲 Colonization Die (D12)

Used when a Colony Ship attempts to colonize a planet. Roll once and read the result directly.

| Faces | Result |
|-------|--------|
| 9 | **Success** — colonization succeeds |
| 2 | **Soft Fail** — colonization fails, colony ship undamaged |
| 1 | **Hard Fail** — colonization fails, colony ship is damaged |

*Replaces the old 2D6 roll.*

---

#### 🎲 Exploration Die (D12)

Used when a Scout enters the inner side of an unexplored star system. Roll once — the result tells you exactly what planets and moons are in the system. No second roll needed.

| Faces | Result |
|-------|--------|
| 6 | **1 planet, 1 moon** |
| 2 | **1 planet, 2 moons** |
| 3 | **2 planets, no moons** |
| 1 | **Giant planet** |

*Replaces the old D8 + D6 two-roll system.*

---

#### 🎲 Space Combat Dice

> **⬜ TODO:** Design custom space combat dice — all ships currently use a standard D6 with different hit thresholds per ship type. Define whether these become custom dice (with faces showing miss/hit/critical symbols) or remain standard D6s referenced against unit cards.

---

#### 🎲 Ground Combat Dice (Colored D6s)

Each ground unit type uses a specific colored D6. The color indicates the unit's combat profile.

| Color | Unit |
|-------|------|
| 🔴 Red | Space Marines I |
| 🔵 Blue | Space Marines II (Special Forces) |
| 🟢 Green | Armored Vehicle I |
| ⚫ Black | Armored Vehicle II |
| 🟡 Yellow | Mobile Artillery |

> **⬜ TODO:** Decide whether ground combat dice are standard D6s (players reference unit cards for results) or custom dice with printed miss/hit/critical faces per unit type. If custom, design the face distribution for each color.

---

## Game Setup

### Galaxy Setup

1. Place the **Center of the Galaxy** tile in the middle of the table.
2. Before setup, players agree on the number of **Anomaly Tiles** to include:
   - **Default:** Equal to the number of players
   - **Maximum:** Up to 2× the number of players
   Shuffle the agreed number of anomaly tiles into the galactic tiles deck. The backs of all tiles look identical — players cannot tell anomalies from star systems until a tile is placed and flipped.
3. Players draw tiles from the shuffled stack and build the galaxy outward from their home base locations toward the center.
4. When a tile is placed and flipped:
   - If it is a **Star System** tile — place it normally.
   - If it is an **Anomaly** tile — place it where it landed. The galaxy is fixed. The anomaly stays.
5. Anomaly placement restrictions:
   - An anomaly tile **cannot** be placed adjacent to another Space Anomaly tile.
   - An anomaly tile **cannot** be placed adjacent to another player's home base (but may be adjacent to your own).


#### Galaxy Size

RoGEs supports **2–4 players**, always played on a **Ring 3 galaxy** (3 rings around the center tile):

| Players | Ring Size | Total Tiles | Anomalies (default → max) | Explorable Systems | Strategic Win (~⅓) |
|---|---|---|---|---|---|
| 2 | Ring 3 | 37 | 2 → 4 | ~30 | ~10 systems |
| 3 | Ring 3 | 37 | 3 → 6 | ~29 | ~10 systems |
| 4 | Ring 3 | 37 | 4 → 8 | ~28 | ~9 systems |

*Explorable systems excludes home systems, Nepiru, and anomaly tiles.*

**Anomaly placement edge case:** If a player draws an anomaly tile but no valid position exists (all available positions are adjacent to another anomaly or another player's home base), they **reshuffle the anomaly tile back into the deck** and draw again until they get a placeable tile.

---

### Space Anomalies

Space Anomalies are permanent features of the galaxy. They cannot be colonized or controlled, but they have lasting effects on the surrounding area and can be harnessed by the empire that discovers them.

#### Discovering an Anomaly
When a player's unit first enters an anomaly hex during play (not during galaxy setup), that player **discovers** the anomaly.

**Invalid anomaly discovery — adjacent to a home planet or another anomaly:**
If the discovered anomaly hex is adjacent to any player's home planet or to another anomaly tile (violating placement rules), the following steps apply in order:

1. **Swap with a valid adjacent system** — the player chooses an adjacent unexplored star system tile that does not violate the anomaly adjacency rules. They physically swap that tile with the invalid anomaly tile — the anomaly is placed in the chosen system's position and stays there permanently. The player then explores the swapped system (now in the original anomaly's position) as normal.
2. **Extend one ring farther** — if only one surrounding system exists and it also violates the rules, the player may choose an unexplored system one star system farther away to swap with instead, using the same swap procedure.
3. **Inaccessible anomaly** — if no valid swap target can be found in either the surrounding or extended range, the anomaly is treated as **inaccessible**. It remains on the map undiscovered. The scouting unit may choose a different route or repeat its full movement from its starting position this turn.

When the anomaly is discovered:
- They immediately draw the **Anomaly Arc Starter card** for that anomaly type.
- They may choose to commit to the arc (meeting any entry condition) or decline.
- The arc **belongs permanently to the discoverer** — it cannot be conquered or transferred. If the discovering empire is eliminated, the arc is lost and the anomaly remains on the map with its current passive effect permanently.

#### Anomaly Passive Effects
Every anomaly has a **passive effect** that applies to surrounding hexes. The nature of this effect depends on the anomaly type and the state of its arc:

**Before the arc is completed**, the anomaly has its default effect — usually a debuff:
- Units in or adjacent to the anomaly hex may suffer **increased maintenance costs**
- Units moving through the hex may require **extra movement power**
- Nearby populations or districts may take **passive damage or resource loss** each Maintenance Phase

**After the arc is completed**, the effect permanently changes based on the arc ending reached:
- A cooperative or positive arc path may **flip the effect to a buff** — generating special resources, boosting nearby production, or providing movement advantages
- An aggressive arc path may **amplify the debuff** — turning the anomaly into a weapon that harms surrounding enemy systems while leaving allied territory unaffected

#### Effect Types
Anomaly effects are not all the same — each anomaly type has its own mechanic:

- **Dice-based recurring** — roll at each Maintenance Phase and apply the result to surrounding hexes. Could be damage, resource loss, or a bonus depending on arc state.
- **Fixed permanent** — a constant effect that applies automatically from discovery. No rolling needed.
- **Triggered once** — fires immediately upon discovery, then settles into a passive state.

#### Strategic Value
Because the arc cannot be taken, controlling the anomaly arc is a form of **permanent passive power**. A player with an anomaly adjacent to enemy territory can pursue an aggressive arc path to turn it into an ongoing hazard for their enemies. This makes discovering anomalies a significant strategic event — not just a neutral obstacle.

> **⬜ TODO:** Define all anomaly types — what anomalies exist (black hole, nebula, etc.), what are their default effects, what movement penalties do they impose, and what special resources if any do they generate?

> **⬜ TODO:** Design the Story Arc for each anomaly type — how many steps, what are the branching choices, and what are the positive vs. negative endings?

> **⬜ TODO:** Define the radius of anomaly effects — how many hexes away do effects reach? Does proximity matter (closer = stronger effect)?

### Player Setup

Each player, in setup order:

1. Takes a set of **Empire Cards** and shuffles them.
2. Draws **5 cards** (hand size) from their Empire deck.
3. Decides where their **home planet** is located:
   - Home planets must not be closer to any other player's home planet than: *(rim system count ÷ number of players, rounded up)*.
4. Runs an **Exploration** turn to populate their starting star system:
   - All planets and moons must be populated.
   - The starting star system must have at least one **Industrial Goods (IG)** district *(unless the player agrees otherwise)*.
   - Adjusts their income tableau to match starting production power.
   > **⬜ TODO:** Define the **income tableau** more precisely — how are production counters tracked per district type? Are there physical tokens, dials, or cards representing current production strength?
5. Takes the following starting resources:
   - 4× Consumer Goods (CG)
   - 4× Eco
   - 2× Industrial Goods (IG)
6. Places a **Scout** unit in one outer rim region of their star system.
7. Places a **Star Dock** in their home system.
8. Places one **Fleet token** on their home planet.
9. Places one fleet card (hidden) containing:
   - 1× Flagship
   - 1× Destroyer
   - 2× Fighters

> **⬜ TODO:** Define player turn order for setup — do players choose home planet locations simultaneously or in turn order? If in turn order, how is the first player determined?

---

## The Game Round

A game round is not a fixed sequence of phases — it is a repeating **Action → Conflict cycle** that continues until all players have fully exhausted their empire decks. Only then does the Maintenance Phase take place.

The full structure of a round is:

1. **Action Phase** — Players spend down their hands one card at a time.
2. **Conflict Phase** — Triggered once all hands are empty. Resolves all battles.
3. **Draw Step** — Each player draws back up to hand size (if cards remain in their deck).
4. *(Repeat steps 1–3 until all decks are empty.)*
5. **Maintenance Phase** — Triggered only when all players have no cards left in hand **and** no cards remaining in their empire deck.

---

## Player Action Phase

Players take turns playing **Action Cards** from hand, starting with the **first player** and proceeding clockwise.

On your turn:
1. Play a card from hand.
2. Execute the action(s) on the card.
3. Discard the played card to your discard pile.
4. Pass the turn clockwise to the next player.

A player **must pass** if they have no cards in hand.

Once **all players have passed** (all hands are empty), the **Conflict Phase** begins.

---

## Draw Step

After the Conflict Phase resolves, each player **draws cards from their empire deck up to hand size (5)**. Players who have no cards remaining in their deck do not draw and are considered **deck-exhausted** for this round.

- If at least one player still has cards to draw, a new **Action Phase** begins immediately.
- If **all players** are deck-exhausted (no cards in hand, no cards left in deck), proceed to the **Maintenance Phase** instead.

---

### Production

The **Production** action card allows the player to either:

- **Produce resources and goods** up to the strength of their empire (as shown on the resources counters on the player tableau):
  1. Add produced resources to the market area of the player's tableau.
  2. Apply the **economic stance** for all available transformations:
     - Remove costs directly from the market area.
     - Add transformed resources to the empire storage area.

- ***or*** **Change the economic stance** to a different one and skip production this turn.

### Resources

There are three resource types in RoGEs:

| Resource | Name | Role |
|---|---|---|
| **CG** | Consumer Goods | Feeds populations; pays empire maintenance costs. The empire's bread. |
| **IG** | Industrial Goods | Builds ships, weapons, and structures. The empire's steel. |
| **Eco** | Economic Power | Flexible energy — work, power, capital. Transforms into CG or IG depending on your Economic Stance. The empire's electricity. |

During the Production action:
1. All districts generate their resources simultaneously — CG districts → CG, IG districts → IG, Eco districts → Eco.
2. All newly produced resources are collected into the **Production Buffer** on the player tableau.
3. The active **Economic Stance** is applied to the buffer — converting Eco into CG, IG, or leaving it as-is.
4. All resources in the buffer (now transformed) are moved into the **Storage Area** of the player tableau.

### Economic Stances

A player's **Economic Stance** determines how their **Eco** is transformed each time they produce. A stance is chosen once and stays active until the player uses a Production action to change it (forgoing production that turn).

| Stance | Eco Converts To | When to use |
|---|---|---|
| **Militarization** | All Eco → IG | Building ships, weapons, or structures |
| **Growth** | All Eco → CG | Expanding population or sustaining a large empire |
| **Balanced** | Eco stays as Eco | Saving flexibility; no conversion takes place |

In **Balanced** stance, no conversion takes place — all resources in the buffer move to storage as-is, including Eco. Stored Eco can be spent directly wherever Eco is accepted as a cost.

### Player Tableau

Each player's tableau tracks their empire's economy across two areas:

- **Production Buffer** — A temporary holding area that collects all newly produced resources each time a Production action is played. The Economic Stance is applied here before resources are moved on.
- **Storage Area** — Where resources live between actions and rounds. All costs (maintenance, building, recruitment) are paid from storage.

> **⬜ TODO:** Define the **income tableau** more precisely — how are production counters tracked per district type? Are there physical tokens, dials, or cards representing current production strength?

---

### Mobilization

The **Mobilization** action card allows the player to either:

- Move a fleet or civilian ship up to their **movement strength**, ***or***
- Move up to **3 flagless fleets** from a neighboring system to reinforce an ongoing space battle or transfer ground units to an ongoing land battle.

Movement may be interrupted if:
- A **Scout** enters an unexplored star system → must perform **Exploration**.
- Any other ship encounters non-allied pieces → initiates **Space Battle**.
- A **Fleet** performs a **Landing**.
- A **Colony Ship** performs a **Colonization**.

#### Movement Costs

Each star system hex has **6 outer rim sections** — one per edge — representing the inter-system space between stars. These are separate from the system's inner side.

| Move | Cost |
|---|---|
| Between outer rim sections within the same hex | 1 step |
| Cross into a **Ring 1** system's outer rim | 1 step |
| Cross into a **Ring 2** system's outer rim | 2 steps |
| Cross into a **Ring 3** system's outer rim | 3 steps |
| Enter a system's **inner side** from its outer rim | +1 step |

The crossing cost always equals the **destination ring number** — outer systems are further apart in space, so reaching them costs more. Moving toward the center is cheap; projecting force to the outer rings is expensive.

#### Movement Strength by Ship Type

| Ship | Steps | Typical range in one action |
|---|---|---|
| **Scout** | 7 | Reaches Ring 1 inner side (5 steps) with 2 steps to spare |
| **Fleet** | 5 | Reaches Ring 1 outer rim exactly from a Ring 3 home system |
| **Colony Ship** | 3 | Reaches Ring 2 outer rim comfortably from home |

Movement strength can be increased through **FTL technology upgrades**.

> **⬜ TODO:** Define FTL technology tiers — what upgrade levels exist, how are they researched, and how many steps does each tier add?

---

### Civilian Actions

The **Civilian** action card allows the player to perform **one** of the following:

- **Repair** — Restore any number of damaged units, buildings, or structures to full health in a single Civilian action.
  - **Cost:** Half the base purchase price of each unit or structure being repaired (rounded down).
  - There is no limit to how many units can be repaired in one action — pay the cost for each and restore them all.
  - > **⬜ TODO:** Define whether Repair can be performed anywhere or only at specific locations (e.g. ships at a Star Dock, ground structures on their planet).

- **Build** — Construct one space ship or one building per Build action.
  - **Space ships:** Must be built at a **Star Dock**. Pay the ship's cost and assign it to a fleet in the same star system or any neighbouring star system. If no fleet is available: create a new fleet (if the ship is a Flagship) or add the ship to any planet card you control in that system.
  - **Buildings:** Must be built in a star system with at least one **populated IG district**. Pay the building's cost and place it on the target planet card.
  - **Star Dock build capacity** is **1 ship per Build action** by default. This can be increased through research:
    > **⬜ TODO:** Define the Star Dock capacity upgrade — which research tech unlocks it, and how many additional ships per action does it allow?

- **Launch** — Deploy a new Star Dock into a star system.
  - Select a star system with at least one **populated IG district**.
  - Pay the Star Dock cost: **1 CG, 2 IG, 1 Eco**.
  - Place the Star Dock token in that star system.
  - **Star Dock limit:** A player may have at most **1 Star Dock per 3 controlled star systems** (rounded up). Exceeding this limit is not possible — a Launch action cannot be played if the player is already at their limit.

- **Recruit Ground Units** — Train new ground forces
  > **⬜ TODO:** Define Recruit rules — where can ground units be recruited? Do they require a specific structure? Can multiple units be recruited in one action?

- **Populate** — Add a population to a planet district
  > **⬜ TODO:** Define Populate rules for each pop type:
  > - **Green pop** — what districts does it fill? What does it produce?
  > - **Blue pop** — what districts does it fill? What does it produce?
  > - **Orange pop** — can only be placed if all other slots are occupied; define what it produces and its cost.
  > - When can a player switch a pop type in a dual/omni production district?

- **Research** — Discover and develop technologies from the Research Decks.

  There are four Research Decks, one per category:
  - 🏛️ **Culture & Infrastructure** — buildings, Star Dock upgrades, population growth
  - 💰 **Economy** — resource production, trade, Eco conversion
  - 🤝 **Diplomacy** — alliances, political influence, inter-empire relations
  - ⚔️ **Military (War)** — fleet combat, ship upgrades, ground units, FTL movement

  The Research action always follows this sequence — a player may perform **both steps or only one**:

  1. **Discover** — Draw one card from any Research Deck and place it face-up in your **Research Area** on your player tableau.
  2. **Develop** — Fulfill the requirements on one card in your Research Area to unlock its effect. If the card is a **Research Arc**, advance it one step — each step unlocks a partial benefit and the player may stop at any depth.

  > **⬜ TODO:** Finalise all Research Card content — names, requirements, and effects for all four decks. See [Tech Tree](tech-tree/tech-tree.md) for the full template and open design questions.

- **Upgrade** — Improve a unit or structure to the next tier.
  - Pay the **price difference** between the current tier and the next tier.
  - Units can only be upgraded **one level at a time**.
  - Both **space ships** and **ground units** can be upgraded.
  - Upgrading costs a full **Civilian action**.
  > **🧪 PLAYTEST:** Decide whether upgrade location should matter — e.g. ships must be at a Star Dock, ground units must be on a planet with a populated IG district. Leave unrestricted for now and evaluate during playtesting.

- **Progress a Story Arc** — Advance one step in one active Story Arc at your tableau. Read the current Arc card, choose an option, pay the cost, and move to the next referenced card. If this is the final card, collect your ending reward.
  - Only **one arc** may be advanced per Civilian action.

---

### Exchange

The **Exchange** action card allows the player to:

- **Initiate a trade agreement**, ***or***
- **Trade with neighboring empires:**
  - Trading can be done with any empire neighboring the player's empire.
  - Or with empires that have an existing trading agreement with the player.
  - Or with the **black market** at black market prices.

#### Neighboring Empires

Two empires are **neighboring** if they have at least one star system whose hex is directly adjacent (shares a border) to a star system controlled by the other empire.

#### What Can Be Traded

There are no limits on what can be traded — resources, star systems, fleet rentals, ground units, and promises are all valid. Trades fall into two categories:

- **Binding agreements** — any trade involving the immediate exchange of resources or star systems is binding and must be honored in full during the same Exchange action. Neither player can partially trade.
- **Promissory agreements** — future promises (e.g. "I will not attack you this round") are non-binding by default. Breaking one carries no mechanical penalty — your reputation is your only collateral.

**Making a Promissory Agreement Binding**

Both players may choose to make a promissory agreement binding. There are two ways to do this:

- **Chaos Penalty** — both players declare the agreement binding. If the agreement is broken, the breaching player immediately draws **1 Chaos Event Card** and must follow it in full.
- **Resource Deposit** — both players deposit an agreed number of resources into a shared escrow at the time of the agreement. If the agreement is broken, the breaching player forfeits their deposit to the other party. If both parties honour the agreement, deposits are returned.

Players choose which method to use when the agreement is made. Both methods can be combined if players agree.

Players may also trade with **NPC empires** (1st Sentients, Ancient Rulers, Galactic Traders) that may appear during play.

#### Trade Agreements

A **Trade Agreement** is initiated via the Exchange action. When established, **both players exchange one Trade Agreement token** with each other — the token represents the active agreement and sits on the other player's tableau as a reminder.

Each player has a limited number of Trade Agreement tokens equal to **half the number of players, rounded down**:

| Players | Trade Agreement tokens per player |
|---|---|
| 2 | 1 |
| 3 | 1 |
| 4 | 2 |

This limits how many active trade agreements a player can hold at once. A player with no tokens available cannot initiate a new Trade Agreement until an existing one is cancelled.

**Cancelling a Trade Agreement:** Either player may cancel using an Exchange action. Both tokens are returned at the **end of the current round** — the agreement remains active for the rest of that round so neither player is blindsided mid-turn.

#### Black Market

The Black Market allows players to buy and sell **CG** and **IG** using **Eco**. It has a total capacity of **20 units** of each resource type.

Prices are **dynamic** — they depend on how much stock is currently on the market. The more supply, the cheaper it is to buy; the less supply, the more expensive. All transactions in one Exchange action use the **current price**. Prices update only after the Exchange action is fully resolved.

If the Black Market exceeds its 20-unit capacity, excess resources go to the bank instead — but the market still accepts purchases even at max capacity.

**Black Market Prices — 2 Players**

| CG on market | Buy/Sell price (in Eco) |
|---|---|
| 1 – 5 | 4 Eco |
| 6 – 10 | 3 Eco |
| 11 – 15 | 2 Eco |
| 16 – 20 | 1 Eco |

| IG on market | Buy/Sell price (in Eco) |
|---|---|
| 1 – 4 | 5 Eco |
| 5 – 8 | 4 Eco |
| 9 – 12 | 3 Eco |
| 13 – 16 | 2 Eco |
| 17 – 20 | 1 Eco |

**Black Market Prices — 3–4 Players**

| CG on market | Buy/Sell price (in Eco) |
|---|---|
| 1 – 7 | 3 Eco |
| 8 – 14 | 2 Eco |
| 15 – 20 | 1 Eco |

| IG on market | Buy/Sell price (in Eco) |
|---|---|
| 1 – 5 | 4 Eco |
| 6 – 10 | 3 Eco |
| 11 – 15 | 2 Eco |
| 16 – 20 | 1 Eco |

> **⬜ TODO:** Define the physical Black Market tracker — how is current stock tracked on the table? Is there a shared board, tokens in a pool, or a dial?

---

## Conflict Phase

The Conflict Phase consists of three sequential parts:

1. **Space Battle** — Resolve all space conflicts
2. **Landing Step** — Players may initiate invasions, landings, or ground reinforcements
3. **Ground Battle** — Resolve all ground conflicts

For both Space and Ground Battles, start with conflicts in player order. Multiple battles may take place simultaneously if all participating players agree.

---

### Conflict Rules

- Only **Allied Empires** may occupy the same star system without conflict.
- Only **Allied Armies** may be positioned on the same stellar body without conflict.
- If non-allied empires/fleets occupy the same star system segment (inner-side, outer rim, or planet), **battle begins immediately**.
- Fleets in the **outer rim** can be targeted by planetary defenses with reach.
- Fleets in the **inner side** can be targeted by planetary defenses with or without reach.
- Fleets in a star system can be targeted by neighboring planetary defenses with reach.

---

## Alliances

Alliances are strategic partnerships between empires that grant specific mutual benefits. There are two alliance types: **Economic** and **War**. They are independent of each other — both can be held with the same empire simultaneously, but each must be formed separately. Tech is not an alliance type — research cards and technologies can be bought, sold, or gifted through the Exchange action as normal trade.

---

### Economic Alliance

**Benefits:**
- Both empires gain access to each other's active **Economic Stance** — either player may produce as if they had their ally's stance active.
- Both empires may trade with each other **regardless of distance** — no adjacency required once the alliance is formed.

**Limits:** Economic Alliances are **bilateral only** — exactly two players per alliance.

**Formation requirement:** The two empires must have at least **one adjacent star system** at the time of formation. Once formed, the alliance persists even if the empires later lose adjacency.

**How to form:** Both players must each spend an **Exchange action in the same round**. The alliance activates at the start of the next round.

**Cancellation:** Either player may declare cancellation during **Maintenance Phase**. The alliance remains active for one full round after the declaration. An Economic Alliance cannot be cancelled until it has been active for at least **2 rounds**.

---

### War Alliance

**Benefits:**
- Neither party may attack the other — non-aggression is automatic and binding.
- Both empires may fight other players as a **coalition**.
- Full co-occupation rights:
  - Fleets may share the same star system without triggering battle.
  - Ground units may occupy different planets within the same star system without conflict.
  - Allied ground units may combine into the same planetary army and defend together.

**Limits:** A War Alliance may include **at most 3 players against 1**. If a 3-player coalition achieves an **Annihilation victory** against their common target, the remaining players may collectively call a vote to **cancel that victory** and continue the game — a 3-against-1 Annihilation win is considered unsportsmanlike and is not automatically valid.

**How to form:** Both players must each spend an **Exchange action in the same round**. The alliance activates at the start of the next round.

**Cancellation:** Either player may declare cancellation during **Maintenance Phase**. The alliance remains active for one full round after the declaration. A War Alliance cannot be cancelled until it has been active for at least **2 rounds**.

**Breaking a War Alliance by attacking your ally** without first declaring cancellation is an immediate violation — the attacking player draws **1 Chaos Event Card**.

---

### Alliance Summary

| | Economic Alliance | War Alliance |
|---|---|---|
| Max parties | 2 players | Up to 3 vs 1 |
| Formation requirement | Adjacent star system | Exchange action only |
| Activates | Start of next round | Start of next round |
| Minimum duration | 2 rounds | 2 rounds |
| Cancellation notice | 1 full round | 1 full round |
| Breaking early penalty | — | 1 Chaos Event Card |

#### Separate Timelines for Battles

Battles run on a faster timeline than the main game:
- **3 conflict rounds** take place for every **1 main game round**.
- After 3 conflict rounds, a normal Game Round takes place — excluding the conflict area.
- Players may attempt to reinforce armies/fleets between game rounds by entering the star system.

**When a battle begins, the main game pauses for all players** until the battle is fully resolved. Non-involved players wait and observe. This is consistent with the existing game rhythm — players already wait between their own action turns while others act. A battle resolving between two players is simply another form of that natural wait, and it keeps the game state clear and visible to everyone at the table.

---

### Space Battle

> **⬜ TODO:** Define Space Battle rules in full, including:
> - How the attacking and defending sides are determined
> - Turn order within a space battle
> - The **Frontline and Defence Line** concept — ships can be moved to the front line to absorb damage first; only when the front line is destroyed does the defensive line take damage. Ships can join the frontline but cannot leave it. Capital ships / cruisers with artillery capabilities can be held back for arty attacks.
> - How ship cards are revealed (fleet cards are placed "hidden" — when are they revealed?)
> - Whether multiple battles in the same system are resolved simultaneously or sequentially
> - Win/loss conditions for a space battle and consequences (destruction, retreat, capture?)
> - What happens to civilian ships (Scouts, Colony Ships) caught in a space battle

---

### Landing

> **⬜ TODO:** Define Landing rules in full, including:
> - When and how a player may initiate a landing
> - Which ships can carry ground units and how many (Carrier capacity)
> - The **Planet Fall** mechanic — referenced in Ground Battle notes but not defined
> - Whether landing is contested and if so how it is resolved
> - What happens when a Planetary Shield System is active (deployment is blocked — only special hero attacks can remove it)

---

### Ground Battle

A Ground Battle begins when ground units from two or more non-allied empires (or NPC empires) are present on the same planet.

1. All ground units on the planet must join the battle for their empire.
2. Before each battle round, each player may declare **retreat or surrender**.
3. Starting with the active player, each player applies any **pre-battle effects** (cards, tech, etc.) — all simultaneously.
4. Each player rolls dice for their units and assigns damage:
   - Each unit/weapon must be assigned a **target before rolling**.
   - Apply damage as rolled.
   - Repeat for **3 fire exchange rounds**.
5. After 3 exchanges, the **battle round ends**.
6. If ships carrying troops are still available, the empire may attempt a **Landing** and continue the ground battle.
7. After each battle round, players apply any **post-battle effects** simultaneously.

> **⬜ TODO:** Define **NPC Empire** behavior — how do NPC/hostile entities (that may appear via event cards during exploration) behave in ground battles? Do they have fixed units and dice rolls?

> **⬜ TODO:** Define **pre-battle and post-battle effects** — what cards or tech can be played, and in what sequence?

> **⬜ TODO:** Define the **Ground Battle Card** — what does it track? How are reinforcement slots used?

> **⬜ TODO:** Define win/loss conditions for ground battle — what determines control of a planet? Is it when all enemy units are eliminated, or can a player win with a single remaining unit?

#### After a Ground Battle is Won

When a player wins a ground battle and has surviving ground units on the planet:

1. The victor **immediately takes the planet card** — including all attached resource tags and event cards — and adds it to their tableau.
2. The defeated empire's population on the planet is **halved, rounded down**:
   - e.g. 3 pops → 1 survives, 4 pops → 2 survive
3. Removed pops follow this **priority order** — most expensive removed first:
   - **IG pops** removed first
   - **Eco pops** removed second
   - **CG pops** removed last
4. Removed pops return to the **general supply** (treated as infinite — pops are always available to be recruited again).
5. Surviving pops **remain on the planet** and now produce for the conquering empire.
6. The conquering player **adjusts their income tableau** to reflect the planet's production under their control.

> *Flavour: The population loss represents lives lost in the conflict and the uprising of the conquered people — the industrial workforce and skilled workers fought back or perished, leaving only ordinary civilians who now live under the new empire.*

---

### Retreat from Conflict

> **⬜ TODO:** Define Retreat rules in full, including:
> - When a player may declare retreat (before any battle round, or only between rounds?)
> - How retreating units move — where do they go, and can they be intercepted?
> - Are there consequences for retreating (morale, card penalties, etc.)?
> - Can only part of a force retreat, or must all units retreat together?

---

### Between Battles

Between game rounds during an ongoing conflict:

1. A standard **Game Round** takes place.
2. Fleets may enter the **outer rim** of a contested star system without joining the ongoing space battle.
3. Fleets entering the **inner side** of a system with an ongoing space battle **must join the battle**.
4. Fleets must follow all general Space Battle rules, including ground reinforcement restrictions.
5. Fleets can bring **reinforcements** to support ongoing space or ground battles.
6. **Flagless fleets** may join ongoing battles.
7. **Flagless fleets** may bring ground units to reinforce ground battles.

---

## Maintenance Phase

The Maintenance Phase is triggered only when all players are deck-exhausted — every player has played through their entire empire deck and has no cards remaining in hand or in their deck.

At that point:

1. **Check Victory Conditions** — declare a victor if any are fulfilled.
2. Each player must pay **empire maintenance costs**:
   - All space ships **not** in a star system belonging to their empire.
   - **Population costs** calculated by district count:
     - Industrial districts incur high costs.
     - Economic and consumer goods districts cost less.
   - Any other costs from active events.
3. **Pass the First Player marker** clockwise to the next player.
4. Each player **shuffles their full discard pile** back into their empire deck and **draws 5 cards** to begin the next round.

> **⬜ TODO:** Define exact **maintenance costs** per unit type — how much CG/IG/Eco does each ship type cost per round when not docked? What are the population maintenance costs per district type?

> **⬜ TODO:** Define costs for any **special buildings or active events** — what kinds of events can impose ongoing maintenance costs?

#### If Maintenance Cannot Be Paid

- The player may **trade with neighbors** or empires with a trade agreement to cover costs.
- If costs still cannot be met, the player must choose which units, populations, or special buildings to forfeit.
- The player draws **1 Chaos Event Card** per fleet or district that caused the unpaid cost.
- The player must **fully follow** the Chaos Event Card instructions.

> **⬜ TODO:** Define the consequences of forfeiting a unit or building — are they immediately destroyed, disbanded, or placed in a degraded state?

> **⬜ TODO:** Define the full **Chaos Card system** — how cards are drawn, when they must be resolved (immediately or end of round?), whether effects are instant or persistent, and whether a player can hold multiple chaos cards at once. Chaos Cards are currently referenced in: maintenance failure, broken binding agreements, and breaking a War Alliance early.

---

## Exploration & Colonization

### Exploration

- Each player starts with their home star system already fully explored and colonized.
- Unexplored star systems are empty — planets and moons are only revealed when explored.
- **Only Scouts** (and ships with scouting capabilities) may explore new star systems.

**Exploration Process:**
1. A scout may enter the **outer rim** of an unexplored system — this does **not** trigger events or resource cards.
2. The player may choose to enter the **inner side** of the system:
   - Roll the **Exploration Die (D12)** and draw planet/moon cards accordingly:
     - 6 faces: **1 planet, 1 moon**
     - 2 faces: **1 planet, 2 moons**
     - 3 faces: **2 planets, no moons**
     - 1 face: **Giant planet**
   - Draw the corresponding planet and moon cards and trigger their **[Reveal]** effects.
   - If an event causes hostile space entities to appear, a battle begins.
   - Scout movement **ends** upon entering the inner side, even if movement steps remain.

> **⬜ TODO:** Clarify when the moon roll is triggered — does a D8 result of 1–5 always allow a moon roll, or only some results? The note says "if the player can roll for moons" without defining the condition.

> **⬜ TODO:** Confirm the movement cost rules — the following are currently **proposed, not confirmed**:
> - Entering inner side always costs 1 movement step.
> - Outer rim entry cost: 1st ring = 1 step, 2nd ring = 2 steps, 3rd ring = 3 steps.
> - These costs may be modified by FTL technology.

---

### Colonization

- Colonization can only be performed by a **Colony Ship** carrying a colonizing population.
- The colonizing pop must be a **Blue (CG) pop** and cannot produce resources while on the colony ship.

**Loading a Pop:**
- Remove a pop from a planet district in a star system the colony ship is currently in (reducing CG production by 1), ***or***
- Add the pop directly using the **Populate** civilian action.

**Colonization Process:**
1. Use a **Mobilization** action to move the colony ship into an explored star system.
2. Initiate colonization on the desired planet.
3. Roll the **Colonization Die (D12)**:
   - **Hard Fail (1 face):** Colonization fails; colony ship is damaged.
   - **Soft Fail (2 faces):** Colonization fails; colony ship is undamaged.
   - **Success (9 faces):** Colonization succeeds.
4. On success:
   - Deploy the pop to any available **blue location** on the planet surface.
   - If no matching district exists in the whole star system, the pop may still be deployed but must be **transformed**.

> **⬜ TODO:** Define **pop transformation** — what does it mean to transform a pop when placed in a non-matching district? What are the costs or rules for transformation?

> **⬜ TODO:** Define colonization rules for **Green** and **Orange** pops — only Blue pop colonization is currently defined. Can other pop types be used to colonize?

---

## Politics & Alliances

Empires may form political relationships with one another:

**Types of Alliances:**
- **Economic Alliance** — Shared trade and resource support
- **War Alliance:**
  - Join each other's wars
  - Share military power
  - Send resources *(subject to supply lines / touching borders)*
- **Tech Alliance:**
  - Share technologies
  - Different tech powers may be partially activated depending on alliance terms

**Agreement Types:**
- **Binding Agreements** — *(rules TBD)*
  > **⬜ TODO:** Define Binding Agreements — what makes an agreement binding, what obligations does it create, and what happens if it is broken?
- **Non-Binding Agreements** — *(rules TBD)*
  > **⬜ TODO:** Define Non-Binding Agreements — how do they differ from binding ones? Can they be cancelled freely?

> **⬜ TODO:** Define supply line / border-touching rules — resource sending in War Alliances is noted as "dependent on supply lines / touching borders." Define what qualifies as a supply line and when borders are considered "touching."

> **⬜ TODO:** Define **Tech Sharing** in detail — which tech powers are activated at reduced strength when shared, and what does "less strong" mean for each tech?

> **⬜ TODO:** Define the consequences of **breaking an alliance** — are there diplomatic penalties, automatic war declarations, or card penalties?

---

## Hand Size

Player hand size is fixed at **5 cards** for all player counts throughout the entire game.

- This applies at setup, during the Action Phase, and when drawing at the end of each Maintenance Phase.
- Hand size does **not** scale with deck size — as Lore Cards and Event Cards are added to your empire deck over time, your hand size stays at 5.

---

## Design Notes & To Do

This section tracks all outstanding design work. Items marked here also appear inline above where they occur in the rulebook.

### Victory Conditions
- [x] ~~**Political Win**~~ — Removed. Does not fit the game.
- [x] **Planet & System Control** — Defined. Control = holding all planet cards in a system with no enemy units remaining.
- [x] **Moral Win** — Defined. Hold Nepiru planet card for 3 consecutive Maintenance Phases.
- [x] **Strategic Win** — Defined. Fully control one-third of star system hexes; checked once galaxy is fully explored.
- [x] **Annihilation Win** — Fully defined. Eliminated = last planet card lost. Shared victory with allies.
- [x] **Conquered population rules** — Defined. Halved (rounded down), removed IG → Eco → CG. Survivors produce for new owner. Removed pops return to supply.
- [x] **Nepiru** — Defined. Ancient dead civilization, Golden Districts (flexible, 2× production), exclusive transferable Story Arc. Number of districts and arc content still TBD.
- [x] **Anomaly tile setup** — Defined. Blind draw, tiles identical from back, galaxy is fixed on placement. Arc belongs to discoverer permanently, lost if eliminated.
- [x] **Anomaly placement edge cases** — Resolved. Reshuffle back into deck and redraw. Mathematically verified as always feasible across all player counts.
- [x] **Galaxy size** — Defined. Ring 3 (37 tiles) for 2–3 players, Ring 4 (61 tiles) for 4–6 players.
- [ ] **Anomaly types** — Define all anomaly types, default effects, movement penalties, special resources
- [ ] **Anomaly arc design** — Design arc for each anomaly type, branching choices, positive/negative endings
- [ ] **Anomaly effect radius** — How many hexes do effects reach? Does proximity affect strength?
- [x] **Simultaneous win conditions** — Defined. Annihilation takes priority. All others result in joint victory, with optional continuation by mutual agreement.

### Rules to Define from Scratch
- [ ] **Space Battle** — full rules including frontline/defence line mechanics, turn order, revelation of hidden fleet cards, and win/loss conditions
- [ ] **Landing / Planet Fall** — when and how units land, carrier deployment, contested landings
- [ ] **Retreat from Conflict** — when retreat can be declared, where retreating units go, interception rules
- [ ] **Research System** — tech tree template created ([Tech Tree](tech-tree/tech-tree.md)); branch names, costs, and effects still need finalising. Open questions: empire-specific branches, multi-research per action, first-to-research race mechanic
- [x] **Economic Stances** — Defined: Militarization (Eco→IG), Growth (Eco→CG), Balanced (no conversion)
- [x] **Player Tableau** — Defined: Production Buffer → stance conversion → Storage Area
- [x] **Movement Strength** — Defined: Scout 7, Fleet 5, Colony Ship 3; ring crossing costs = destination ring number
- [ ] **Docking Area** — what qualifies as a docking area beyond Star Docks
- [ ] **Maintenance Costs** — exact costs per ship type, per district type, per active event
- [ ] **Pop Transformation** — what it means and its cost
- [ ] **Populate Rules** — Green, Blue, and Orange pop rules; dual/omni district switching
- [ ] **Upgrade Rules** — where upgrades happen, whether they take a full action
- [ ] **Repair Rules** — how much is restored, cost, location requirements
- [ ] **Recruit Rules** — location requirements, multi-unit per action?
- [ ] **Trade Agreement Mechanics** — initiation, duration, cancellation
- [ ] **Black Market** — exchange rates, risks
- [ ] **Binding vs. Non-Binding Agreements** — obligations and consequences
- [ ] **Allied Armies & Allied Empires** — co-occupation rules, alliance tiers
- [ ] **NPC Empire Behavior** — hostile entities from exploration events
- [ ] **Ground Battle Card** — layout and reinforcement slot rules
- [ ] **Planet Fall** — mechanics for deploying troops from ships to a contested planet

### Cards to Create
- [ ] **Lore Cards** — per empire, full set with effects
- [x] **Event Cards** — system defined: single unified deck with Immediate, Choice, and Arc Starter types. Full card content still TBD.
- [x] **Story Arc Cards** — system defined: numbered branching card groups pulled from box. Full arc content still TBD.
- [ ] **Arc Reward Cards** — permanent cards earned by completing Story Arcs. Content TBD.
- [ ] **Chaos Cards** — full set of chaos effects; define how they are drawn, when they must be resolved, whether effects are immediate or persistent, and whether a player can hold multiple at once
- [ ] **Moon Cards** — properties, districts, colonization rules
- [ ] **Giant Planet Cards** — properties and unique effects

### Components to Define
- [ ] **Resource Tokens** — Rare Resources, Extra Deposits, Enhancers
- [ ] **Trading Agreement Tokens**
- [ ] **Mega Structures** — Dyson Swarm, SDS, Habitats, Lore Mega Structures
- [ ] **Theme/Lore Ground Structures**
- [ ] **Hero Ground Unit** — stats and special ability
- [ ] **Lore-Based Fleet Ships** — per empire
- [ ] **Lore-Based Ground Units** — per empire
- [ ] **Fleet Board/Card** — layout and what it tracks
- [x] **Colonization Die** — D12 designed: 9 success, 2 soft fail, 1 hard fail
- [x] **Exploration Die** — D12 designed: 6× (1 planet 1 moon), 2× (1 planet 2 moons), 3× (2 planets no moons), 1× (giant planet)
- [x] **Colored Dice System** — ground unit colors confirmed: Red, Blue, Green, Black, Yellow
- [ ] **Space Combat Dice** — decide: custom faces or standard D6 with unit cards?
- [ ] **Ground Combat Dice** — decide: custom faces per color or standard D6 with unit cards?

### Inconsistencies to Resolve
- [x] **Anomaly tile count** — Default = number of players. Players may agree to increase up to 2× the number of players before setup.
- [x] **Galaxy size** — Defined. Ring 3 (37 tiles) for 2–3 players, Ring 4 (61 tiles) for 4–6 players.
- [x] **Hand size** — Fixed at 5 cards for all player counts. Does not scale with deck size.
- [ ] **Draw timing during action phase** — draw after each card played, or only when hand is empty?
- [ ] **Hero Flagship Special Attack** — clarify what "2× D6 [5, 7, 11]: success" means and what success does

### Design Ideas Under Consideration
- [ ] Ship cards with upgrade slots and individual carrier cargo slots (from Idea notes)
- [ ] Fleet capacity limits based on empire level
- [ ] Variable exploration movement costs by galaxy ring distance
- [ ] "Total damage" definition — clarify whether this means target's full health or attacker's max damage

---

*Last compiled: April 2026 — based on all Obsidian notes under `01 - Rough Notes/Board-Games/RoGEs/Guide`*
