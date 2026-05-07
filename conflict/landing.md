# Landing

Landing is the process of deploying ground units from carrier ships onto a planet surface. It triggers a Ground Battle if any units survive the landing.

Landing can occur in two contexts:
- **Deployment** — initial landing at the start of an engagement
- **Reinforcement** — additional units landed from carriers still present after a Space Battle round

Both use the same sequence.

---

## Carrier Capacity

Each Carrier ship holds up to **3 points** of ground unit cargo.

| Unit | Size |
|---|---|
| Space Marines (Tier I) | 1 |
| Marines Special Forces (Tier II) | 1 |
| Armored Vehicle (Tier I) | 2 |
| Advanced Armored Vehicle (Tier II) | 2 |
| Mobile Artillery | 2 |

Multiple carriers in the same fleet **stack** their capacity. A fleet with 2 carriers can transport up to 6 points of ground units.

> The same capacity rules apply when loading ground units during a [Retreat](retreat.md) — units board up to total carrier capacity; the rest surrender.

---

## Landing Sequence

### Step 1 — Pre-Landing Abilities

Both the attacking and defending player may activate any abilities that explicitly trigger at the start of a landing/deployment phase (hero abilities, tech, empire passives).

#### Planetary Shield Check

If the defending player has a **Planetary Shield** on the target planet, it must be destroyed before any landing can proceed.

- The attacking player may use a **Hero Unit or Hero Ship** ability to attempt to destroy the shield.
- Roll **1D6**:

| Roll | Result |
|---|---|
| 4–6 | ✅ Shield destroyed — landing continues |
| 1–3 | ❌ Shield holds — landing is cancelled |

If the shield is not destroyed, the landing attempt ends here. No ground units are deployed and no Ground Battle takes place.

> 📋 **TODO (Tech Tree):** Design tech upgrades that improve the hero's shield-breaking roll (e.g. reroll, +1 bonus, automatic success). Add to Military research deck.

---

### Step 2 — Planetary Defenses Fire

All active **planetary defense structures** (e.g. Defense Artillery Systems) fire simultaneously at the landing units.

- The **attacker** chooses which of their landing units takes each hit.
- Each defense structure fires **once per landing attempt**.
- Damage is applied immediately — units do not fire back during this step.

---

### Step 3 — Units Land

All surviving ground units land on the planet surface, carrying any damage they sustained during Step 2.

If **no units survive** the planetary defense fire, the landing ends here — no Ground Battle takes place.

---

### Step 4 — Ground Battle

If at least one unit survived landing, a [Ground Battle](ground-battle.md) begins immediately.

---

## Summary

| Step | What Happens |
|---|---|
| 1 — Pre-abilities | Both sides activate landing-phase abilities; hero may attempt to destroy Planetary Shield |
| Shield check | D6: 4–6 shield down, landing continues; 1–3 shield holds, landing cancelled |
| 2 — Defense fire | All planetary defenses fire simultaneously; attacker assigns hits |
| 3 — Land | Survivors land with damage; if none survive, no Ground Battle |
| 4 — Ground Battle | Begins if any units are on the ground |

---

## References

- [Space Battle](space-battle.md)
- [Ground Battle](ground-battle.md)
- [Retreat](retreat.md)
- [Ground Structures](../pieces/ground/ground-structures.md)
- [Ground Forces](../pieces/ground/ground-forces.md)
- [Conflict Overview](overview.md)
