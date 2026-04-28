---
name: marketing-os-build-roadmap
description: Use when an operator has an Agentic Marketing OS maturity assessment in hand (or one can be done first) and needs a 90-day operating plan. Returns a week-by-week roadmap with the move per domain, who owns it, and what gets observed. Source — Mahmoud Halat, AMOS v3.
---

# Marketing OS — build a 90-day roadmap

Take a maturity assessment (or run [`assess-maturity.md`](./assess-maturity.md) first) and produce a week-by-week operating plan.

## Workflow

### Step 0 — Confirm inputs

You need three things. If any are missing, ask for them in one message:

1. **Current state per domain** — the assessment from `assess-maturity.md`. If absent, run that skill first.
2. **Team shape** — headcount, roles, budget bracket. Affects how many domains they can move at once.
3. **Quarter goal** — one sentence. Pipeline target, brand position, retention metric, whatever it is.

### Step 1 — Pick the moves

Don't try to move all eight domains at once. Pick **3 domains** for the quarter, max:

- **One Substrate move** — usually AgentOps (observability, eval, rollback) if it isn't in place yet. Without it, the other moves don't compound.
- **One Compounding move** — a domain whose advance unlocks 2-3 others. Sensing → Strategy → Content is a common chain. So is AI Search → Demand.
- **One Stretch move** — a domain currently at Crawl that the team's quarter goal directly depends on.

If they're already Run/Fly across the board, use the quarter to push **one domain** to the frontier (see [`research-plan.md`](../research-plan.md) for what's frontier-stage in v4).

### Step 2 — Decompose each move into weeks

Each domain move gets a 4-week structure. Don't invent the substance — pull the named *next move* from the relevant domain doc.

```
Week 1 — Diagnose & instrument
  - Read the domain canon + named case study
  - Stand up the eval / observability piece (AgentOps requirement)
  - Define the one metric you're moving

Week 2-3 — Build & ship
  - Implement the next move
  - Run against the eval
  - Iterate weekly

Week 4 — Review & decide
  - Did the metric move? Cite the data
  - If yes: lock in, advance one stage
  - If no: name the failure mode, decide stop/persist
```

### Step 3 — Output the roadmap

```
## Your 90-day Marketing OS roadmap

### Quarter goal
[Their one-sentence goal, restated]

### The three moves

**Move 1 — Substrate: AgentOps**
- Current → Target: [stage] → [stage]
- The move: [from 0-agentops.md]
- Owner: [role / name]
- Eval metric: [the one thing being measured]

**Move 2 — Compounding: [Domain name]**
- Current → Target: [stage] → [stage]
- The move: [from domain doc]
- Owner: [role / name]
- Eval metric: [metric]

**Move 3 — Stretch: [Domain name]**
- Current → Target: [stage] → [stage]
- The move: [from domain doc]
- Owner: [role / name]
- Eval metric: [metric]

### Week-by-week

| Week | Move 1 | Move 2 | Move 3 |
|---|---|---|---|
| 1 | Diagnose, stand up eval | Diagnose, instrument | Diagnose |
| 2 | Build | Build | Build |
| 3 | Ship + measure | Ship + measure | Ship + measure |
| 4 | Review | Review | Review |
| 5 | Iterate | Iterate | Iterate |
| ... | ... | ... | ... |
| 12 | Lock in / pivot | Lock in / pivot | Lock in / pivot |

### What's NOT in this plan (and why)

[List the 5 domains you didn't pick. State the reason for each — usually "not the highest leverage this quarter" or "depends on the substrate move landing first".]

### Stop conditions

- If [Move 1 metric] hasn't moved by Week 6, pause and re-instrument before continuing.
- If [Move 2 metric] is moving but the leading indicator [X] isn't, the move was wrong — switch.
- If your quarter goal is already de-risked by Week 8, accelerate one of the deferred domains instead of optimizing what's working.

### Source

*Operating cadence and domain content from the Agentic Marketing Operating System v3 by Mahmoud Halat. Full framework: https://mahmoudhalat.com/marketing-os*
```

## Don't

- **Don't promise outcomes.** This is a *process* roadmap, not a pipeline forecast. The framework doesn't claim deterministic outcomes per move.
- **Don't pick more than 3 domains** unless the team is 50+ people. Marketing teams under 50 that try to move 5+ domains fail at all of them.
- **Don't skip the eval setup in week 1.** A move you can't measure isn't a move; it's a guess.
- **Don't fabricate week-by-week tasks.** Pull the structure from the relevant domain doc; if a domain doesn't specify a week-1 instrumentation move, say so explicitly rather than inventing one.
