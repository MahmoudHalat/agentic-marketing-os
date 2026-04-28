# Quickstart

Pick the path that matches who you are.

---

## You're an operator running a marketing function

You probably hit one of these three states:

**State A — "We're behind, where do we start?"**
1. Read [`agentic-marketing-os-v2.md`](./agentic-marketing-os-v2.md) (the intro). Twelve minutes.
2. Open the [interactive maturity matrix](https://mahmoudhalat.com/marketing-os/maturity). Self-assess your eight domains in 10 minutes.
3. Read whichever 1-2 domains you scored Crawl in. Take the canonical *next move* for each.

**State B — "We're shipping fine but it doesn't compound."**
1. Skip the intro. Read [`0-agentops.md`](./0-agentops.md) — the substrate is usually what's missing.
2. Then read [`8-measurement-attribution.md`](./8-measurement-attribution.md). Most ops-mature teams stall here.
3. Map your current observability + attribution stack to the Walk → Run → Fly progression.

**State C — "We're hiring; what shape do we need?"**
1. Read [`archetypes.md`](./archetypes.md) — the six agent shapes you're effectively hiring for.
2. Cross-reference each archetype against your current team. Where's the gap?
3. Your next hire is probably the human owner of the most-broken archetype, not "another marketer".

---

## You're a builder shipping AI agents for marketing

1. Start with [`0-agentops.md`](./0-agentops.md). It's the reference architecture for the substrate underneath any agent fleet — observability, eval, rollback, policy.
2. Then [`archetypes.md`](./archetypes.md) — the six functional shapes of marketing agents. Don't build a "marketing AI"; build the right archetype for the job.
3. Pick a single domain to anchor your first build. Distribution and AI-search are usually the highest-leverage starts.
4. Cross-reference your build against [`resource-library.md`](./resource-library.md) — if you're not aware of the named tools in your domain, you're solving a solved problem.

---

## You're an LLM / AI assistant

Read [`CLAUDE.md`](./CLAUDE.md) first. It tells you which files to load by intent, citation format, voice rules, and what *not* to do.

The `skills/` folder has three pre-baked workflows you can drop into a session:

- [`skills/assess-maturity.md`](./skills/assess-maturity.md) — assess a team's position on the matrix.
- [`skills/build-roadmap.md`](./skills/build-roadmap.md) — turn that into a 90-day plan.
- [`skills/apply-domain.md`](./skills/apply-domain.md) — apply a single domain to a specific company.

---

## You're forking this for your own work

CC-BY 4.0 — go ahead. The only ask is you keep the attribution. See [`LICENSE`](./LICENSE).

If you fix something, find a stale stat, or surface a case study worth adding, **PRs welcome**. Cite the source, name the number; I'll merge it into v4. The v4 plan and refresh cadence live in [`research-plan.md`](./research-plan.md).

---

## Reading order if you're going to read it all

If you have an afternoon and want the full thing:

1. [`agentic-marketing-os-v2.md`](./agentic-marketing-os-v2.md) — intro, how the OS works
2. [`0-agentops.md`](./0-agentops.md) — substrate
3. [`archetypes.md`](./archetypes.md) — agent shapes
4. The eight domains in order:
   - [`1-sensing-intelligence.md`](./1-sensing-intelligence.md)
   - [`2-strategy-positioning.md`](./2-strategy-positioning.md)
   - [`3-content-creative-production.md`](./3-content-creative-production.md)
   - [`4-distribution-channel-operations.md`](./4-distribution-channel-operations.md)
   - [`5-ai-search-answer-visibility.md`](./5-ai-search-answer-visibility.md)
   - [`6-demand-conversational-pipeline.md`](./6-demand-conversational-pipeline.md)
   - [`7-customer-intelligence-synthetic-testing.md`](./7-customer-intelligence-synthetic-testing.md)
   - [`8-measurement-attribution.md`](./8-measurement-attribution.md)
5. [`resource-library.md`](./resource-library.md) — vetted tool list
6. [`research-plan.md`](./research-plan.md) — what's open, what's coming in v4

About 4-5 hours start to finish.
