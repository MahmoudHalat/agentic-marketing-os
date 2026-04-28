# PART IV. THE SIX AGENT ARCHETYPES (DEEP)

Build agents around archetypes; deploy them across domains. The reusability is the point.

**Reference implementations to study before building (all v3 additions):**
- [`anthropics/skills`](https://github.com/anthropics/skills), canonical SKILL.md examples (file-based skills system)
- [`langchain-ai/deepagents/examples/content-builder-agent`](https://github.com/langchain-ai/deepagents/tree/main/examples/content-builder-agent), 21.8K-star reference for Content Generator + Knowledge + Governance chain (the brand-governance-agent in LangGraph form)
- [`crewAIInc/crewAI-examples`](https://github.com/crewAIInc/crewAI-examples). Content Creator Flow, Senior Article Editor agent (role-based crews)
- [Anthropic's "Building Effective Agents" engineering essay](https://www.anthropic.com/engineering/building-effective-agents), six patterns (prompt chaining, routing, parallelization, orchestrator-workers, evaluator-optimizer, autonomous agents) that map to archetype combinations

## 1: Content Generator

**What it does:** Produces text, image, video, or code outputs against a defined spec.

**Across the domains:**
- Domain 3: blog posts, social posts, ad copy, email drafts
- Domain 4: campaign creative variants, headlines, CTAs
- Domain 6: outbound email drafts, follow-up sequences
- Domain 5: AEO-optimized definitional paragraphs

**Key design choices:**
- Multi-model routing (Claude for technical, GPT for general, Gemini for multimodal)
- Brand Governance Agent in the loop (always)
- Output schema enforcement (so downstream consumers can parse)
- Iterative refinement (draft → critique → refine; the Reflexion pattern)

**Common sub-types:**
- Short-form text generator (headlines, social posts, ad copy)
- Long-form text generator (blog posts, whitepapers, scripts)
- Image generator (social cards, illustrations)
- Video generator (shorts, ad creative)
- Code generator (landing pages, custom widgets)

## 2: Knowledge

**What it does:** Retrieves, synthesizes, and cites from internal and external knowledge sources. Includes RAG (retrieval-augmented generation) over your knowledge base.

**Across the domains:**
- Domain 1: synthesizing competitive intelligence from multiple sources
- Domain 2: pulling positioning research and customer interview transcripts
- Domain 3: research-first content workflows
- Domain 6: account research before outreach
- Domain 7: building synthetic personas from first-party data

**Key design choices:**
- Index design (vector DB choice: Pinecone, Weaviate, Qdrant, pgvector)
- Retrieval strategy (semantic vs. hybrid vs. graph)
- Citation requirements (every claim should be traceable)
- Freshness vs. depth tradeoffs
- Knowledge graph integration (for relationships between entities)

**Common sub-types:**
- Internal knowledge synthesizer (Confluence, Notion, Slack archives)
- Web research agent
- Account research agent (Clay-style)
- Customer voice synthesizer (interview transcripts, support tickets)
- Competitive intelligence agent

## 3: Localization

**What it does:** Adapts existing content across languages, regions, segments, regulatory contexts.

**Across the domains:**
- Domain 3: translating long-form content for non-English markets
- Domain 4: regional ad creative adaptation
- Domain 5: AEO/GEO for non-English LLMs (Yandex, Baidu, regional)
- Domain 6: regional outbound voice/tone shifts
- Domain 8: regional benchmarks for measurement

**Key design choices:**
- Translation vs. transcreation (translation preserves meaning; transcreation preserves intent)
- Cultural validation (in-region human review for high-stakes content)
- Compliance overlay (GDPR, CCPA, regional data rules)
- Vocabulary localization (terms that work in US ≠ UK ≠ Australia)

**Common sub-types:**
- Pure translation agent
- Transcreation agent (cultural adaptation)
- Regulatory compliance adapter
- Persona-segment adapter (enterprise vs. SMB voice)

## 4: Analyzer

**What it does:** Examines data and produces insight. The "what's going on?" agent.

**Across the domains:**
- Domain 1: anomaly detection in account behavior
- Domain 4: ad creative performance analysis
- Domain 6: deal slip prediction, pipeline health scoring
- Domain 8: attribution analysis, MMM interpretation, incrementality test design and analysis

**Key design choices:**
- Statistical rigor (significance testing, confidence intervals)
- Causal vs. correlational framing (don't claim causation without testing)
- Anomaly threshold tuning (too sensitive = noise; too loose = missed signals)
- Insight vs. recommendation distinction (analysis informs decisions; doesn't make them)

**Common sub-types:**
- Performance analyzer (campaign / channel / creative)
- Anomaly detection agent
- Forecast agent (pipeline, revenue)
- Attribution interpretation agent
- Cohort analyzer

## 5: Planner

**What it does:** Decomposes a goal into a sequence of actions. The "what should we do?" agent.

**Across the domains:**
- Domain 4: campaign planning, channel mix decisions
- Domain 6: ABM play orchestration, account-level engagement plans
- Domain 8: experiment design, test prioritization

**Key design choices:**
- Decomposition depth (when does the plan stop being useful?)
- Constraint awareness (budget, timeline, brand boundaries)
- Re-planning frequency (when do you re-plan vs. execute?)
- Human approval gates (which decisions need human sign-off?)

**Common sub-types:**
- Campaign planner
- Account-level engagement planner (ABM)
- Experiment designer
- Content calendar planner
- Budget allocation planner

## 6: Operator

**What it does:** Executes the plan. Calls APIs, ships content, books meetings, adjusts spend, sends messages.

**Across the domains:**
- Domain 3: publishing content to CMS / social platforms
- Domain 4: launching campaigns, adjusting bids and budgets
- Domain 6: sending outbound emails, booking meetings, updating CRM
- Domain 8: pausing underperforming campaigns

**Key design choices:**
- Tool permissions (read vs. write; small actions vs. high-stakes)
- Rate limiting and quotas
- Failure handling and retry logic
- Audit logging (every action traced)
- Reversibility (can this action be undone?)

**Common sub-types:**
- Content publisher
- Ad campaign operator (bid management, budget shifts)
- Outbound sequence operator (sends, replies, follow-ups)
- CRM update agent
- Calendar/meeting operator

## Anti-Patterns (when an archetype is the wrong choice)

- **Don't use a Content Generator for strategic positioning.** Generators output against a spec, they don't decide what the spec should be. Strategy decisions are Domain 2 / human work.
- **Don't use a Knowledge agent without provenance.** A RAG pipeline that returns claims without source attribution is a hallucination factory waiting to fire (cf. Lily Ray's "AI Slop Loop" feedback loop in Domain 5).
- **Don't use a Localization agent for high-stakes regulated content** without in-region human review, translation preserves meaning, transcreation preserves intent, but neither catches regulatory risk.
- **Don't use an Analyzer to make causal claims** without proper experimental design. Analyzers can spot correlations; causal claims require the Domain 8 incrementality framework.
- **Don't use a Planner without explicit constraints.** Open-ended planning produces over-confident multi-step proposals that fail expensively. Always pin budget, timeline, brand boundaries, and approval gates.
- **Don't give an Operator destructive tool access without hardcoded prohibitions.** The Replit incident (Domain 0 case studies) is the canonical case study for this failure mode, observability records failures *after*; enforcement prevents them *before*.

## How to Combine Archetypes

A typical agentic marketing workflow chains 3-5 archetypes:

### Chain 1: Account research → personalized outreach (Domain 6 + Domain 1)

*"Find an account that's in market, research it, write personalized outreach, send it, follow up."*

1. **Analyzer** monitors signal feeds (Domain 1) and identifies an in-market account
2. **Knowledge** agent does deep research on the account (recent news, leadership, tech stack)
3. **Planner** designs the multi-thread engagement strategy (which contacts, what messages, what cadence)
4. **Content Generator** drafts the personalized messages
5. **Brand Governance Agent** (a Knowledge + Analyzer hybrid) reviews drafts
6. **Operator** sends the messages and schedules follow-ups
7. **Analyzer** monitors response and triggers re-engagement or human escalation

**Reference implementation:** Anthropic + Clay (Domain 1 case study). Analyzer + Knowledge layer compresses 60-min research → <5 min per prospect.

### Chain 2: Content production pipeline (Domain 3 + Domain 5)

*"Take a topic, write a blog post that earns AI citations, ship it, measure citation lift."*

1. **Knowledge** agent (researcher). Perplexity API + Profound to surface what AI platforms currently cite for the target prompt; identify citation gaps
2. **Analyzer**, score competitor content on AEO criteria (answer-block placement, citation density, schema markup); produce a gap report
3. **Planner** (outliner), generate the AEO-first content brief (40-60 word answer block, question-led H2s, named-org statistics)
4. **Content Generator** (writer). Sonnet 4.5 long-form draft against the brief
5. **Content Generator** (editor). Opus 4.7 1M context for high-stakes piece review
6. **Brand Governance Agent** (8-agent parallel), voice / grammar / banned terms / legal / persona / sentence structure / terminology / factual grounding; threshold ≥95 = auto-publish
7. **Operator**, publish to CMS via API
8. **Analyzer**, track citation rate weekly via Profound; feed back to (1) for next round

**Reference implementation:** [`langchain-ai/deepagents/examples/content-builder-agent`](https://github.com/langchain-ai/deepagents/tree/main/examples/content-builder-agent) (21.8K stars). The CITABLE-framework B2B SaaS case study (Domain 3), citation rate 8% → 24% in 90 days, uses this exact chain shape.

### Chain 3: Measurement loop (Domain 8 + Domain 4)

*"Run an incrementality test, decide budget, deploy, measure, iterate."*

1. **Planner** (experiment designer), define hypothesis, select treatment + control geos, calculate required sample size, set duration
2. **Operator** (campaign launcher), deploy via Meta/Google Ads API; suppress treatment in control geos
3. **Knowledge** (data sync), pull spend, exposure, conversions from ad platforms + CRM into the warehouse
4. **Analyzer** (causal interpreter), run synthetic-control or geo-test analysis; produce incremental ROAS per channel
5. **Planner** (budget reallocator), feed incrementality output as Bayesian priors into MMM (Recast / Lifesight / Robyn); recommend budget reallocation
6. **Operator** (budget adjuster), push new budget allocations to ad platforms
7. **Analyzer** (anomaly watcher), alert on CAC drift > tolerance; loop back to (1) when next channel needs validation

**Reference implementation:** Soft Surroundings (Domain 8 case), cut retargeting 52% based on incrementality test → +17% revenue MoM, +12% YoY. PODS (Recast), moved from 2x/year MMM to weekly updates → +181% Google Non-Brand spend after go-dark test.

### Chain 4: Brand governance (Domain 0 + Domain 2 + Domain 3)

*"Every public-facing AI output gets reviewed before publish."*

This chain runs as a service consumed by Chains 1, 2, and others, not a standalone workflow.

1. **Orchestrator** (a thin Knowledge agent), receives draft + metadata (target persona, channel, brand spec version)
2. **8 specialized Analyzer agents in parallel**, each with a single audit dimension and its own context window:
   - Voice auditor (matches brand voice axes)
   - Grammar auditor
   - Banned-terms auditor (against the ontological don't-list)
   - Legal-claims auditor (against approved-claims registry)
   - Persona-fit auditor (target persona consumption test)
   - Sentence-structure auditor (banned patterns: "In today's fast-paced world...")
   - Terminology auditor (terms-we-own enforcement)
   - Factual-grounding auditor (citation verification)
3. **Aggregator** (Analyzer), produces single Brand Governance Score 0-100
4. **Decision gate** (Operator), score ≥95 auto-publish; 85-94 human review queue; <85 block + return to source agent for rework
5. **Audit logger** (Operator), every decision logged with `{brief, draft, governance_score, flagged_violations, approver, brand_spec_version}` for AgentOps observability + regulatory audit trail

**Reference implementation:** Brand.ai (Lyft, Opendoor), enterprise brand-compliance costs $5M/yr → small fraction; one copywriter manages 600 pieces of content (Domain 2 case). The Animalz "Claude Code style-guide" pattern published in 2025 + [anthropics/skills `brand-guidelines` repo](https://github.com/anthropics/skills/tree/main/skills/brand-guidelines).

### What every chain shares

- **Knowledge agents inject context** at the start of the chain
- **Analyzer agents validate quality** at multiple checkpoints, never just at the end
- **Planner agents produce explicit, constrained plans**, not open-ended "figure it out"
- **Brand Governance Agent gates every public-facing output** (Chains 1 + 2 cite to Chain 4 as a sub-routine)
- **Operator agents are sandboxed**: they can only call tools that have been pre-approved, with hardcoded prohibitions on destructive actions (the Replit lesson)
- **Audit logs are immutable** and feed AgentOps observability for drift detection (Domain 0)

Each archetype is reusable across these chains. Build once, deploy many.

---

## Future Expansion (v4 target)

This file is the v3 baseline (current). See [research-plan.md](research-plan.md) for methodology and master plan. Per-file checklist:

- [ ] **Primary sources to mine**, highest-signal reports, papers, podcasts, expert posts to extract from (with URLs and dates).
- [ ] **Claims to validate / refresh**, statistics that need primary-source verification or are stale.
- [ ] **Case studies to add**, real deployments with named clients, numbers, before/after data.
- [ ] **Tactical playbooks to add**, build-this-yourself walkthroughs, prompts, configs, decision trees.
- [ ] **Tooling deep-dives**, head-to-head comparisons, pricing notes, integration gotchas, switching costs.
- [ ] **Open questions**, unresolved debates worth tracking.
- [ ] **Cross-references**, links to Mahmoud's other skills, related domain files, external knowledge bases.

