# Retreat from Conflict

Retreat is a free tactical decision — there is no resource cost or penalty for choosing to retreat. It applies independently to Space and Ground battle theatres.

---

## Space Battle Retreat

### When Retreat Can Be Declared
- Only during a **between-round window** (the `+` token phase).
- The fleet must have **fought at least one full battle round** before retreat can be declared. A fleet that has not yet fired cannot immediately retreat.

### Who Retreats
- The **entire fleet** retreats — no partial retreats. Whatever ships remain on all three lines leave together.

### Where to Retreat
Retreating fleets must jump to a **valid destination system**:

| Destination | Result |
|---|---|
| Adjacent system with an owned planet or War Ally's planet | ✅ Safe — no penalty |
| Adjacent empty discovered system | ⚠️ Penalty — roll the Retreat Die |
| Further than adjacent (default) | ❌ Not allowed |
| Any undiscovered system | ❌ Never allowed |

### The Retreat Die

When a penalty roll is required, roll a **D12** and consult the table:

| Roll | Result |
|---|---|
| 1–8 | ✅ No effect — clean escape |
| 9–11 | 💥 One ship of your choice in the fleet takes **1 damage** |
| 12 | 🃏 Draw a **Chaos Card** |

The damaged ship is not destroyed unless it was already at 1 hit point. The player chooses which ship takes the damage.

### Extended Retreat Jumps
By default, retreat is limited to **immediately adjacent** systems only.

Extended jumps (beyond adjacent) may become possible through **Tech** — a researched ability that explicitly extends retreat range. For each additional system jumped through beyond the first, roll the Retreat Die once.

> 📋 **TODO (Tech Tree):** Design the tech that unlocks extended retreat jumps. Add to Military research deck.

### Interception
By default, a retreating fleet **cannot be intercepted**.

> 📋 **TODO (Tech Tree):** Design a tech or lore ability that allows a player to intercept retreating fleets. Add to Military research deck.

---

## Ground Battle Retreat

Ground units **cannot retreat on their own**. They require carrier support from the space theatre above.

### Conditions for Ground Retreat
- At least one **Carrier** must be present in the space battle (or have survived it).
- Ground retreat is declared independently from space retreat — retreating in space does not automatically retreat ground units, and vice versa.

### How Ground Retreat Works
1. The player declares which ground units will board the carrier(s).
2. Units board up to **carrier capacity** — the player chooses which units to load.
3. Ground units that do not fit (or are not selected) **surrender and are lost**.
4. Boarded units travel with the retreating fleet to its destination system.

### No Carrier = No Escape
If no carrier is available in the space theatre, ground units **fight to the end or surrender**. There is no other option.

### Surrender
At any between-round window a player may **surrender** their ground forces. All ground units in the theatre are lost.

---

## Summary Table

| | Space Battle | Ground Battle |
|---|---|---|
| **When** | Between rounds, after ≥1 round fought | Between rounds, after ≥1 round fought |
| **Who** | Whole fleet | Carrier-loaded units only; rest surrender |
| **Cost** | Free | Free |
| **Destination** | Adjacent owned/ally system (penalty if empty) | Boards carrier; travels with fleet |
| **Interception** | Not possible (default) | N/A |
| **No valid escape** | Must surrender | Must fight to end or surrender |

---

## References

- [Space Battle](space-battle.md)
- [Ground Battle](ground-battle.md)
- [Allied Empires](../diplomacy/allied-empires.md)
- [Conflict Overview](overview.md)
