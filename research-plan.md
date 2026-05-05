# Research & Expansion Plan

This page is two documents: (1) the **v3 changelog** documenting what shipped from the original plan, and (2) the **v4 forward plan** for the next iteration. Methodology applies to both.

---

# Part 1, v3 (shipped Apr 2026)

## Headline numbers

- **13 files**, ~4,200 lines of structured markdown
- **280+ cited URLs** with author and date
- **42 named case studies** with brand + numerical before/after
- **32-cell interactive maturity matrix** (8 domains × 4 stages: Crawl/Walk/Run/Fly)
- **5 Mermaid architecture diagrams** (Brand Governance Agent, multi-source signal feed, agentic content pipeline, hybrid AI+human outbound, triangulated measurement)
- **32 industry overlay tables** (4 industries × 8 domains: B2B SaaS, Biopharma, Consumer DTC, Dev tools)
- **22 verbatim practitioner quotes** with primary-source URLs
- **10 frontiers** with current-state Q2 2026 sourcing + leading indicators + practical move
- **Cross-link audit closed**: every domain passes 5+ inter-domain links and 2+ skill cross-references

## Cross-cutting validation [✓ all closed]

| ID | Status | What shipped |
|---|---|---|
| **V1** Citation stat reconciliation | ✓ Closed | [Ahrefs Mar 2026](https://ahrefs.com/blog/ai-overview-citations-top-10/) (38% AIO from top 10, n=863K SERPs) + [Ahrefs Aug 2025](https://ahrefs.com/blog/ai-search-overlap/) (~80% non-Google LLMs from outside top 100, n=15K queries). Mahmoud's `aeo-geo-playbook.md` 70% figure replaced. Methodology footnote added. |
| **V2** McKinsey forecasts | ✓ Closed | Each forecast dated and linked: 10-15× velocity ([Apr 2026](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/reinventing-marketing-workflows-with-agentic-ai)); $750B US AI search ([Nov 2025](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/new-front-door-to-the-internet-winning-in-the-age-of-ai-search)); $3T-$5T agentic commerce range ([Oct 2025](https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-agentic-commerce-opportunity-how-ai-agents-are-ushering-in-a-new-era-for-consumers-and-merchants)). The "$7.6B/$47.1B/45.8% CAGR" reattributed to MarketsandMarkets (not McKinsey) with note that exact combination doesn't appear in a single release. |
| **V3** Qualified case studies | ✓ Closed | Demandbase verified (2× pipeline, $80K savings). **Greenhouse corrected to 50%/91% (not 60%/130%)**, original v2 figures don't match current case study. Crunchbase verified (67K conversations, 3× meetings, 2× MQLs). |
| **V4** AI SDR collapse data | ✓ Closed | 11x.ai sourced to [TechCrunch Mar 2025](https://techcrunch.com/2025/03/24/a16z-and-benchmark-backed-11x-has-been-claiming-customers-it-doesnt-have/) + [Sifted](https://sifted.eu/articles/11x-toxic-culture-ceo-working-nights-a16z) (≥70% customers closed/paused). **Artisan corrected to 3.9/5 on G2** (not 3.5/5; 22 verified reviews, polarized 72% 5★ / 13% 1★). **"Only 2% survive past first year" flagged as unverifiable**, closest verified line is Lemkin/SaaStr's "90% produce zero pipeline" (paraphrase). 50-70% UserGems churn estimate retained as industry-cited but flagged as not having published primary methodology. |
| **V5** Vendor M&A | ✓ Closed | **Drift sunset Mar 6, 2026** flagged across all files; 1Mind named exclusive successor. Bizible → Adobe Marketo Measure (rebranded Mar 2022). Clearbit → HubSpot Breeze Intelligence (Nov 2023 acquisition + Inbound 2024 rebrand; standalone API sunset). Chorus.ai → ZoomInfo Chorus (Jul 2021, $575M). |

## Per-domain depth [✓ all 8 + AgentOps shipped]

Each domain file passes the v3 quality bar (≥10 primary sources, ≥3 case studies, ≥1 tactical playbook, head-to-head tool table, cross-refs).

| Domain | Anchor case shipped | Headline new content |
|---|---|---|
| **0. AgentOps** | Klarna 700-FTE-equivalent / re-balance (LangChain) + Replit production-DB-deletion incident | Klarna, ServiceNow, Decagon AQS, Replit, Air Canada, DPD, McDonald's-IBM, Anthropic Managed Agents (8 case studies); LangSmith / AgentOps.io / Helicone / Langfuse comparison; SUPERWISE vs. IBM watsonx.governance; Brand Governance Agent Mermaid diagram + 4-playbook stack |
| **1. Sensing** | Anthropic + Clay (3× enrichment, canceled top legacy contract) | 6sense 2025 (94% / 77% / 95% Day One Shortlist); Vendr median ACV pricing; Forrester Wave Q1 2025 leaders; Clay+n8n architecture diagram; 6 named cases (Anthropic, OpenAI, Notion, Semgrep, LeanIX, Cobalt) |
| **2. Strategy** | Brand.ai (Lyft, Opendoor), $5M/yr → fraction; one copywriter, 600 pieces | Dunford Mar 2026 quotes + Raskin verbatim; 5 named cases (Userlist, Influ2, Workday, Superhuman, Brand.ai); 8-agent Brand Governance Agent build (Animalz pattern); Wynter / SparkToro / PyMC sequencing; Klue / Crayon / custom Clay comparison |
| **3. Content** | Anthropic's own growth team, 30 min → 30 sec, 10× output | Jasper 2026 (91% adoption / governance up 3.4× YoY); McKinsey Apr 2026; 7 named cases; Jasper / Writer / Custom Claude TCO; LangGraph + Skills Mermaid diagram; customer-language capture workflow; AEO-first brief template; Handley + Rose verbatims (incl. "Slop is generated. Craft is built and made.") |
| **4. Distribution** | Refine Labs / Passetto, $50M HIRO / $14M ARR; 93% gap vs. software attribution | Walker + Welsh + Simmonds verbatims; 6 named cases (Vandenberghe 50% pipeline, Recall.ai 40K LinkedIn, Refine Labs, Genesys, Dell+EA, podcast guesting $680K); 1-3-5 atomization method; two-stack social management thesis; Cision Trajaan acquisition framed as PR↔AEO crossover |
| **5. AEO/GEO** | Vercel, <1% → 10% of new signups from ChatGPT in 6 months | Solis + Ray + King verbatims (incl. Ray's "AI Slop Loop"); 6 named cases (Ramp 7×, Rootly 10×, Grüns 23×, Popl 1,561% ROI, Vercel signups, Anthropic llms-full.txt pattern); Profound vs. AthenaHQ vs. Peec AI vs. Bluefish comparison; Bing AI Performance launch (Feb 2026); llms.txt deployment patterns (Anthropic / Vercel / Cloudflare) |
| **6. Demand** | SaaStr, 20 AI agents + 1.2 humans, 70K emails/mo, 15% of London revenue | Lemkin verbatims; 6 named cases (SaaStr, Broadvoice 40% pipeline, Salesloft Rhythm benchmarks, Ideals 452 meetings, FERMÀT 5d→<3d, Apollo $150M ARR); Outreach Aug 2025 + Salesloft Dec 2025 product launches; sender reputation auto-pause (May 2025 Google/Yahoo/MSFT thresholds); 7-element conversation handoff bundle; hybrid AI+human Mermaid diagram |
| **7. Customer Intel** | CVS Health × Simile, 2.9M consented responses, 100K+ agentic twins | Park 85% accuracy correction (was miscited 94%); Toubia "Funhouse Mirrors" critique (0.197 average twin-to-human correlation, 93.9% twin-SD-lower); 5 cases (CVS, EY×Evidenza 95%, Aaru NY primary, PandaDoc×Wynter, PyMC validation); Simile / Aaru / Ditto / Synthetic Users / Evidenza comparison; AI-interview-hybrid distinction (Listen Labs / Outset / Keplar are NOT synthetic) |
| **8. Measurement** | Refine Labs $50M HIRO + PODS Recast +181% Google Non-Brand | IAB/BWG 2026 (75% measurement-inadequacy stat); AIMx framework paper; 7 cases (PODS, Soft Surroundings 52% retargeting cut → +17% revenue, Refine Labs $50M, Lifesight retailer +32%, Lifesight $1B gaming, Jones Road geo-test, Semgrep +74%); Measured / Recast / Lifesight comparison; open-source Robyn / Meridian / PyMC-Marketing head-to-head; triangulation Mermaid diagram |

## Site experience [✓ shipped]

- ✓ Single-file HTML viewer with sidebar navigation (`v3/index.html`, 416K)
- ✓ Hash-based routing (`#0-agentops`, `#5-ai-search-answer-visibility`, etc.)
- ✓ Cross-file `.md` links auto-rewritten to in-app navigation
- ✓ External links open in new tab
- ✓ Dark mode (matches `prefers-color-scheme`)
- ✓ Mobile sidebar (hamburger, bottom-sheet)
- ✓ Mermaid diagram rendering (theme-aware light/dark)
- ✓ Blockquote styling (orange-bordered, accent-soft background)
- ✓ Maturity matrix view (`#maturity`):
  - 8×4 grid, click any cell → drawer with full detail
  - Domain pill selection → row highlight + journey view (4 stage cards)
  - Self-assessment (8 questions → automatic stage placement)

## Frontiers expansion [✓ shipped]

10 frontiers in [agentic-marketing-os-v2.md Part VII](agentic-marketing-os-v2.md#part-vii--open-questions-and-frontiers-q2-2026-update), each with **current state + leading indicators + practical move**:

1. Agent-to-agent commerce + protocols (MCP donated to Linux Foundation Dec 9, 2025)
2. Brand-to-LLM communication (OpenAI ads in ChatGPT testing Jan 16, 2026)
3. The Ghost Workforce labor problem (Robert Rose CMI Apr 2026 research)
4. Regulated-industry synthetic methodology (FDA NAM draft Mar 18, 2026)
5. AI-Agent Buyer Behavior (Gartner $15T forecast)
6. The Accountability Question (EU AI Act Aug 2, 2026 enforcement)
7. Saturation / Commoditization (a16z Momentum-as-Moat thesis)
8. Sentiment Risk in AI Search
9. Wikipedia Editorial Wars (Mar 20, 2026 ban, 44-2 vote)
10. The Creative Quality Ceiling (Apple Creator Studio Pro Jan 2026)

## What was deferred from the original plan (honest list)

These items were in the v2 → v3 plan but did **not** ship:

| Item | Why deferred |
|---|---|
| **Mahmoud's own Space & Story SSR migration case** (Domain 5) | Requires Mahmoud's first-party data (before/after AI traffic numbers). Plan calls for it; only Mahmoud has the data. Slot exists in Domain 5 to add when Mahmoud provides numbers. |
| **Per-archetype reference implementations (2-3 each × 6 archetypes)** | v3 ships 4 cross-archetype references at top of `archetypes.md` (anthropics/skills, deepagents content-builder-agent, crewAI-examples, Anthropic Building Effective Agents). v4 expands to per-archetype detail. |
| **Anti-patterns per archetype** | ✓ Actually shipped, added to archetypes.md as a dedicated section. |
| **Archetype chaining patterns (multiple worked examples)** | v3 ships 1 example chain (account research → outreach). v4 adds 2-3 more (content production, measurement loop, brand governance). |
| **One Wikipedia/Wikidata entity-presence case** (Domain 5) | Vercel + Anthropic llms-full.txt cases shipped (better-documented). Wikipedia case would be Anthropic itself but lacks public before/after numbers. |
| **One agent-drift incident with detection + remediation** (Domain 0) | DPD + Replit incidents shipped (drift-related); explicit "drift detected → remediated → resolved" timeline case is rare in public reporting. v4 candidate if a public post-mortem lands. |

## v3 Definition of Done, final scoring

Original criteria from v2 → v3 plan:

- [x] All cross-cutting validation items (V1-V5) resolved.
- [x] Every domain file passes the quality bar (10+ primary sources, 3+ case studies, 1+ playbook, 1+ tool comparison, cross-references to Mahmoud skills).
- [x] All vendor M&A and naming updated to current state.
- [x] AI Overview citation stat reconciled with a single, sourced statement.
- [x] Each domain file's expansion checklist closed (replaced with "v3 shipped" + v4 deferred).
- [x] Resource library pruned of stale entries and refreshed with 2025-2026 additions.
- [x] An "open questions / frontiers" note in each domain file flags where the field is still moving (handled centrally in Part VII).

---

# Part 2, v4 (forward plan, 2026 onward)

The framework is now structurally complete. v4 is **maintenance + selective deepening + experience layer**, not another foundational rewrite.

## v4.1. Mobile-first reading experience (separate workstream)

Tracked separately. Sprint plan exists; will be executed via Mahmoud's `mahmouds-seo-writer` skill so the rewrites get AEO-optimized treatment in the same pass.

Mobile-essential moves:
- Mobile matrix view (replace 8×4 grid with stacked accordion + horizontal stage carousel)
- Per-page sticky table of contents (sidebar on desktop, bottom-sheet on mobile)
- Reading time + scroll progress
- Section anchors with copy-link
- Tables → cards on mobile

## v4.2. Quarterly stat-refresh cadence

Public commitment: every quarter, mine the highest-signal new sources and update.

**Q3 2026 refresh targets** (themes likely to move):
- New 6sense Buyer Experience Report (annual, typically Nov)
- Conductor 2027 AEO/GEO Benchmarks (if released)
- Jasper "State of AI in Marketing 2027"
- IAB / BWG "State of Data" annual update
- New Ahrefs / seoClarity / BrightEdge AI search studies
- McKinsey agentic AI updates
- FDA NAM draft → final guidance status (Mar 2026 → ~Q4 2026)
- EU AI Act enforcement actions post-Aug 2, 2026

**Cadence rule:** if a stat is older than 12 months and the field has moved, retire or update.

## v4.3. Per-domain v4 enrichments

| Domain | What v4 adds |
|---|---|
| **0. AgentOps** | Per-archetype reference implementations (2-3 per archetype × 6 archetypes); 2-3 more architecture diagrams (cost auto-pause, multi-agent observability dashboard, MCP server publishing pattern); first agent-drift post-mortem when one becomes public |
| **1. Sensing** | LLM-visibility intent tooling deep-dive as the category forms; 2-3 more biopharma cases (KOL graph, Veeva Link, Komodo Health) |
| **2. Strategy** | Brand Governance Agent regression-set methodology + violation-rate benchmark; pricing-as-positioning case in regulated industries |
| **3. Content** | Per-team productivity benchmarks at scale; brand-voice fidelity scoring methodology when one is published |
| **4. Distribution** | Founder-led marketing data when LinkedIn slop saturation is empirically measurable; podcast-guesting attribution methodology |
| **5. AEO/GEO** | Mahmoud's own Space & Story SSR migration case (when data is provided); Wikipedia/Wikidata entity-presence case with documented LLM-citation lift; Bing Webmaster Tools "AI Performance" usage patterns at scale |
| **6. Demand** | Second-wave AI SDR cases (post-2025 collapse), what actually works; conversation-handoff impact at named enterprise B2B |
| **7. Customer Intel** | Continuous-calibration methodology (synthetic-to-live correlation tracking); first regulated-industry public failure case to clarify boundaries |
| **8. Measurement** | Real-time MMM agentic-decision case study with named brand; LLM-citation-attribution closed-loop |

## v4.4. Archetype layer expansion

- 2-3 reference implementations per archetype (currently 4 cross-archetype references; v4 distributes these per archetype + adds new)
- 3 more archetype-chaining example workflows beyond v3's account-research → outreach example:
  - **Content production chain**: Knowledge → Analyzer (citation gap) → Planner (brief) → Content Generator → Brand Governance → Operator (publish + measure)
  - **Measurement loop chain**: Operator (run experiment) → Analyzer (incrementality) → Planner (budget reallocation) → Operator (deploy) → loop
  - **Brand governance chain**: 8-agent parallel reviewers → Aggregator → Decision (auto-publish / human review / block) → audit log

## v4.5. Frontier status updates (each frontier reviewed quarterly)

For each of the 10 frontiers in Part VII:
- Update "current state" with new sources
- Add new leading indicators or retire ones that resolved
- Refresh "practical move today" if the field changed

**Frontiers most likely to move in Q3-Q4 2026:**
- Agent-to-agent commerce (UCP / ACP convergence?)
- The Accountability Question (first EU AI Act enforcement)
- Wikipedia Editorial Wars (will other language editions follow English ban?)
- AI-Agent Buyer Behavior (early measurement of "Agent Engine Optimization")

## v4.6. Open questions to seed v5 research

Tracked here, not addressed in v4:

- Will MMM fully replace MTA for B2B by 2027?
- What's the credibility ceiling of synthetic research in regulated industries?
- How do you measure agentic-stack ROI itself (the meta-measurement question)?
- Does brand-voice fine-tuning beat brand-voice prompting at enterprise scale?
- What's the "Agent Engine Optimization" successor to AEO?
- Will OpenAI's "Sponsored" labeling hold the answer-influence wall?

---

# Methodology (applies to v3 and v4)

## Source hierarchy (best to worst)

1. **Primary research**, academic papers, original survey reports (Conductor, 6sense, Jasper, McKinsey), vendor case studies with numbers, post-mortems on production deployments.
2. **Practitioner-led primary sources**, original posts/videos from named experts (Dunford, Walker, Solis, Park, etc.) describing their own work.
3. **Aggregator/analyst content**. Forrester, Gartner, IDC reports; First Round, a16z, McKinsey writeups.
4. **Tool documentation + product pages**, only for capability mapping, never for performance claims.
5. **General SEO/marketing blogs**, last resort, only when corroborating primary claims.

**Rule:** every statistic must trace to a named source with a date. If a claim can't be traced, either remove it or label it "anecdotal."

## Quality bar (v3, maintained for v4)

Each domain file must:
- Have ≥10 cited primary sources (URL + date + author).
- Include ≥3 named case studies with before/after numbers.
- Include ≥1 build-this-yourself tactical playbook (prompts, configs, or decision tree).
- Include a head-to-head tool comparison table (price, fit, switching cost) for the top 3-5 tools in that domain.
- Cross-reference Mahmoud's relevant existing skill(s), never duplicate; always link.
- Pass the "would Aleyda Solis / April Dunford / Chris Walker quote this?" test.

## Integration with Mahmoud's existing skills

| Domain | Mahmoud's skills to integrate |
|---|---|
| 1. Sensing | `customer-research-playbook`, `competitor-research-playbook` |
| 2. Strategy | `product-marketing-context`, `pricing-strategy`, `copywriting`, `competitor-alternatives` |
| 3. Content | `mahmouds-seo-writer`, `copy-editing`, `lead-magnets`, `ad-creative` |
| 4. Distribution | `mahmouds-reddit-strategist`, `community-marketing`, `email-sequence`, `cold-email`, `directory-submissions`, `launch-strategy` |
| 5. AEO/GEO | `mahmouds-seo-guide-v3` (especially `aeo-geo-playbook.md`), `mahmouds-seo-writer` |
| 6. Demand | `cold-email`, `signup-flow-cro`, `form-cro`, `revops` |
| 7. Customer Intelligence | `customer-research-playbook` (heavy overlap) |
| 8. Measurement | `ab-test-setup`, `mahmouds-seo-guide-v3` (`analytics-measurement.md`) |
| 0. AgentOps | `claude-api`, `update-config` |

**Approach:** when a domain file has a tactic that's already in a Mahmoud skill, link out instead of restating. This keeps the OS doc strategic and the skills tactical.

## Workflow tools (used for v3, repeat for v4)

- **WebSearch + WebFetch** for primary sources, news, vendor pages.
- **Agent (Explore)** for initial scoping of a domain's information landscape ("medium thoroughness").
- **Agent (general-purpose)** for parallelized multi-source research dives, used heavily in v3 (4 parallel agents per phase).
- **Mahmoud's existing skills**, load before any domain-specific work (especially `mahmouds-seo-guide-v3` for Domain 5).

## v3 retrospective, what worked

- **Parallelizing 4-6 research agents per phase** delivered Phase 1 + Phase 2 in one session and Phase 3-4 in a second. Single biggest velocity unlock.
- **Cross-cutting validation first** (V1-V5) prevented compounding errors when the same stat appears across multiple files.
- **Quality bar checklist** ensured nothing shipped half-baked.
- **Cross-link audit script** caught silent gaps that would have been invisible without instrumentation.

## v3 retrospective, what to fix in v4

- **Per-domain checklist stubs were left unchecked even after work shipped**, created confusion. v4 closes them with explicit "shipped" markers.
- **One full pass at the resource library was deferred**. Drift entries lingered until specifically flagged. v4 adds an automated check.
- **Mobile experience was not part of v3 scope** but is a real usage gap. v4.1 addresses.
