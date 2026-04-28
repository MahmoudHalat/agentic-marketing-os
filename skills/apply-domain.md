---
name: marketing-os-apply-domain
description: Use when an operator wants to take a single Agentic Marketing OS domain and apply it to a specific company / product / situation. Outputs the named tools, case-study analogue, and concrete next move tailored to their context. Source — Mahmoud Halat, AMOS v3.
---

# Marketing OS — apply a domain

Take ONE of the eight domains and apply it concretely to a specific product or company. Output: the named tools that fit their stack, the closest case-study analogue, the next move with the canonical pitfall called out.

## Workflow

### Step 1 — Confirm the domain + the context

Ask in ONE message:

> "Which domain do you want to apply? (1) Sensing & Intelligence, (2) Strategy & Positioning, (3) Content & Creative Production, (4) Distribution & Channel Operations, (5) AI Search & Answer Visibility, (6) Demand & Conversational Pipeline, (7) Customer Intelligence & Synthetic Testing, (8) Measurement & Attribution.
>
> Then: tell me about your product in 3 lines — what it is, who it's for, and what stage you're at (pre-PMF, scaling, mature). I'll tailor the domain content to your context."

### Step 2 — Load only the relevant domain file

Don't load all eight. Load:
- The selected domain file (e.g., [`5-ai-search-answer-visibility.md`](../5-ai-search-answer-visibility.md))
- [`resource-library.md`](../resource-library.md) — the vetted tool list

### Step 3 — Match their context to the framework

Identify in their answer:

- **Stage**: pre-PMF / scaling / mature → determines Crawl/Walk/Run/Fly target
- **Audience shape**: B2B / B2C / B2B2C / regulated → narrows tool list
- **Resource profile**: solo / lean / mid / large team → narrows next-move scope
- **Closest case-study analogue**: from the named cases in the domain doc

### Step 4 — Output the application

```
## Applying [Domain N: Name] to [their company / product]

### Where you are vs. where the work is happening

The frontier state for this domain right now is **[Run or Fly]**: [one sentence describing what that looks like, from the domain doc]. Most of your peers are at **[Walk]**, doing [behavior]. You're at **[their estimated stage]** based on what you described.

### The case study most like you

[Brand name from the domain doc] — [the named result, with number]. Why this fits: [1-2 sentences linking their context to the case].

[Ignore this section if no case study cleanly maps. Don't fabricate.]

### The named tools that fit your stack

| Tool | Why for you | Cost shape |
|---|---|---|
| [tool from resource-library] | [reason tied to their context] | [from resource-library] |
| ... | ... | ... |

[Only list tools from resource-library.md. If a category has no good match, say "no vetted tool fits this slot — flagged for v4".]

### The next move

**Do this:** [the canonical Walk → Run move from the domain doc, made concrete to their product].

**The pitfall to avoid:** [the canonical pitfall from the domain doc, plus a sentence on how it'd manifest specifically for them].

**The metric you'll know it worked:** [from the domain doc].

### What this unlocks

If this move lands, the next domain to attack is **[adjacent domain]** because [reason].

### Source

*Domain content from the Agentic Marketing Operating System v3 by Mahmoud Halat. Full framework: https://mahmoudhalat.com/marketing-os*
```

## Don't

- **Don't generalize beyond what the domain doc supports.** If their context is unusual (e.g., heavily regulated industry the case studies don't cover), say so explicitly: "the framework doesn't have a regulated-industry analogue here — frontier territory."
- **Don't recommend tools outside [`resource-library.md`](../resource-library.md).** If they ask about a popular tool not in the library, you can mention it but flag it as un-vetted.
- **Don't skip the pitfall.** Every domain has a canonical failure mode. Most users are about to make it.
- **Don't fabricate case studies.** Only cite the brands and numbers actually present in the domain doc. If there's no clean analogue, say so.
