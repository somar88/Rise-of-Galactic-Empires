# RoGEs — Design Log

A living record of key design decisions, the reasoning behind them, and any alternatives that were considered and rejected. Updated at the end of every work session.

---

## How to use this file

Each entry follows this format:
- **Decision** — what was decided
- **Why** — the reasoning or concern that drove it
- **Alternatives considered** — what was rejected and why

---

## Session 1–2 — Core Game Loop & Structure

### Game loop: Action → Conflict → Draw, not fixed phases

**Decision:** The round is not a fixed sequence of phases. Instead, it is a repeating cycle: one player plays a card (Action), any resulting conflict is resolved immediately (Conflict), then the next player acts. When all hands are empty, everyone draws back to hand size. When all decks are fully exhausted, a Maintenance phase triggers.

**Why:** A fixed phase structure (everyone acts, then everyone conflicts) felt too sequential and slow. The interleaved loop keeps the game moving and makes each card play feel consequential immediately.

**Alternatives considered:**
- Draw after every card played → too frequent, disrupted pacing
- Draw only at Maintenance → hands ran dry too fast

---

### Galaxy size: Ring 3 only, 2–4 players

**Decision:** The galaxy is fixed at Ring 3 (37 hex tiles) for all player counts (2–4). No scaling to Ring 4.

**Why:** Keeping the galaxy at Ring 3 maintains a consistent board feel and avoids the complexity of variable map sizes. Ring 4 was proposed for 4 players but rejected — the designer wanted a tighter, more contested galaxy regardless of player count.

**Alternatives considered:**
- Ring 4 for 4 players → rejected, too spread out

---

## Session 2 — Movement

### Movement costs: destination ring number

**Decision:** Crossing from one star system to another costs movement steps equal to the destination ring number (Ring 1 = 1 step, Ring 2 = 2 steps, Ring 3 = 3 steps). Moving within a hex's outer rim sections costs 1 step per section (6 sections per hex edge).

**Why:** Creates a natural tension between the safety of inner rings and the cost of reaching outer systems. Fleets operating in the outer rim pay more per move, which rewards early expansion and punishes late pushes.

---

### Ship movement values: Scout 7, Fleet 5, Colony Ship 3

**Decision:** Scout = 7 movement steps, Fleet = 5, Colony Ship = 3.

**Why:** Initial values (Scout 6, Fleet 4, Colony Ship 2) were playtested and felt too slow — the designer felt the game would stagnate with units unable to cross the board in a reasonable number of turns. Values were bumped up one step across the board.

**Alternatives considered:**
- Scout 6 / Fleet 4 / Colony Ship 2 → rejected as too slow, risk of map stagnation

---

## Session 3 — Economy & Production

### Production flow: Buffer → Stance → Storage

**Decision:** When districts produce, all generated resources (CG, IG, Eco) go into a Production Buffer first. The player's current Economic Stance is then applied to the buffer (converting Eco into IG or CG, or leaving it unchanged). The final result moves into the Storage Area on the player tableau.

**Why:** The buffer step gives players a clear moment to see what they produced before the stance conversion is applied, and makes the stance choice feel meaningful each maintenance cycle.

---

### Three Economic Stances

**Decision:** Three stances — Militarization (converts Eco → IG), Growth (converts Eco → CG), Balanced (no conversion, everything stays as produced).

**Why:** Gives players a strategic lever to shift their economy each maintenance cycle without requiring a separate action. The Balanced stance was added after the designer confirmed it was needed — "yes there is a balanced one so everything stays the same."

---

### Resources: CG, IG, Eco

**Decision:** Three resource types: Consumer Goods (CG), Industrial Goods (IG), and Eco (Energy / Economic Power). Eco is the conversion currency affected by Economic Stance.

**Why:** Separating consumer and industrial goods creates distinct production roles for districts (civilian vs military economy) while Eco acts as the flexible resource that players shape via their stance.

---

## Session 4 — Civilian Actions

### Repair: half price, unlimited units per action

**Decision:** Repairing a unit or building costs half the price of building a new one. A player can repair any number of units in a single Repair action.

**Why:** Full price repair would make units disposable rather than worth maintaining. Allowing unlimited repairs per action means players don't need to spend multiple turns to recover from a battle — recovery should be meaningful but not a game-long slog.

---

### Build: 1 unit per action, at Star Dock

**Decision:** The Build civilian action produces one unit per action, and must be performed at a Star Dock.

**Why:** Limits snowballing — a player can't flood the board in a single turn. The Star Dock requirement means controlling key systems matters for military production.

**Note:** Advanced Star Dock tech (Culture & Infrastructure research arc) will unlock building 2 or 3 units per action.

---

### Story Arc: 1 per civilian action

**Decision:** A player may trigger one Story Arc event per civilian action.

**Why:** Keeps Story Arcs meaningful without letting players chain multiple narrative events in one turn.

---

### Repair location: TBD (playtest)

**Decision:** Where repairs can be performed (in-system only? anywhere?) is left unresolved pending playtesting. Marked 🧪 PLAYTEST in the rulebook.

**Why:** Not enough data yet on whether location restrictions add interesting decisions or just slow the game down.

---

## Session 5 — Research System

### Research: card-based decks, not a fixed tree

**Decision:** Research is driven by four card decks (Culture & Infrastructure, Economy, Diplomacy, Military) rather than a branching tech tree on a board. Each deck contains Standard cards (single unlock) and Arc cards (multi-step, partial benefits at each step).

**Why:** A fixed printed tech tree locks in the design and is hard to iterate. Card decks are modular — cards can be added, removed, or rebalanced without redesigning the board. Arc cards preserve the "tech tree" feel of progression without the rigidity.

**Alternatives considered:**
- Fixed tech tree grid on a board → rejected, too inflexible for a game still in design
- Single research deck → rejected, wanted thematic separation between domains

---

### Research action: Discover then Develop, both optional

**Decision:** The Research civilian action has two steps: Discover (draw one card from any deck into your Research Area) and Develop (fulfill one card's requirement to unlock it). Both steps are optional, but Discover always comes before Develop if both are taken.

**Why:** Separating discovery from development means players invest in a pipeline — they don't immediately get what they research. The ordering ensures you can't develop something you just discovered in the same action.

---

### Four research deck categories

**Decision:** Culture & Infrastructure (buildings, Star Dock, population), Economy (resources, trade, Eco conversion), Diplomacy (alliances, agreements, influence), Military / War (fleet combat, ship upgrades, FTL movement).

**Why:** Mirrors the four major domains of the game. Players can specialize or diversify depending on their strategy.

---

## Session 6 — Trade & Diplomacy

### Trade Agreements: token count = ½ players (rounded down)

**Decision:** The number of Trade Agreement tokens available equals half the number of players, rounded down (2 players = 1 token, 3 players = 1 token, 4 players = 2 tokens).

**Why:** Scarcity makes Trade Agreements meaningful choices rather than default behaviors. With few tokens, players must decide which relationships to formalize.

---

### Black Market: dynamic pricing, 20-unit capacity

**Decision:** The Black Market has a maximum capacity of 20 units each for CG and IG. Prices shift based on how much stock is on the market. New prices take effect only when an Exchange action is completed (not mid-action).

**Why:** Dynamic pricing creates a shared economic pressure — flooding the market drops prices, scarcity drives them up. The delayed price update (only after Exchange resolves) prevents mid-action price gaming.

---

### Trading: binding for resources, promissory is flexible

**Decision:** Trade agreements involving resource or star system exchanges are binding. Promissory agreements (future favors, non-immediate) are not binding unless both parties explicitly agree otherwise.

**Why:** Binding resource trades give the market stability and trust. Promissory notes being flexible allows for political dealmaking without rigid enforcement mechanics.

---

### What can be traded: almost anything

**Decision:** There are no limits on what can be traded — resources, star systems, armies, fleets, and even renting of units are all valid trade subjects.

**Why:** Open trading creates emergent diplomacy and complex deals. Restricting trade types would reduce political depth.

---

## Session 7 — Alliances

### Two independent alliance types: Economic and War

**Decision:** There are two distinct alliance types that are completely independent of each other — a player can have one, both, or neither with any given empire.

- **Economic Alliance:** Bilateral (both parties must agree), requires adjacency to form, provides economic benefits.
- **War Alliance:** Up to 3 players vs 1, not strictly bilateral, grants co-occupation rights in allied systems.

**Why:** Separating economic and military alliances reflects real-world complexity — trading partners aren't always military allies. Keeping them independent avoids forced bundling and allows more nuanced diplomacy.

**Alternatives considered:**
- Single alliance type covering both → rejected, conflated too many different relationships
- Threat agreements as alliances → rejected by designer: "A threat agreement is not an alliance"

---

### War Alliance: max 3v1

**Decision:** A War Alliance can involve at most 3 players attacking 1. No more than 3 allied attackers against a single target.

**Why:** Prevents complete pile-ons that would make the game feel unfair and eliminate any comeback potential for the defender.

---

## Session 8 — Conflict

### Battle pauses the main game

**Decision:** When a battle begins, the main game pauses for all players until the battle is fully resolved. No other actions take place while a battle is in progress.

**Why:** The designer specifically requested this — "if the players other players are waiting for the main players to do something, the game should stop until the battle is done." Prevents situations where spectating players are taking actions while others are mid-battle.

---

## Session 9 — Repository

### Repo structure: kebab-case, standard markdown links

**Decision:** The GitHub repository uses kebab-case filenames (e.g. `space-battle.md`, `black-market.md`), standard markdown links instead of Obsidian `[[wiki links]]`, and a clean folder hierarchy (rules/, conflict/, economy/, pieces/, diplomacy/, world/, tech-tree/, archive/).

**Why:** Obsidian wiki links only render in Obsidian. GitHub renders standard markdown. Kebab-case is the GitHub/web convention. The folder structure mirrors the game's conceptual domains.

---

### DESIGN-LOG.md: living document updated every session

**Decision:** This file is updated at the end of every work session to capture any new decisions made.

**Why:** Makes the repo fully self-contained — a Claude instance on any machine can read this file and understand not just what the rules say, but why they are the way they are.

---

## Session 10 — Space Battle, Retreat, Population & Districts

### Space Battle: three-line formation, always attacker-first

**Decision:** Every fleet arranges across three lines on the Fleet Card — Frontline (all combat ships), Defensive Line ([Defensive]-tagged units and all non-combat ships), Reinforcement Line (reserves). The attacker always acts first unless a tech changes this. Damage flows Frontline → Defensive → Reinforcement; a line must be empty before the next takes any hits. [Arty] units can skip the sequence and target any line.

**Why:** Three lines create tactical depth without complexity. Making damage flow sequential (rather than distributing freely) gives frontline ships real meaning. Arty as a line-skip exception creates a distinct role worth paying for.

---

### Space Battle: Prologue Phase (once, before Round I)

**Decision:** Before battle rounds begin, the attacker may fire all available prologue abilities (from tech, special units, or empire passives). The defender may respond only with abilities whose card explicitly states they can be used as a defensive prologue response. War Alliance partners contribute on their respective sides. All prologue costs are per card (currently free during design phase).

**Why:** The designer asked for a pre-battle ability window ("a prolog for the battle"). Making it attacker-first by default is consistent with the broader initiative rule. Defender responses are opt-in only to avoid a lengthy negotiation over "can I respond to this?"

**Alternatives considered:**
- Both sides fire prologue simultaneously → muddied initiative concept
- Prologue for defender too by default → too much symmetry, lost the attacker advantage feel

---

### Space Battle: Battle Phase tokens I·+·II·+·III

**Decision:** Each side uses a set of tokens: I · + · II · + · III. The + token marks the between-round window where players push reinforcements, repair ships act, and retreat/surrender can be declared. A fleet must have fought at least one full round before retreat can be declared.

**Why:** Physical tokens make the round progression unambiguous during play. The + token explicitly represents the "breathing room" between rounds — a natural slot for all between-round decisions.

---

### Retreat: whole fleet, between-round only, adjacent systems only (default)

**Decision:** Retreat can only be declared during a + (between-round) window, after at least one full round has been fought. The entire fleet retreats together — no partial retreats. By default, retreat is limited to immediately adjacent systems. Retreating into an adjacent owned/ally system is free; retreating into an adjacent empty discovered system incurs a penalty roll. Undiscovered systems are never valid.

**Why:** "Between rounds" was the designer's explicit timing. Whole-fleet retreat avoids fiddly partial-fleet state. Adjacent-only is the safe default to playtest first.

**Alternatives considered:**
- Retreat at any time → breaks battle structure
- Partial fleet retreat → logistically complex for components
- Extended jumps freely → leaves retreat too safe

**Open:** Extended retreat jumps via tech or die rolls (playtest TODO). Interception via future tech (Military deck TODO).

---

### Ground Retreat: requires carrier, player chooses who boards

**Decision:** Ground units cannot retreat on their own. At least one Carrier must be present (or have survived) in the space theatre. The player chooses which units to board up to carrier capacity; units that don't board surrender and are lost. Ground retreat is declared independently from space retreat.

**Why:** The designer specified carriers as the only escape vector. Player choice of which units to save adds a meaningful decision under pressure.

---

### Population: three colors — Blue (CG), Green (Eco), Orange (IG)

**Decision:** Three pop token colors map directly to the three resource types: Blue = Consumer Goods (CG), Green = Ecological/Economy (Eco), Orange = Industrial Goods (IG).

**Why:** Direct color-to-resource mapping makes the production indicator system visually intuitive.

---

### Districts: Small/Medium/Large sizes; Single/Dual/Omni token types

**Decision:** Districts come in three sizes (Small=1 slot, Medium=2 slots, Large=3 slots) and three type tokens (Single-color, Dual two-color, Omni gold). A district produces nothing until fully filled. Filling the last slot triggers an immediate production indicator adjustment.

**Why:** Partial districts not contributing until full creates a satisfying "district completion" moment and makes size a real decision. Dual and Omni districts create planet variety without needing many different token types.

---

### Populate action: one pop per action (default)

**Decision:** The Populate action places exactly one population token per use. "A CG pop", "an Eco pop", "an IG pop" — singular. IG pops may only be placed when all CG and Eco district slots on the planet are already filled (with an exception for pure-IG planets). Eco district pops cost 1× CG (same as CG pops). IG pops cost 1× CG + 1× Eco.

**Why:** "A/an" wording in the original design note confirmed singular. Limiting IG placement protects the resource ordering (CG and Eco fill first, industry comes after).

**IDEA POOL:** Tech tree ability to place more than one pop per Populate action. Tier and cost TBD.

---

### Black Market tracker: dual sliding track, color-coded price bands

**Decision:** Physical component is a dual sliding track board with two sections (2-player / 3+ player). Each section has two rows (CG and IG), numbered 0–20, with a sliding cube marking the current amount. Price bands are color-coded — Red (highest/scarce) → Orange → Yellow → Green (lowest/flooded) — for instant readability without scanning numbers. Prices lock during a transaction and only update after the Exchange action resolves.

**Why:** Sliding cube is the simplest physical mechanism for a 0–20 range. Color coding removes the need to read numbers mid-game. Two-section board avoids needing a separate component for player count variants.

---

### Nepiru: 5 golden districts, 3-step branching Story Arc

**Decision:** Nepiru has 5 Golden Districts producing at 2× output, fully automated (no pop tokens needed). The Story Arc activates on first capture — player chooses one of three paths (Excavation, Reactivation, Communion), each with 3 steps. One step advances per Maintenance Phase held. Completing all 3 steps coincides with the Moral Victory condition. On conquest, new owner inherits the arc at its current state; resetting to the branch point costs 1 step. Step 3 of Reactivation grants 3 free mechanized units (no Space Marines).

**Why:** 5 districts at 2× makes Nepiru decisively powerful without being infinite. 3 steps rhymes with the 3 consecutive phases for Moral Victory — arc completion and win condition are the same moment. Branching paths give replayability. Inherited arc on conquest keeps the tension alive — you benefit from someone else's progress, or pay a cost to change direction.

---

### Trade Agreements: open-ended, free cancellation, 1 slot default with tech expansion

**Decision:** Trade Agreements are open-ended with no fixed duration. Either player can cancel at any time at no action cost — both return their tokens immediately. Each empire starts with 1 Trade Agreement slot; additional slots unlocked via Economic tech. A physical token on each player's tableau marks the active agreement.

**Why:** Open-ended agreements feel more like real diplomatic relationships. Free cancellation keeps diplomacy fluid. Starting at 1 slot forces a genuine choice about who your economic partner is early game, while tech expansion rewards investment in economic research.

**Alternatives considered:**
- Fixed duration (X rounds) → felt arbitrary, created awkward timing
- No limit → removes the strategic choice entirely
- Penalty for cancellation → too punishing, discourages diplomacy

**New TODO:** Tech to increase Trade Agreement slots — Economic research deck.

---

### Maintenance costs: per fleet, per solo ship, per planet with units/buildings

**Decision:** Fleet away from owned/ally system: 1× CG + 1× IG. Solo ship not on a friendly planet: 1× IG per ship (playtest flag: may switch to Eco). Planet with ground units: 1× CG flat. Planet with ground buildings: 1× IG flat. Districts have no maintenance — their net production already reflects running costs. Can't pay → trade first, then skip and draw one Chaos Card per unpaid fleet/planet.

**Why:** Flat per-fleet and per-planet costs keep bookkeeping fast. CG for troops (they need supplies), IG for buildings (machines need fuel). No district maintenance avoids double-counting since district output already nets against consumption.

**Playtest flag:** Solo ship cost IG vs Eco — test both.

---

### Recruit Ground Units: IG district cap, CG pop per unit, Tier I only

**Decision:** Recruitment can happen across any number of star systems in one Civilian action. Each system requires at least one populated IG district (unlocks recruitment) and at least one CG pop (consumed per unit). Maximum units per system = number of populated IG districts. Any unit type may be recruited. Tier I only — Tier II requires the Upgrade action unless a tech changes this.

**Why:** Tying the cap to populated IG districts makes industrial investment directly reward military output. Consuming a CG pop per unit creates a real tension between growing your population and building your army. Multi-system recruitment in one action keeps the civilian action feel expansive without needing multiple turns to build up.

**New TODO:** Tech that unlocks direct Tier II recruitment — Military or Industrial research deck.

---

### Landing: carrier capacity, shield break roll, defense fire sequence

**Decision:** Each Carrier holds 3 points of ground unit cargo (stackable across multiple carriers). Space Marines and Marines Special Forces = size 1; Armored Vehicles, Advanced AVs, and Mobile Artillery = size 2. The same capacity applies to ground retreat boarding. Landing sequence: pre-abilities → Planetary Shield check (D6: 4–6 destroys it, 1–3 cancels landing) → all planetary defenses fire simultaneously (attacker assigns hits) → survivors land with damage → Ground Battle begins if any units survive. If no units survive defense fire, no Ground Battle.

**Why:** Stacking capacity per carrier rewards fleet composition decisions. Size 1 for marines keeps them cheap to transport; size 2 for heavy units creates a real tradeoff. 50% shield break (D6 4–6) is the base — meaningful risk without making the shield feel unbreakable. Attacker assigns hits to preserve player agency under fire.

**Alternatives considered:**
- Fixed fleet capacity regardless of carrier count → removes carrier count as a meaningful decision
- Defender assigns hits → too punishing, attacker has no agency
- Automatic shield destruction with a hero present → no tension, just a checkbox

**New TODO:** Tech upgrades for the shield-breaking roll (reroll, +1 bonus, auto-success) — Military research deck.

---

### Retreat Die: D12, 30% bad outcomes, flat 1 damage or Chaos Card

**Decision:** The Retreat Die is a D12. Rolls 1–8 (67%) are no effect. Rolls 9–11 (25%) deal 1 damage to a ship of the retreating player's choice. Roll 12 (8%) triggers a Chaos Card draw. Total bad outcome chance: ~33%, targeting the 30% design goal. The same die is used for retreating into an empty discovered system and for each extra system jumped through on an extended retreat.

**Why:** D12 gives the cleanest whole-number split near 30%. Flat 1 damage (rather than ship loss) keeps the penalty meaningful but not devastating — a punishing result that doesn't end a fleet. Player chooses the target ship to preserve agency. One Chaos Card face adds unpredictability without making the die feel purely mechanical.

**Alternatives considered:**
- D6 → couldn't hit 30% cleanly; too coarse
- Instant ship loss → too punishing for a tactical retreat decision
- Graduated faces (worse as number climbs) → adds complexity without much payoff

---

### District Switching: during Populate action only; upgrade costs Eco, downgrade free

**Decision:** A player may switch a district's color type as part of the Populate action (before placing the pop). Upgrade direction (CG→Eco, Eco→IG, CG→IG) costs 1× Eco per step. Downgrade is free. Existing pops of the old color are removed and returned to supply when switching. Switching can only happen during the Populate action.

**Why:** Restricting switching to the Populate action prevents it from becoming a free mid-round restructure. Eco cost for upgrades creates a meaningful spend. Free downgrade avoids punishing players who need to reset.

---

## Open Design Questions (as of 2026-05-07)

These are known unknowns — decisions not yet made:

- ~~**Landing / Planet Fall**~~ ✅ Resolved (Session 10)
- ~~**Recruit Ground Units**~~ ✅ Resolved (Session 10)
- **Chaos Card system** — draw triggers, resolution timing, instant vs persistent, multi-card holding
- **Tech Tree content** — actual card names, requirements, and effects for all four decks; including:
  - Interception of retreating fleets (Military deck)
  - Extended retreat jump range beyond adjacent system
  - Repair ship action cost
  - Place more than one pop per Populate action
- **Recruit Ground Units** — multi-unit per action? exact location requirements?
- ~~**Maintenance costs**~~ ✅ Resolved (Session 10)
- ~~**Trade Agreement duration/cancellation**~~ ✅ Resolved (Session 10)
- ~~**Black Market tracker**~~ ✅ Resolved (Session 10)
- **Anomaly types** — specific effects, movement penalties, arc designs
- **Moon and Giant Planet card properties**
- ~~**Nepiru golden districts count and Story Arc**~~ ✅ Resolved (Session 10)
- **FTL tech tiers** — upgrade levels and step bonuses
- **Star Dock capacity upgrade** — which tech unlocks it, how many extra ships per action
- **Repair location** — in-system only or anywhere? (🧪 PLAYTEST)
- ~~**Extended retreat penalty die**~~ ✅ Resolved (Session 10)
- **Colonization: pop transformation rule** — "if no matching districts in whole star system, pop must be transformed" — what does transformation cost/look like?
