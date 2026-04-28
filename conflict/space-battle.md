# Space Battle

A Space Battle begins when a fleet enters a star system segment occupied by a non-allied empire's fleet. All fleets in that segment join the battle for their empire.

---

## Formation — The Fleet Card

Every fleet is organised across three lines on the Fleet Card before the battle begins. Placement is determined by unit role, not player choice.

| Line | Who goes here | Notes |
|---|---|---|
| **Frontline** | All combat ships without a defensive role | Mandatory |
| **Defensive Line** | Support ships with [Defensive] role (Arty, Repair) + all non-combat ships (Carriers, Colony Ships) | Support ships provide fire from here |
| **Reinforcement Line** | Reserve units waiting to enter the battle | Cannot attack; can be hit by [Arty] |

### Unit Tags
Tags define what a unit can do in battle. Tags are printed on unit cards and may be gained through tech research:

- **[Arty]** — may target any line from any line
- **[Defensive]** — may occupy the Defensive Line instead of Frontline
- **[Shields]** — provides damage reduction
- **[Space Cannon]** — long-range weapon; specific targeting rules per card

---

## Battle Structure

### 1. Prologue Phase
*Happens once, before Round I only.*

1. **Attacker fires all available prologue abilities** in any order they choose.
   - Prologue abilities come from: researched tech, special units carrying the ability, or permanent empire passives (e.g. *Fear Propaganda*).
2. **Defender responds** — only with abilities whose tech/unit card explicitly states it may be used as a defensive prologue response.
   - Without such tech, the defender absorbs the prologue silently.
3. **War Alliance partners** contribute their prologue abilities on their respective sides.

Prologue ability costs are defined per tech card. All prologue abilities are free during the current design phase.

---

### 2. Battle Rounds (I → II → III)

Battle rounds are tracked with tokens. Each side has a set: **I · + · II · + · III**

#### Each Battle Round:
1. **Attacker acts first** (initiative is always with the attacker unless a tech changes this).
2. Each player **assigns targets** to all their attacking units before any dice are rolled.
3. Players **roll dice and apply damage** simultaneously.
4. Damage flows strictly in sequence — **Frontline → Defensive Line → Reinforcement Line**.
   - A line must be completely empty before the next line takes any damage.
   - Exception: units with **[Arty]** may target any line directly, regardless of this sequence.

#### Between Rounds (the `+` token):
1. Each player may **push any number of units** from the Reinforcement Line into the Defensive Line or Frontline.
2. **Repair ships** activate their repair ability here *(cost TBD — see TODO)*.
3. Each player may declare **retreat or surrender** before the next round begins.

---

## Civilian Ships in Battle

Scouts and Colony Ships assigned to the Defensive Line are **destroyed immediately** when they are targeted. They have no combat ability and do not fight back.

---

## Win / Loss Conditions

A Space Battle ends when:
- All units on one side are **annihilated** (all three lines empty), or
- All remaining units on one side have **retreated**

**Surrender** — a player may surrender at any between-round window. All ships in the theatre are lost.

---

## Retreat

See [Retreat Rules](retreat.md) for the full retreat system.

Key points:
- Retreat must be declared in a between-round window; the fleet must have fought at least one full round first.
- The whole fleet retreats — no partial retreats.
- Retreating fleet must jump to an adjacent system containing at least one owned planet or a War Ally's planet.

---

## References

- [Fleet Card & Ship Types](../pieces/space/fleets.md)
- [Retreat Rules](retreat.md)
- [Landing](landing.md)
- [Conflict Overview](overview.md)
- [Allied Empires](../diplomacy/allied-empires.md)
