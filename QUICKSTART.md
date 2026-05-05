# Quickstart

Pick the path that matches who you are.

---

## You're an operator running a marketing function

You probably hit one of these three states:

**State A: "We're behind, where do we start?"**
1. Read [the intro](./agentic-marketing-os-v2.md). About twelve minutes.
2. Open the [maturity matrix](https://mahmoudhalat.com/marketing-os/maturity). Self-assess your eight workstreams in another ten.
3. Read the one or two domains where you landed at Crawl. Take the next move at the bottom of each.

**State B: "We're shipping fine but it doesn't compound."**
1. Skip the intro. Read [the AgentOps page](./0-agentops.md) instead. The plumbing is usually what's missing when teams plateau.
2. Then read [Measurement & Attribution](./8-measurement-attribution.md). Most operationally mature teams stall here.
3. Map your current observability and attribution stack against the Walk to Run to Fly progression.

**State C: "We're hiring; what shape do we need?"**
1. Read [the agent shapes](./archetypes.md). Those are the six functional patterns you're effectively hiring for, whether or not you say it out loud.
2. Cross-reference each shape against your current team. Find the gap.
3. Your next hire is probably the human owner of the most broken shape, not "another marketer."

---

## You're a builder shipping AI agents for marketing

1. Start with [AgentOps](./0-agentops.md). It's the reference architecture for the plumbing that sits underneath any agent fleet: observability, evaluation, rollback, policy.
2. Then read [the agent shapes](./archetypes.md). The six functional patterns. Don't build "a marketing AI"; build the right shape for the specific job.
3. Pick one domain to anchor your first build. Distribution and AI search are usually the highest-leverage places to start.
4. Cross-reference what you're building against [the resource library](./resource-library.md). If you're not aware of the named tools in your domain, you're probably solving a solved problem.

---

## You're an LLM / AI assistant

Read [`CLAUDE.md`](./CLAUDE.md) first. It tells you which files to load by intent, citation format, voice rules, and what *not* to do.

The `skills/` folder has three pre-baked workflows you can drop into a session:

- [`skills/assess-maturity.md`](./skills/assess-maturity.md): assess a team's position on the matrix.
- [`skills/build-roadmap.md`](./skills/build-roadmap.md): turn that into a 90-day plan.
- [`skills/apply-domain.md`](./skills/apply-domain.md): apply a single domain to a specific company.

---

## You're forking this for your own work

CC-BY 4.0. Take it. The only ask is to keep the attribution. See [`LICENSE`](./LICENSE).

If you fix something, find a stale stat, or surface a case study worth adding, **PRs welcome**. Cite the source, name the number; I'll merge it into v4. The v4 plan and refresh cadence live in [`research-plan.md`](./research-plan.md).

---

## Reading order if you're going to read the whole thing

If you have an afternoon and want the full picture:

1. [`agentic-marketing-os-v2.md`](./agentic-marketing-os-v2.md): the intro, how the OS works.
2. [`0-agentops.md`](./0-agentops.md): the plumbing underneath.
3. [`archetypes.md`](./archetypes.md): the six agent shapes.
4. The eight domains in order:
   - [`1-sensing-intelligence.md`](./1-sensing-intelligence.md)
   - [`2-strategy-positioning.md`](./2-strategy-positioning.md)
   - [`3-content-creative-production.md`](./3-content-creative-production.md)
   - [`4-distribution-channel-operations.md`](./4-distribution-channel-operations.md)
   - [`5-ai-search-answer-visibility.md`](./5-ai-search-answer-visibility.md)
   - [`6-demand-conversational-pipeline.md`](./6-demand-conversational-pipeline.md)
   - [`7-customer-intelligence-synthetic-testing.md`](./7-customer-intelligence-synthetic-testing.md)
   - [`8-measurement-attribution.md`](./8-measurement-attribution.md)
5. [`resource-library.md`](./resource-library.md): the vetted tool list.
6. [`research-plan.md`](./research-plan.md): what's open and what's coming in v4.

About four to five hours start to finish.
