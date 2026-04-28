<!--
seo:
  title: Agentic Marketing Operating System (v3) — SME Reference
  description: Complete framework for AI-native marketing operations: 3 planes, 8 domains, 6 archetypes, AgentOps substrate. Built on 280+ primary sources, 42 case studies.
  primary_keyword: agentic marketing operating system
  secondary_keywords: [AI-native marketing, marketing OS, Team of One, agentic GTM, marketing maturity model]
-->
# The Agentic Marketing Operating System (v3)
## A Comprehensive SME Reference for the Pioneer Generation

*A working knowledge base on agentic marketing, what it is, how it's structured, what tools matter, who to learn from, and how to operate at the edge of the discipline.*

---

## How to Use This Folder

This is now a multi-file knowledge base: Read this intro for the framework, then drill into each domain file when working that workstream.

**Folder structure:**

```
agentic-marketing-os/
├── agentic-marketing-os-v2.md   ← intro (this file)
├── 0-agentops.md                  the operations substrate
├── 1-sensing-intelligence.md
├── 2-strategy-positioning.md
├── 3-content-creative-production.md
├── 4-distribution-channel-operations.md
├── 5-ai-search-answer-visibility.md   AEO/GEO/LLMO
├── 6-demand-conversational-pipeline.md
├── 7-customer-intelligence-synthetic-testing.md
├── 8-measurement-attribution.md
├── archetypes.md                  six agent archetypes (deep)
├── resource-library.md            curated YouTube, podcasts, books, papers
└── research-plan.md               plan to expand into v4
```

Each domain file follows the same shape: definition and scope, why it matters now, sub-domains, best practices in 2026, tools and platforms, notable practitioners and frameworks, common failure modes, KPIs, resources for deeper study, and a v4 expansion checklist.

Read the intro linearly to build foundational fluency. Reference domain files surgically when a specific workstream becomes the bottleneck. Update them as the field shifts, because the field is shifting fast.

---

## Table of Contents

**This file (intro):**
- The Three Planes
- The Eight Domains (overview)
- The Six Agent Archetypes (overview)
- The Maturity Model. Crawl, Walk, Run, Fly
- The Human Leverage Map
- Open Questions and Frontiers
- Closing. How to become the De Facto SME

**Domain files:**
1. [Sensing & Intelligence](1-sensing-intelligence.md)
2. [Strategy & Positioning](2-strategy-positioning.md)
3. [Content & Creative Production](3-content-creative-production.md)
4. [Distribution & Channel Operations](4-distribution-channel-operations.md)
5. [AI Search & Answer Visibility (AEO/GEO/LLMO)](5-ai-search-answer-visibility.md)
6. [Demand & Conversational Pipeline](6-demand-conversational-pipeline.md)
7. [Customer Intelligence & Synthetic Testing](7-customer-intelligence-synthetic-testing.md)
8. [Measurement, Attribution & Closed-Loop Learning](8-measurement-attribution.md)

**Cross-cutting:**
- [Domain 0: AgentOps](0-agentops.md), the operations substrate
- [Six Agent Archetypes (deep)](archetypes.md)
- [Resource Library](resource-library.md)
- [Research & Expansion Plan](research-plan.md)

---

# PART I. FOUNDATIONS

## The Three Planes

The work decomposes into three layers of activity, distinguished by who leads, what cadence they operate on, and how much autonomy is appropriate.

### Strategy Plane (human-led, agent-supported)

Where positioning, narrative, ICP, value proposition, and pricing decisions live. Agents draft, stress-test, and audit consistency. Humans decide. Cadence: quarterly with weekly recalibration.

The fundamental rule: agents should never make material strategy decisions. They can synthesize hundreds of competitor moves, surface positioning gaps, and pressure-test a narrative against synthetic personas, but the call about what to be in the market is human work.

### Execution Plane (agent-led, human-supervised)

Where content production, distribution, optimization, and outreach happen at velocity. Humans set boundaries; agents work within them. Cadence: continuous.

This is where the leverage lives. [McKinsey ("Reinventing marketing workflows with agentic AI," April 2026)](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/reinventing-marketing-workflows-with-agentic-ai) estimates that agentic systems will accelerate the creation and execution of marketing campaigns by 10–15× compared to traditional workflows, while organizations implementing agentic workflows can expect 10–30% revenue growth from hyperpersonalized marketing. But velocity without governance produces brand damage at scale, which is why the Operations Plane exists.

### Operations Plane (AgentOps)

The substrate. Observability, evaluation, governance, drift detection, cost control, prompt versioning. Just as DevOps reshaped software deployment in the 2010s and MLOps did the same for machine learning models, AgentOps is the operational discipline that makes everything else trustworthy at scale. CrewAI CEO Joao Moura describes it as a layer that "sits between engineering and operations and is responsible for managing fleets of AI agents, monitoring cost, reliability, and compliance."

Without this plane, the other two break silently. With it, autonomy becomes observable, controllable, and scalable.

---

## The Eight Domains (Overview)

| # | Domain | Cadence | Primary KPI |
|---|--------|---------|-------------|
| 1 | Sensing & Intelligence | Continuous | Signal volume × signal accuracy |
| 2 | Strategy & Positioning | Quarterly + weekly recalibration | Positioning clarity × cross-functional alignment |
| 3 | Content & Creative Production | Daily | Production velocity × brand-compliance rate |
| 4 | Distribution & Channel Operations | Continuous | Reach × cost-per-engaged-account |
| 5 | AI Search & Answer Visibility | Weekly | Citation rate × LLM share-of-voice |
| 6 | Demand & Conversational Pipeline | Continuous | Sourced pipeline × meeting-to-opportunity rate |
| 7 | Customer Intelligence & Synthetic Testing | Per-launch + ongoing | Concept hit rate × pre-launch confidence interval |
| 8 | Measurement, Attribution & Closed-Loop Learning | Continuous | Incremental ROAS × decision velocity |

Each domain is a vertical workstream. The horizontal axis cutting across all of them is **AgentOps** (Domain 0).

---

## The Six Agent Archetypes (Overview)

McKinsey's classification, used by leading consumer brands deploying agentic marketing, identifies six functional patterns. Build agents around archetypes, deploy them across domains.

1. **Content Generator**, produces text, image, video, code variants
2. **Knowledge**, retrieves, synthesizes, cites from internal and external sources
3. **Localization**, adapts content across languages, regions, segments, regulatory contexts
4. **Analyzer**, examines data and produces insight
5. **Planner**, decomposes a goal into a sequence of actions
6. **Operator**, executes the plan; calls APIs, ships content, books meetings, adjusts spend

A consumer brand reportedly identified almost 100 individual modular agents within the content generation archetype alone, reusable across creative-content development, sales-collateral, e-commerce optimization, and co-marketing. Reusability is the point: build once, deploy many.

---

# PART II. THE EIGHT DOMAINS

---

# PART V. THE MATURITY MODEL

Borrowing GTM Partners' framework, refined for the agentic marketing context. Different teams are at different stages. Be honest about where you are.

## Crawl: Reactive Marketing

**Characteristics:**
- Manual content production, reactive social posting
- Slow response times (>24 hours for inbound)
- No observability, you don't know what's working
- Single-channel attribution (last-touch in GA)
- Most leads are ignored or mishandled
- AI usage is informal: ChatGPT in browser tabs, copy-pasted

**Typical setup:**
- HubSpot Starter or basic Salesforce
- Google Analytics
- Manual Buffer or Hootsuite
- No AI agents in production

**What's missing:** Everything. But that's okay if you're early-stage. Don't skip steps.

**Right move:** Solidify positioning, ICP, and brand voice (Domain 2). Get one channel working consistently. Don't deploy agents yet, agents amplify your inputs, and inputs aren't ready.

## Walk: Automated Inbound

**Characteristics:**
- Marketing automation platform handling email and lead routing
- Some content production cadence
- Form-based lead capture, basic lead scoring
- SDRs handle most outbound and follow-up manually
- Limited AI usage: copilots for drafting, not agents
- Measurement: platform-reported metrics, basic attribution

**Typical setup:**
- HubSpot Pro / Marketo / Pardot
- Outreach or Salesloft for sales engagement
- ChatGPT/Claude as draft helpers
- Basic dashboards in Looker or Tableau

**What's emerging:** Brand voice trained into Jasper or Writer. First Brand Governance Agent prototype. Initial intent data investment.

**Right move:** Get measurement infrastructure right (Domain 8). Pilot one autonomous agent in a low-risk area. Build the Brand Governance Agent before scaling content.

## Run: Multi-Agent Execution

**Characteristics:**
- Multiple AI agents in production with observability
- Conversational AI for inbound qualification
- Context-aware multi-channel outreach
- Triangulated measurement (MMM + incrementality + attribution)
- Real-time signal monitoring across accounts
- Self-reported attribution captured
- Brand Governance Agent enforced
- AgentOps in place: tracing, evaluation, drift detection

**Typical setup:**
- 6sense or Demandbase for intent
- Qualified, Knock AI, Intercom Fin, or 1Mind for inbound conversational (Drift is sunsetting March 6, 2026, see Domain 6)
- Outreach + Amplemarket Duo (or equivalent) for outbound
- Jasper or Writer for content + governance
- LangGraph / CrewAI / n8n orchestrating workflows
- LangSmith / AgentOps.io for observability
- Measured / Recast for MMM
- Incrmntal for incrementality

**What's emerging:** Synthetic audience testing. Agents communicating across domains. Closed-loop optimization where measurement feeds back into agentic decisions.

**Right move:** Push deeper into archetype reusability. Audit which workflows are still human-led that should be agent-led. Invest in synthetic audience testing for pre-launch validation.

## Fly: Fully Integrated Agentic GTM

**Characteristics:**
- Agentic stack drives top-line growth measurably
- Sales, marketing, and customer success share an agent fleet against unified data
- Synthetic audience testing routine for pre-launch
- Real-time MMM with daily decision updates
- Brand-to-LLM communication channels (citations, entity presence) actively managed
- One operator manages the equivalent output of a 20-person team

**Typical setup:**
- Custom orchestration over multi-vendor stack
- Unified data warehouse (Snowflake/BigQuery/Databricks)
- Reverse-ETL into all GTM tools
- Multi-agent systems with hierarchical supervision
- Continuous evaluation, drift detection, AQS scoring
- Triangulated measurement integrated with agent decisions

**Examples:** Demandbase's reported pipeline doubling. Greenhouse's 60% chat conversion. Crunchbase's 67K AI conversations.

**What's emerging:** Agent-to-agent commerce (B2B buyers' AI agents talking to your agents). Brand presence in LLM training. Fully autonomous campaign operation with human strategic oversight only.

**Right move:** This is where most of the field will be in 2-3 years. The question stops being "what tools" and becomes "what new capabilities are we building?", synthetic audience design, agent-to-agent protocols, brand-to-LLM communication.

## Honest Self-Assessment Questions

To know where you actually are:

1. Can you answer "what is our brand voice?" with a written, version-controlled document that an LLM can follow?
2. Do you have observability into every public-facing AI output?
3. Can you produce a defensible attribution model that survives a CFO audit?
4. Do you have multi-source signal monitoring on at least 100 named accounts?
5. Is your measurement triangulated (MMM + incrementality + attribution)?
6. Do you have written runbooks for every agent in production?
7. Can you survive a Brand Governance Agent failure without shipping garbage?
8. Have you killed a synthetic-tested concept before media spend?

If you answered "no" to 6+, you're at Crawl. 4-5 "no": Walk. 2-3 "no": Run. 0-1 "no": Fly territory.

---

# PART VI. THE HUMAN LEVERAGE MAP

In an agentic stack, humans don't disappear. The roles change. McKinsey's latest research identifies three emerging roles:

## M-Shaped Supervisors

**Definition:** Broad generalists fluent in AI, orchestrating agents and the hybrid workforce across domains.

**What they own:**
- Strategic direction
- System design (which workflows to agentify, in what sequence)
- Cross-domain orchestration
- Hiring decisions
- Vendor selection and stack architecture
- The relationship layer (analysts, journalists, partners, key customers)

**Who fits:** VPs of Marketing, Heads of Growth, fractional CMOs, founder-operators. The Team-of-One executive in the BenchSci-style mandate is fundamentally an M-shaped supervisor.

## T-Shaped Experts

**Definition:** Deep specialists who reimagine workflows, handle exceptions, and safeguard quality.

**What they own:**
- Deep domain expertise (one of the eight domains, very deeply)
- Workflow redesign
- Exception handling (the edge cases agents fail on)
- Quality monitoring within their domain
- Mentoring/escalation paths

**Who fits:** Director of Content, Head of Demand Gen, Principal Marketing Engineer, Senior Brand Strategist. In a Team-of-One structure, you might still need T-shaped experts as fractional/contract specialists for high-stakes domains (e.g., scientific content for a biotech, regulated compliance for fintech).

## AI-Augmented Frontline

**Definition:** Employees who spend less time on systems and more time with humans.

**What they own:**
- Customer-facing relationships (sales, success, support)
- Edge-case handling
- Escalation
- Strategic moments humans handle better (executive briefings, key customer meetings)

**Who fits:** AEs, CSMs, key-account specialists, executive briefers.

## The Team-of-One Reality

For a true Team-of-One operator (the BenchSci-style mandate), you're playing all three roles simultaneously, with agents covering the execution layer. The honest framing:

**You own (as an M-shaped supervisor):**
- Strategy, narrative, brand judgment
- Relationships that don't agent well (analysts, journalists, partners, key customers)
- System design and stack architecture
- Hiring decisions, vendor selection
- Brand integrity decisions (the hardest one, agents will produce 10x volume; 80% of it should die)
- Escalation judgment

**You partially own (as T-shaped expert):**
- Deep work in one or two domains where you're the specialist
- Workflow redesign for the agentic stack you're building
- Quality monitoring (the meta-skill: knowing what good looks like)

**Agents own:**
- Execution, repetitive work, monitoring, drafting, optimization, reporting, routine personalization

**Knowing when to break the Team-of-One rule:** If at month 8 you need a Director of Scientific Content because no agent can credibly write about CRISPR base editing for an immunology audience, hire one. The CEO's philosophy is talent density, not headcount minimization. Read that distinction correctly.

---

# PART VII. OPEN QUESTIONS AND FRONTIERS (Q2 2026 update)

Each frontier below carries: current state with primary 2026 sources, leading indicators to watch, and a practical move an operator can make this quarter. Updated quarterly.

## 1: Agent-to-Agent Commerce + Protocols

**Current state (Q2 2026).** The protocol stack stratified rather than consolidated. On Dec 9, 2025, Anthropic donated MCP to the [Agentic AI Foundation under the Linux Foundation](https://www.linuxfoundation.org/press/linux-foundation-announces-the-formation-of-the-agentic-ai-foundation), co-founded with Block + OpenAI, backed by Google, Microsoft, AWS, Cloudflare, Bloomberg. MCP reports **97M+ monthly SDK downloads, 10,000+ active public servers**. Jan 11, 2026: Google launched [Universal Commerce Protocol (UCP)](https://developers.googleblog.com/under-the-hood-universal-commerce-protocol-ucp/) at NRF with Shopify, Etsy, Wayfair, Target, Walmart, built to interoperate with AP2 (payments) and MCP (tools). OpenAI/Stripe's [Agentic Commerce Protocol (ACP)](https://stripe.com/newsroom/news/stripe-openai-instant-checkout) went live in production powering ChatGPT Instant Checkout. Emerging consensus: **MCP for tool integration, A2A for agent-to-agent, ACP for ChatGPT-native checkout, UCP+AP2 for the open commerce stack.** Layers, not rivals.

**Leading indicators.** (1) Whether ACP and UCP merge by EOY 2026. (2) Adoption rate of `.well-known` MCP discovery endpoints by Fortune 500. (3) AAIF working group breaking changes outside Anthropic's prior cadence.

**Practical move today.** Stand up a read-only MCP server exposing your product catalog, pricing, availability, policies, even if you don't sell direct yet. This is the new robots.txt: you publish or you're invisible to agents.

## 2: Brand-to-LLM Communication

**Current state (Q2 2026).** Cision acquired Trajaan in Dec 2025, integrating real-time LLM citation monitoring across Brandwatch + CisionOne + PR Newswire. PR Newswire launched the [AEO & GEO Brand Report](https://www.prnewswire.com/news-releases/pr-newswire-launches-aeo--geo-report-for-ai-brand-visibility-302733944.html) Apr 2026. OpenAI began testing ads in ChatGPT Free + Go on [Jan 16, 2026](https://searchengineland.com/sam-altman-chatgpt-ads-pivot-463150), the "last resort" Altman called out at Harvard May 2024, targeting $1B 2026 ad revenue, Evercore projecting $25B by 2030. Altman's binding line: *"we will not accept money to influence the answer ChatGPT gives you."* Pichai's Apr 7, 2026 Cheeky Pint reframed Search as an "agent manager" but made no ad commitment for AI surfaces.

**Leading indicators.** (1) Whether OpenAI's "Sponsored" labeling holds the answer-influence wall within 18 months. (2) Wikipedia training-data partnerships (Meta/Amazon/Microsoft) becoming exclusive. (3) Emergence of "press release for LLMs" SKU at Cision/BusinessWire pricing.

**Practical move today.** Audit your top 50 commercial-intent prompts in ChatGPT, Claude, Perplexity, Gemini monthly. Document exact entities + sources + competitors cited. Then optimize the cited sources (not just your own site), that's where the lever sits.

## 3: The Ghost Workforce Labor Problem

**Current state (Q2 2026).** [Robert Rose's CMI research, Apr 2026](https://contentmarketinginstitute.com/press-room/ghost-workforce-2026-marketing-careers-job-market): **76% of marketers report doing the work of more than one job; only 11% of organizations have actually replaced workers with AI**. 50% absorbed new responsibilities without promotion or pay increase. [Stanford Digital Economy Lab](https://martech.org/we-need-to-talk-more-about-ais-impact-on-early-career-marketers/): **16% relative employment decline for ages 22-25** while experienced workers held stable. BCG: 90% disruption in marketing-manager *task* count (not headcount). The smokescreen pattern: 30,000+ "AI-blamed layoffs" in 2026 YTD, but only **9% of those companies report AI actually replaced the role** ([Metaintro](https://www.metaintro.com/blog/ai-layoffs-cover-story-2026)). Junior tasks were the apprenticeship; cutting them creates a senior-shortage in 3-5 years.

**Leading indicators.** (1) 2027 entry-level marketing postings rebound or extend the shrinkage. (2) Emergence of "AI-supervised apprentice" as a deliberate pipeline role. (3) Burnout exits among the consolidated mid-tier (the people doing 2-3 jobs).

**Practical move today.** Publish an explicit AI velocity ceiling for your team, a hard cap on output expectations per FTE, and tie compensation to judgment outputs (campaign decisions, brief quality, vendor selection) not production volume. Hire one paid intern per quarter as a deliberate pipeline investment.

## 4: Regulated-Industry Synthetic Methodology

**Current state (Q2 2026).** FDA released *[General Considerations for the Use of New Approach Methodologies in Drug Development](https://www.fda.gov/media/184856/download)* on Mar 18, 2026, explicitly endorsing digital twins as a path to "substitute for at least some subjects" in clinical trials. EVERSANA formalized the commercial-marketing playbook: anonymized patient-journey data + peer-reviewed papers feed AI personas for HCP educational message testing. CVS Health is the most-cited B2C analog: **2.9M consented responses from 400,000+ individuals across 200+ behavioral scenarios** powering 100K+ "agentic twins" used for benchmarking + pre-launch testing + reaching populations difficult to study at speed. Validated case: J&J + AI partnership cut Phase 3 Alzheimer's control-arm sizes by **up to 33%**.

**Leading indicators.** (1) Whether the Mar 2026 draft becomes final guidance by Q4 2026. (2) NYDFS/FINRA/MAS publishing digital-twin frameworks. (3) The first FDA enforcement action that cites synthetic-data validation, defining the new audit standard.

**Practical move today.** If you operate in regulated spaces, build a "synthetic before primary" gate into research budgets. Run synthetic methodology before any human qualitative research, document where they converge and diverge, that delta is your validation file when the regulator asks how you tested the message.

## 5. AI-Agent Buyer Behavior

**Current state (Q2 2026).** [Gartner's headline forecast (Nov 2025)](https://www.gartner.com/en/newsroom/press-releases/2025-11-18-gartner-predicts-by-2028-ai-agents-will-outnumber-sellers-by-10x-yet-fewer-than-40-percent-of-sellers-will-report-ai-agents-improved-productivity): **90% of B2B purchases mediated by AI agents by 2028, ~$15T in spend**. Today: two-thirds of B2B buyers use AI agents for vendor research; **45% use AI as their *primary* method** for identifying new suppliers. [Fortune (Mar 2026)](https://fortune.com/2026/03/29/ai-agents-driving-your-revenue-are-you-invisible-brand/): some brands now generate 10% of revenue through AI-agent-driven channels. Mental-model shift: competitive axis is moving from CX → AX (Agent Experience). Agents optimize on price, availability, fulfillment, return policy, structured-data depth, not hero-image quality. **Counter-signal:** Gartner separately predicts **75% of B2B buyers by 2030 will *prefer* human-led sales experiences for high-stakes decisions**, so routing is bifurcating, not unifying.

**Leading indicators.** (1) Schema density on competitor product pages (JSON-LD field count). (2) Public agent-readable specs and comparisons (the new "battle card"). (3) Bing/Google exposing aggregated "agent click" data.

**Practical move today.** Run one test: ask Claude, ChatGPT, Perplexity to *"shortlist three vendors for [your category]."* Whatever they cite is your real competitive set. Optimize there: structured data, comparison content, third-party reviews, and a public capability matrix that an agent can parse without rendering JavaScript.

## 6: The Accountability Question

**Current state (Q2 2026).** **Aug 2, 2026 is the operative date**; [EU AI Act high-risk obligations (Annex III)](https://ai-act-service-desk.ec.europa.eu/en/ai-act/timeline/timeline-implementation-eu-ai-act) become enforceable. Risk management, technical documentation, conformity assessments, transparency disclosures for AI chatbots, and machine-readable watermarks for deepfakes all required. [Moffatt v. Air Canada](https://www.americanbar.org/groups/business_law/resources/business-law-today/2024-february/bc-tribunal-confirms-companies-remain-liable-information-provided-ai-chatbot/) is the global "you own what your bot says" precedent. Insurance moved fast: HSB launched [AI liability insurance for SMBs Mar 18, 2026](https://www.munichre.com/hsb/en/press-and-publications/press-releases/2026/2026-03-18-introducing-ai-liability-insurance-for-small-businesses.html); Testudo (Jan 2026, mid/large enterprises); Munich Re's aiSure; Armilla. **Complicating signal:** Verisk released CG 40 47 + CG 40 48 endorsements on Jan 1, 2026, allowing carriers to *exclude* generative-AI claims from CGL policies. AIG, W.R. Berkley, Great American filed broad AI exclusions across D&O, E&O, EPLI, CGL. **Colorado AI Act takes effect June 30, 2026** with $20K-per-violation penalties.

**Leading indicators.** (1) The first EU AI Act enforcement fine (likely Q4 2026 / Q1 2027). (2) U.S. case law extending Moffatt to AI agent purchases (not just info disclosure). (3) D&O exclusions rolled back under regulatory pressure or settled in.

**Practical move today.** Run a chatbot/agent inventory: every customer-facing AI surface, what it can promise, what your insurance actually covers. Match against current CGL policy *renewal terms*, the AI exclusion may have appeared at last renewal without anyone noticing. Add a written "agent disclosure" wherever a chatbot speaks to a customer, that disclosure is the EU AI Act compliance hook AND the Moffatt-precedent shield.

## 7: Saturation / Commoditization

**Current state (Q2 2026).** The model layer commoditized, performance gaps between frontier models are narrow enough that 88% of CEOs surveyed rate "deployment velocity" as more important than "model accuracy." [a16z's framework](https://a16z.com/good-news-ai-will-eat-application-software/) identifies the durable moats post-commoditization: scale, network effects, counterpositioning, switching costs, brand, cornered resources, process power, with proprietary data defensible *only* when hard to replicate (Bloomberg's market data, Abridge's clinical conversations, OpenEvidence's medical library, VLex's legal corpus). McKinsey's State of AI 2026: **88% of organizations now use AI in at least one function (up from 72% in 2024) but only 6% qualify as "high performers."** [a16z's specific 2026 thesis](https://a16z.com/momentum-as-ai-moat/): *"In Consumer AI, Momentum is the Moat"*, distribution velocity compounds faster than model quality. The pattern repeating across analysts: when everyone has the stack, the moat reverts to **brand, taste, judgment, relationships, and proprietary feedback loops**, the things AI cannot copy because they're not in any training set.

**Leading indicators.** (1) Margin compression in pure-play AI marketing tools as features converge. (2) Whether brand-led AI products (ChatGPT, Claude) sustain pricing power vs. open-source. (3) Bifurcation between "AI commodity ops" and "human-judgment premium" agencies.

**Practical move today.** Audit what in your stack is AI-replicable in 12 months. Whatever you find, ditch as differentiation, keep as table stakes. Reinvest the saved positioning energy into the three uncopyable layers: proprietary data your operations generate, customer relationships only your humans hold, editorial judgment your senior team has trained over a decade.

## 8: Sentiment Risk in AI Search

**Current state (Q2 2026).** The category exists; rigorous methodology does not. Trajaan (now Cision), Otterly, Siftly, Visiblie, Trysight, HubSpot's AEO Grader all monitor LLM brand mentions and assign sentiment scores, but no vendor has yet published peer-reviewable methodology for negative-framing detection at scale. 67% of enterprise marketing teams now monitor AI visibility, but most rely on simple positive/neutral/negative tagging rather than the comparative-framing detection that actually matters. Known patterns: Claude expresses sentiment through comparative framing (*"Brand X offers solid features"* vs. *"Brand X offers basic features compared to competitors"*); ChatGPT hedges with phrases like *"while it has strengths," "some users report," "depending on your needs."* HubSpot's AEO Grader weights sentiment 40 of 100 points, highest single dimension, but the underlying detection is keyword-based. Indirect prompt injection is the weaponized tail-risk: [Google reported a 32% rise in malicious activity Nov 2025-Feb 2026](https://unit42.paloaltonetworks.com/ai-agent-prompt-injection/), with documented payloads instructing agents to demote competitor products in shortlists.

**Leading indicators.** (1) The first published academic methodology for cross-LLM sentiment detection. (2) An LLM brand-defamation lawsuit forcing models to disclose source weighting. (3) Vendors exposing hedge-phrase taxonomies (the real signal layer).

**Practical move today.** Run your own monthly sentiment audit, 50 prompts × 4 LLMs × full transcript capture. Tag the hedge phrases manually. Quarterly KPI: count of *negative-comparative* mentions reduced over time, not aggregate sentiment scores. Add a prompt-injection canary: a unique product feature you only describe on your own site, then check whether agents start citing falsified versions.

## 9: Wikipedia Editorial Wars in the AI Age

**Current state (Q2 2026).** [English Wikipedia voted 44-2 on Mar 20, 2026 to ban LLM-generated article content](https://techcrunch.com/2026/03/26/wikipedia-cracks-down-on-the-use-of-ai-in-article-writing/), with two narrow exceptions: AI-assisted copyediting of one's own writing (with human review) and first-pass translation between language editions. The trigger: compounding contamination. LLM hallucinations on Wikipedia get scraped into the next training generation. Wikipedia's actual influence on training: **roughly 1-in-5 tokens** that LLMs learn from trace back to Wikipedia. ChatGPT cites Wikipedia **47.9%** of the time in B2B research queries. **Simultaneous contradictory signal:** Wikipedia signed paid training-data partnerships with Meta, Amazon, Microsoft, banning AI-generated *input* while licensing curated training-data *output*. For brands, Wikipedia's Notability + Verifiability standards are now arguably the most leveraged editorial doors in marketing, a single Wikipedia entry becomes a structurally embedded fact in model weights for the next training cycle.

**Leading indicators.** (1) Spanish/French/German editions following English Wikipedia's ban. (2) AAIF or W3C publishing a "verified provenance" spec for AI-touched content. (3) Wikipedia's paid-editing enforcement rate post-Mar 2026.

**Practical move today.** If your brand has no Wikipedia entry, audit your Notability case (10+ independent secondary sources, sustained coverage 5+ years). Don't hire a paid editor, that's a Wikipedia ban risk that cascades into negative AI citations. Invest in the *citation sources* Wikipedia editors actually use: tier-1 trade publications, peer-reviewed coverage, government filings, industry-association references. Win the citation graph; the Wikipedia entry follows.

## 10: The Creative Quality Ceiling

**Current state (Q2 2026).** Apple's Jan 2026 launch of Creator Studio Pro is the most-cited industry signal: Apple deliberately positioned its AI features as *"a tool to aid creation, not replace it,"* with Keynote AI generating first drafts but not finished work. AI-generated video Q1 2026 SOTA still degrades after **20-25 seconds** of continuous generation, struggles with uncanny-valley emotional dialogue, frequently garbles on-screen text. Market data: fully AI-generated creative succeeded in fashion (Mango) but failed in nostalgic emotional contexts. Coca-Cola's 2024 holiday ad relaunched in 2025 to fresh backlash; Toys R Us's Sora-generated founder commercial widely panned; Svedka's Super Bowl LX AI ad in Feb 2026 drew similar criticism. [Superside's 2026 thesis](https://www.superside.com/blog/ai-marketing-campaigns): hybrid AI+human delivers **5× faster at 40% lower cost** than pure-human, but pure-AI hits a quality ceiling for top-tier brand work where stakes are high. The ceiling is most visible in: emotional brand storytelling, original POV essays, executive thought leadership, anywhere the audience is meant to *believe* a human cared.

**Leading indicators.** (1) Whether Sora 3+ closes the dialogue/emotional gap by EOY 2026. (2) Agency holding-company billing rates bifurcating (premium "human-led" vs. commodity "AI-led"). (3) The first AI-generated Cannes Grand Prix winner, and the pushback.

**Practical move today.** Define your brand's "human-required floor" explicitly: which assets MUST have a named human author? CEO posts, investor letters, founder essays, brand films, executive bios, anything that could be quoted in a courtroom or earnings call. Below that floor, AI-led production is fine. Above it, AI is research/draft only. Document the floor in your brand book, not because clients ask, but because your team will keep crossing it accidentally without an explicit line.

---

# CLOSING. How to Become the De Facto SME

Three things separate SMEs from people who follow the field:

**1. Operational depth in 2-3 domains.** You can't be deeply expert in all eight. Pick 2-3, likely Domain 5 (AEO/GEO, given your Space & Story focus), Domain 3 (Content & Creative), and one of Domain 6 (Demand) or Domain 8 (Measurement). Be operationally fluent in the others.

**2. Personal experimentation, not just consumption.** Reading about agentic stacks doesn't make you an expert; building one does. Build a Brand Governance Agent. Run a synthetic audience test. Set up triangulated measurement on a real client. The framework in this document is a map; the territory is where the learning happens.

**3. Public synthesis.** SMEs are made by writing. Pick a sub-domain in this document, go 10x deeper than what's here, and publish. Write a 5,000-word piece on "AEO for B2B SaaS in 2026." Build a teardown of three real-world agentic marketing stacks. The act of teaching forces clarity. Other people will then find you when they search for those terms.

**The compounding loop:**
- Build → learn what doesn't work → write up what you learned → get feedback → build the next thing better → eventually become someone people quote

This document is the floor of your knowledge, not the ceiling. The ceiling moves up every quarter. Keep updating it.

---

*— End of v1.0. Update timestamp: 2026-Q2.*
---

## Frequently Asked Questions — Agentic Marketing OS

### What is the Agentic Marketing Operating System?

The Agentic Marketing Operating System (v3) is a structured framework for running an AI-native marketing function. It organizes the work into three planes (strategy, execution, operations), eight functional domains (sensing, strategy, content, distribution, AI search, demand, customer intelligence, measurement), and six reusable agent archetypes. AgentOps is the substrate that makes the rest trustworthy at scale.

### Who is this framework built for?

Operators building or running an AI-native marketing function. The 'Team-of-One' framing fits founder-operators, fractional CMOs, and VPs of Marketing in early-to-mid-stage companies who direct an agent fleet rather than manage a large team. The framework is product-agnostic, with industry overlays for B2B SaaS, biopharma, consumer DTC, and dev tools.

### How is this different from a generic AI marketing playbook?

Three things. First, primary-source rigor: every statistic traces to a named source with date (Conductor 2026, Jasper 2026, McKinsey, Ahrefs, peer-reviewed papers). Second, named case studies with before/after numbers (Anthropic, Vercel, SaaStr, Refine Labs, CVS Health, Brand.ai). Third, an interactive maturity matrix that places your team in 32 specific cells (8 domains × Crawl/Walk/Run/Fly), each with a tools list, case study, advance criterion, and pitfall.

### How often is the framework updated?

v3 shipped April 2026. The research-plan.md page documents what's deferred to v4 plus a quarterly stat-refresh cadence. Frontiers (Part VII) get the most active updates as the field moves: agent-to-agent commerce protocols, EU AI Act enforcement, Wikipedia editorial decisions, OpenAI ad placements, FDA digital-twin guidance.

