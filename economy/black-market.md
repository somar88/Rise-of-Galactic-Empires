# Black Market

The Black Market is a neutral trading system where players can buy and sell Consumer Goods (CG) and Industrial Goods (IG) at prices determined by supply and demand. It is accessed through the [Exchange action](../rules/player-actions/exchange.md).

---

## The Black Market Tracker (Physical Component)

The Black Market Tracker is a dual sliding track board. It has two sections — one for **2 Players** and one for **3+ Players** — players use the appropriate section for their game.

Each section has two parallel rows:
- **Top row** — Consumer Goods (CG)
- **Bottom row** — Industrial Goods (IG)

Each row has numbered slots from **0 to 20**, representing how many resources are currently held on the market. A **sliding cube** on each row marks the current amount.

### Color Coding
Each price band zone on the track is color-coded for instant readability — players can see the current price at a glance without needing to read the numbers below:

| Color | Price |
|---|---|
| 🔴 Red | Highest price (market is scarce) |
| 🟠 Orange | High price |
| 🟡 Yellow | Mid price |
| 🟢 Green | Low price (market is flooded) |

---

## Capacity

The Black Market holds a maximum of **20 resources** for both CG and IG. If resources exceed the cap, all additional resources go to the bank instead — but the market will still accept purchases at the cap price.

---

## Pricing

Prices are determined by how many resources are currently on the market. More supply = lower price. Less supply = higher price.

### 2 Players

| Resources on Market | CG Price | IG Price |
|---|---|---|
| 1 – 5 | 4 | — |
| 1 – 4 | — | 5 |
| 5 – 8 | — | 4 |
| 6 – 10 | 3 | — |
| 9 – 12 | — | 3 |
| 11 – 15 | 2 | — |
| 13 – 16 | — | 2 |
| 16 – 20 | 1 | — |
| 17 – 20 | — | 1 |

### 3+ Players

| Resources on Market | CG Price | IG Price |
|---|---|---|
| 1 – 7 | 3 | — |
| 1 – 5 | — | 4 |
| 6 – 10 | — | 3 |
| 8 – 14 | 2 | — |
| 11 – 15 | — | 2 |
| 15 – 20 | 1 | — |
| 16 – 20 | — | 1 |

---

## Rules

- Players buy and sell at the **current price** shown on the tracker.
- Prices are **locked during a transaction** — the new price only activates after the Exchange action is fully resolved.
- The market starts at **0** (empty) at the beginning of the game.
- Resources sold to the market move the cube up; resources bought move it down.

---

## References

- [Exchange Action](../rules/player-actions/exchange.md)
- [Resources](resources.md)
- [Economy Overview](overview.md)
