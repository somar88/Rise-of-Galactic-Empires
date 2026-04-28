# Rise of Galactic Empires (RoGEs)

A hex-based space empire board game for 2–4 players. Build your empire, command fleets, trade across the galaxy, forge alliances, and race to victory across a Ring 3 galaxy of 37 star systems.

---

## Quick Navigation

| Section | Description |
|---|---|
| [RULEBOOK.md](RULEBOOK.md) | The complete, authoritative rulebook |
| [TODO.md](TODO.md) | Open design questions and backlog |

---

## Repository Structure

```
├── RULEBOOK.md                        # Master rulebook — start here
├── TODO.md                            # Design backlog
│
├── rules/                             # Core rules reference
│   ├── general.md
│   ├── game-round.md                  # The Action → Conflict → Draw loop
│   ├── setup.md
│   ├── victory-conditions.md
│   ├── movement.md                    # Movement costs & ship speeds
│   ├── hand-size.md
│   ├── player-order.md
│   ├── docking-area.md
│   ├── maintenance.md
│   ├── enhancers.md
│   ├── galaxy-setup.md
│   ├── player-setup.md
│   │
│   ├── round-phases/
│   │   ├── action-phase.md
│   │   ├── conflict-phase.md
│   │   └── maintenance-phase.md
│   │
│   └── player-actions/
│       ├── civilian.md                # Build, Repair, Research, Story Arc…
│       ├── exchange.md                # Trade & diplomacy actions
│       ├── mobilization.md
│       ├── production.md
│       └── empire-cards.md
│
├── conflict/                          # Battle rules
│   ├── overview.md
│   ├── space-battle.md
│   ├── ground-battle.md
│   ├── landing.md
│   ├── planet-fall.md
│   ├── retreat.md
│   ├── between-battles.md
│   └── damage/
│       ├── units.md
│       └── buildings.md
│
├── economy/                           # Resources, production & trade
│   ├── overview.md
│   ├── resources.md                   # CG, IG, Eco
│   ├── economic-stance.md             # Militarization / Growth / Balanced
│   ├── black-market.md
│   └── goods.md
│
├── pieces/                            # Physical game components
│   ├── player-tableau.md
│   ├── cards/                         # All card types
│   ├── space/                         # Fleets, Scouts, Colony Ships, Star Dock…
│   └── ground/                        # Ground forces & structures
│
├── diplomacy/                         # Alliances & politics
│   ├── allied-empires.md              # Economic & War Alliances
│   ├── allied-armies.md
│   └── politics.md
│
├── world/                             # Galaxy & star systems
│   ├── overview.md
│   ├── anomaly-tiles.md
│   ├── outer-rim.md
│   └── exploration-colonization/
│       ├── exploration.md
│       └── colonization.md
│
├── tech-tree/
│   └── tech-tree.md                   # Research decks & card templates
│
└── archive/                           # Early design drafts (kept for reference)
```

---

## Design at a Glance

- **Players:** 2–4
- **Galaxy:** Ring 3 — 37 hex tiles
- **Game loop:** Repeating **Action → Conflict → Draw** cycles until all decks are exhausted, then **Maintenance**
- **Resources:** Consumer Goods (CG) · Industrial Goods (IG) · Eco (Energy/Economic Power)
- **Ships:** Scout (7 steps) · Fleet (5 steps) · Colony Ship (3 steps)
- **Research:** Four decks — Culture & Infrastructure · Economy · Diplomacy · Military

---

## Status

This project is in active design and playtesting. Many sections are drafts with open design questions marked `🧪 PLAYTEST` or `TODO`.
