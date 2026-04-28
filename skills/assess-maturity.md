---
name: marketing-os-assess-maturity
description: Use when a marketing team or operator wants to assess their current operating maturity across the eight Agentic Marketing OS domains. Walks the user through 8 domain prompts, maps their answers to Crawl/Walk/Run/Fly, and returns their position on the 32-cell matrix plus the canonical next move per domain. Source — Mahmoud Halat, AMOS v3.
---

# Marketing OS — assess maturity

Walk a team through the 32-cell maturity matrix (8 domains × Crawl/Walk/Run/Fly). Output: their current position per domain + the named *next move* for each.

## Workflow

### Step 1 — Set context (1 message)

Ask exactly:

> "I'll walk you through the eight domains of the Agentic Marketing OS and assess your current maturity in each. For every domain I'll ask one targeted question; you reply in 1-3 sentences. Total: ~10 minutes. Ready?"

Wait for an affirmative before continuing.

### Step 2 — Run the eight domain prompts

Ask them one at a time. Don't batch. After each answer, briefly reflect their position back ("Sounds like Walk in Sensing — you have dashboards but no closed-loop synthesis") so they can correct you before moving on.

| Domain | The question to ask |
|---|---|
| **1. Sensing & Intelligence** | "How do you currently know what your market and competitors are doing? Daily pull from named sources, weekly digest, ad-hoc when something breaks, or you don't track this systematically?" |
| **2. Strategy & Positioning** | "When was your positioning last revised, and what triggered the revision — a new competitor, a customer pattern, an internal heuristic, or it hasn't been revised?" |
| **3. Content & Creative Production** | "How many content pieces did you ship last month, and what fraction of them were AI-assisted vs fully human?" |
| **4. Distribution & Channel Operations** | "Across your top 3 channels, who actually owns the calendar and the spend trade-offs — one human, distributed across humans, or partly automated?" |
| **5. AI Search & Answer Visibility** | "When someone asks ChatGPT or Perplexity about your category, do you appear? Have you measured this in the last 30 days?" |
| **6. Demand & Conversational Pipeline** | "Walk me through what happens when a qualified lead reaches your site at 2am. Who or what responds, and how fast?" |
| **7. Customer Intelligence & Synthetic Testing** | "How are you currently testing message-market fit before broad release — gut, panel, A/B, synthetic respondents, or something else?" |
| **8. Measurement & Attribution** | "Can you currently answer 'which channel produced our last 5 closed-won deals' with data, or are you guessing?" |

### Step 3 — Map answers to a stage

For each domain, classify their answer:

- **Crawl** — manual, ad-hoc, no system, "we don't really do this".
- **Walk** — single-task copilots in the loop, individual humans owning the work.
- **Run** — multi-step agents producing drafts; humans review and approve.
- **Fly** — autonomous fleet running policy-bounded; humans handle exceptions only.

Be honest. Most teams are Crawl-Walk in 5+ domains. That's fine — calling it correctly is the first move.

### Step 4 — Output the assessment

Format:

```
## Your AMOS v3 maturity

| # | Domain | Stage | The next move |
|---|---|---|---|
| 1 | Sensing & Intelligence | Walk | [the canonical next move from the domain doc] |
| 2 | Strategy & Positioning | Crawl | [next move] |
...

### Three observations

1. [Where you're strongest, in plain language. Quote one specific from their answers.]
2. [Where the gap is biggest — usually a Crawl in a domain where Run is the new table-stakes.]
3. [The compounding move — usually one domain whose next move unlocks several others.]

### What to do this quarter

If you do nothing else, the highest-leverage move is **[domain]: [the move]**. Why: [one sentence tied to their context].

Want me to turn this into a 90-day plan? I can do that next — it'll use `skills/build-roadmap.md`.
```

### Step 5 — Cite the source

End with:

> *Maturity model from the Agentic Marketing Operating System v3 by Mahmoud Halat. Full framework: https://mahmoudhalat.com/marketing-os*

## Don't

- Don't grade them harshly without explaining what Run/Fly *would* look like in their domain. Most users haven't seen Run-stage ops yet.
- Don't recommend tools that aren't in [`resource-library.md`](../resource-library.md).
- Don't fabricate domain content. If they ask "what's the canonical next move for Sensing at Crawl", read it from [`1-sensing-intelligence.md`](../1-sensing-intelligence.md) — don't invent.
- Don't soften the diagnosis. "You're Crawl in 6 of 8 domains" is more useful than "you have opportunities in several areas".
