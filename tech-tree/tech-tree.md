
2026-04-26

Status: Draft — Structure defined, card content TBD

Tags: #RoGEs #design #tech-tree #research

# Tech Tree — Research System

## Overview

Research is driven by **four Research Decks**, one per category. Players draw from these decks and develop them through the **Research** Civilian action.

Each deck contains cards of two types:
- **Standard Tech Cards** — unlocked in a single Develop step
- **Research Arc Cards** — multi-step tech trees; each step unlocks a partial benefit. Players can stop at any depth.

---

## The Research Action

The Research Civilian action always follows this sequence:

1. **Discover** *(optional)* — Draw one card from any one Research Deck and place it face-up in your **Research Area** on your player tableau.
2. **Develop** *(optional)* — Fulfill the requirements on one card already in your Research Area to unlock its effect (or advance it one step if it is an Arc card).

A player may do **both steps**, or **only one**, but Discover always comes before Develop in the same action.

---

## Research Card Format

### Standard Tech Card
```
┌─────────────────────────────────┐
│  [DECK CATEGORY]                │
│                                 │
│  Tech Name                      │
│                                 │
│  Requirement:                   │
│  [What must be fulfilled]       │
│                                 │
│  Effect:                        │
│  [What is permanently unlocked] │
│                                 │
│  Prerequisite: [Tech name / —]  │
└─────────────────────────────────┘
```

### Research Arc Card
```
┌─────────────────────────────────┐
│  [DECK CATEGORY]          ARC   │
│                                 │
│  Arc Name                       │
│                                 │
│  Step 1 — Requirement: [...]    │
│           Effect: [...]         │
│                                 │
│  Step 2 — Requirement: [...]    │
│           Effect: [...]         │
│                                 │
│  Step 3 — Requirement: [...]    │
│           Effect: [...]         │
│                                 │
│  (Player may stop at any step)  │
└─────────────────────────────────┘
```

---

## Research Decks

---

### 🏛️ Culture & Infrastructure

Covers buildings, Star Dock upgrades, population growth, and structural development.

| # | Name | Type | Requirement | Effect |
|---|------|------|-------------|--------|
| C1 | [Tech Name] | Standard | [e.g. Control 3+ star systems] | [Effect TBD] |
| C2 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| C3 | Advanced Star Dock | Arc | Step 1: [Req] → Build 2 ships per action / Step 2: [Req] → Build 3 ships per action / Step 3: [Req] → [Effect TBD] | See steps |
| C4 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| C5 | [Arc Name] | Arc | [Steps TBD] | [Effect TBD] |

---

### 💰 Economy

Covers resource production, economic stances, trade, and Eco conversion efficiency.

| # | Name | Type | Requirement | Effect |
|---|------|------|-------------|--------|
| E1 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| E2 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| E3 | [Arc Name] | Arc | [Steps TBD] | [Effect TBD] |
| E4 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| E5 | [Arc Name] | Arc | [Steps TBD] | [Effect TBD] |

---

### 🤝 Diplomacy

Covers alliances, trade agreements, political influence, and inter-empire relations.

| # | Name | Type | Requirement | Effect |
|---|------|------|-------------|--------|
| D1 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| D2 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| D3 | [Arc Name] | Arc | [Steps TBD] | [Effect TBD] |
| D4 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| D5 | [Arc Name] | Arc | [Steps TBD] | [Effect TBD] |

---

### ⚔️ Military (War)

Covers fleet combat, ship upgrades, ground unit improvements, and FTL movement.

| # | Name | Type | Requirement | Effect |
|---|------|------|-------------|--------|
| M1 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| M2 | FTL Drive I | Standard | [Requirement TBD] | +1 movement step to all ships |
| M3 | FTL Drive | Arc | Step 1: [Req] → +1 step / Step 2: [Req] → +2 steps / Step 3: [Req] → +3 steps | See steps |
| M4 | [Tech Name] | Standard | [Requirement TBD] | [Effect TBD] |
| M5 | [Arc Name] | Arc | [Steps TBD] | [Effect TBD] |

---

## Open Design Questions

- [ ] How many cards per deck? (Suggested: 8–12 per deck)
- [ ] Are all decks available to all empires, or are some decks locked per empire?
- [ ] Can a player hold unlimited discovered cards in their Research Area, or is there a hand limit?
- [ ] What happens to a partially developed Arc card if the player is eliminated?
- [ ] Can two players develop the same tech, or is it a first-come race?
- [ ] Should requirements be resource costs, conditions (e.g. "control 3 systems"), or a mix of both?

---

# References

- [RoGEs Rulebook](../RULEBOOK.md)
- [Action Card - Civilian](../rules/player-actions/civilian.md)
- [Star dock](../pieces/space/star-dock.md)
