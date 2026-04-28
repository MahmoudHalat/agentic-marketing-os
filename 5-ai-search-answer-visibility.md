<!--
seo:
  title: AEO, GEO, LLMO: AI Search Answer Visibility in 2026 — Domain 5
  description: Get cited in ChatGPT, Perplexity, AI Overviews. Vercel <1%→10% ChatGPT signups, Ramp 7×, Rootly 10×, Profound vs AthenaHQ comparison, llms.txt deployment patterns.
  primary_keyword: AEO GEO AI search optimization
  secondary_keywords: [llms.txt, AI Overview citations, ChatGPT optimization, AthenaHQ vs Profound, Bing AI Performance, Wikipedia entity]
-->
## Domain 5: AI Search & Answer Visibility (AEO/GEO/LLMO)

> **TL;DR.** The newest standalone discipline. **Anchor stat: 38% of Google AI Overview citations come from pages ranking in Google's top 10** (down from 76% in July 2025; [Ahrefs Mar 2026](https://ahrefs.com/blog/ai-overview-citations-top-10/)). For non-Google LLMs, ~80% of citations come from pages that don't rank in Google's top 100 ([Ahrefs Aug 2025](https://ahrefs.com/blog/ai-search-overlap/)). **Tools that win:** Profound or AthenaHQ for tracking, Bing Webmaster Tools "AI Performance" (free, Feb 2026 launch), llms.txt + llms-full.txt published. **Canonical case: Vercel** — <1% → 10% of new signups from ChatGPT in 6 months. **What changed in v3:** added 6 named cases (Ramp 7×, Rootly 10×, Grüns 23×, Popl 1,561% ROI, Vercel signups, Anthropic llms-full.txt pattern), Profound vs. AthenaHQ vs. Peec AI vs. Bluefish comparison, llms.txt deployment patterns (Anthropic two-tier / Vercel use-case-mapped / Cloudflare product-modular), Bing AI Performance launch.

> *"A brand can now be surfaced, recommended, and materially influence a purchase decision in AI search without necessarily generating a click."* — Aleyda Solis, [*A 3-Layer Framework to Measure AI Presence*](https://www.aleydasolis.com/en/ai-search/a-3-layer-framework-to-measure-ai-presence-readiness-and-business-impact-redefining-metrics-for-the-ai-search-era/), Apr 23, 2026

> *"For a RAG-based system like Perplexity or AI Overviews, enough citations are basically all it needs to treat something as fact, regardless of whether it's actually true."* — Lily Ray, [*The AI Slop Loop*](https://lilyraynyc.substack.com/p/the-ai-slop-loop), Apr 14, 2026

> *"we need to reinvent ourselves. And that reinvention I'm calling is relevance engineering."* — Mike King, [Search Engine Land SMX Advanced 2025 interview](https://searchengineland.com/mike-king-smx-advanced-2025-interview-456186), May 29, 2025

**See also:** Mahmoud's [`aeo-geo-playbook.md`](skill) for the tactical depth (query fanout, ranking factors, money-pages strategy), Mahmoud's [`mahmouds-seo-writer`](skill) for AEO content brief execution, [Domain 3 (Content)](3-content-creative-production.md) for AEO-first content briefs, [Domain 4 (Distribution)](4-distribution-channel-operations.md) for Cision Trajaan + entity-presence building, [Domain 8 (Measurement)](8-measurement-attribution.md) for the AI-search KPI layer, [Domain 0 (AgentOps)](0-agentops.md) for output validation in AI-search content, [Domain 1 (Sensing)](1-sensing-intelligence.md) for the new "LLM-visibility intent" frontier.

### Definition and Scope

The newest standalone discipline, formerly buried inside SEO. Now its own domain because the mechanics are structurally different. Owns: entity presence in LLM training and retrieval; structured content for extractability; citation-earning PR strategy; multi-platform AI visibility tracking (ChatGPT, Claude, Perplexity, Gemini, Copilot); schema markup; llms.txt; and corroboration signals across the wider web.

The acronym soup:
- **SEO**. Search Engine Optimization (the original)
- **AEO**. Answer Engine Optimization (structuring content so engines can extract it as direct answers)
- **GEO**. Generative Engine Optimization (visibility within LLM responses from ChatGPT, Claude, Perplexity, Gemini)
- **LLMO**. LLM Optimization (broader than GEO; includes entity-level presence in training data)
- **AI SEO**, umbrella term covering all of the above

Most teams treat these as overlapping disciplines under one strategy. The distinction: AEO focuses on extractable passages; GEO covers the broader generative surface; LLMO adds the entity-level training-data dimension.

### Why It Matters Now

The data is decisive: As of Q1 2026:
- ChatGPT has surpassed 900 million weekly active users.
- Google AI Overviews appear in 25.11% of searches ([Conductor 2026 AEO/GEO Benchmarks Report](https://www.conductor.com/academy/aeo-geo-benchmarks-report/), April 2026, analyzed 21.9M searches across 13,770 enterprise domains).
- AI referrals are 1.08% of total traffic on average; ChatGPT = 87.4% of AI referrals (Conductor 2026). Category-level variance is large. Vercel reported 10% of new signups from ChatGPT in 6 months (developer-tool category).
- **The citation-and-rank stat (canonical):** Only **38% of Google AI Overview citations** come from pages that rank in the top 10 for the original query, down from 76% in July 2025 ([Ahrefs, "Update: 38% of AI Overview Citations Pull From The Top 10," March 2, 2026](https://ahrefs.com/blog/ai-overview-citations-top-10/), n=863K SERPs). The decline reflects Google's increased reliance on fan-out subqueries, not a real decline in top-10's importance. **For non-Google LLMs** (ChatGPT, Gemini, Copilot), the gap is wider: ~80% of citations come from pages that don't rank in Google's top 100 for the *original* prompt ([Ahrefs, "Only 12% of AI Cited URLs Rank in Google's Top 10," August 11, 2025](https://ahrefs.com/blog/ai-search-overlap/), n=15K queries). Perplexity is the exception (28.6% in top 10). Other studies report different overlaps (seoClarity Oct 2025 found 32% on a different methodology; BrightEdge 54%), read methodology before quoting.
- Gartner predicted traditional search volume would drop 25% by 2026, playing out in real time.

Translation: the rules have changed. Pages that rank in Google often don't get cited by LLMs. Pages that rank nowhere on Google can still be cited heavily. Optimizing only for SEO leaves you invisible in the channel that will increasingly drive discovery.

The economic case: McKinsey projects ~$750 billion in **US** revenue flowing through AI search by 2028 ([McKinsey, "New front door to the internet,"](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/new-front-door-to-the-internet-winning-in-the-age-of-ai-search) Nov 2025, note: US-only forecast, ~75% of $1T total search market). This is no longer an "experiment" line item.

### Sub-Domains

**5.1 Answer Engine Optimization (AEO)**
- Question-led headings (H2/H3 as direct questions)
- One-sentence answers immediately under each heading
- Definitional paragraphs (the "what is X" pattern)
- Schema markup (FAQ, HowTo, Article, Product)
- Featured snippet optimization

**5.2 Generative Engine Optimization (GEO)**
- Content structuring for LLM retrieval
- Citation-earning content (statistics, original research, primary data)
- "Quotable insights", content designed to be extractable as a quote
- Multi-platform optimization (different LLMs cite differently)
- llms.txt (proposed standard for LLM-readable site maps)

**5.3 LLM Optimization (LLMO) / Entity Building**
- Brand entity presence across the wider web
- Wikipedia / Wikidata presence
- Schema.org Organization markup
- Cross-domain mentions and corroboration
- Author / expert E-E-A-T signals
- Influence over training data (limited but real)

**5.4 Measurement & Visibility Tracking**
- LLM citation monitoring (which LLMs cite you, for what queries?)
- Share of voice across AI search platforms
- Sentiment analysis in AI responses
- Competitive AI visibility benchmarking

**5.5 PR-Driven Citation Building**
- Press release distribution (PR Newswire, BusinessWire)
- Data-driven research that earns citations
- Industry report sponsorships
- Earned media that feeds LLM training

**5.6 Technical AI-SEO Foundations**
- Server-side rendering (SSR), critical, since many AI crawlers don't execute JavaScript
- Site speed and Core Web Vitals
- Structured data validation
- robots.txt and AI crawler permissions
- llms.txt and llms-full.txt

### Best Practices in 2026

**Stop chasing prompts; start tracking entity presence.** As one expert put it: if your brand is being cited, summarized, or referenced by AI, you're not just visible, you're trusted by the systems shaping the future of search. Track entity presence over time as the primary KPI.

**Invert your content research workflow.** Instead of starting with keyword volume, start with how the LLMs currently answer your target questions. Identify gaps, biases, or incomplete answers. Produce content that fills the void. Teams using this approach report 3x higher citation rates.

**Make every page extractable.** Question-led H2s. One-sentence answers. Tables for comparison content. Lists for steps. Definitional paragraphs at the top. AI systems do not want vague marketing copy; they want stable, well-structured source material.

**Build corroboration across the wider web.** A page that exists only on your domain is harder to validate. Pages cited and linked to from elsewhere, third-party publications, analyst reports, podcasts, communities, get more LLM trust. This is why analyst relations + PR matter for AEO/GEO.

**Update key pages more often than you used to.** AI systems are heavily exposed to fast-moving categories. A page that hasn't been updated since 2023 looks stale and gets bypassed. Treat key pages as living documents.

**Don't kill SEO; expand it.** AEO is not a replacement for SEO, it's an extension. Traditional SEO is still required for being crawlable, indexed, and authoritative. AEO adds the answer-extractability layer. The most effective 2026 strategies integrate both under a unified search-visibility team with shared KPIs.

**Choose your distribution sources for AI training, not just for SEO.** Pages on Reddit, GitHub, YouTube, and Wikipedia have outsized influence on what LLMs know. [Profound × Reddit's 4-billion-citation analysis](https://rosssimmonds.com/blog/visibility-llms/) found Reddit accounts for 3.11% of all AI citations, 45% more than YouTube, 2× Wikipedia. Distribution strategy now includes "show up in places LLMs trust."

### Named Case Studies (with before/after numbers)

| Brand | Tool / approach | Result | Source |
|---|---|---|---|
| **Ramp** | Profound — built two AEO money-pages (Accounts Payable for SMB, Accounts Payable for Large Biz) + comparison content | AI visibility **3.2% → 22.2% (7×)** in one month; 300+ citations from 2 pages; doubled overall citations vs. all prior content combined; rose from 19th to 8th most-visible fintech in Accounts Payable | [Profound case](https://www.tryprofound.com/customers/ramp-case-study) |
| **Rootly** | AthenaHQ — competitive baseline, weekly content shipping, focus on **unbranded** evaluation prompts | Citation rate **3% → 30% (10×)**; mention rate 7.5% → 18.3%; non-branded mention lift 2.5×; equivalent media value $87K → $214K | [AthenaHQ case](https://www.athenahq.ai/case-studies/10x-citation-rate-rootly-geo-case-study) |
| **Grüns** | AthenaHQ — pillar-and-cluster + 15 articles, programmatic scaling via Shopify integration | 60-day result: SoV **2.0% → 12.6% (6×)**; citation rate **0.3% → 7.0% (~23×)**; brand mention rate 4.0% → 25.0%; ~10,500 LLM impressions | [AthenaHQ case](https://athenahq.ai/case-studies/10-6pp-sov-gruns-ai-search-case-study) |
| **Popl.co** | AthenaHQ — content restructured for AI extraction; multi-platform optimization | 3-month result: AI Search rank **5th → 1st**: AI visibility 10% → 28.9% (+189%); monthly citations 23 → 212 (+822%); 38.85% MoM lead growth from AI search; **ROI 1,561%, 18-day payback** | [AthenaHQ case](https://athenahq.ai/case-studies/38-mom-growth-leads-popl-ai-search-leadership) |
| **Vercel** | llms.txt + llms-full.txt via Mintlify | **<1% → 10% of new signups from ChatGPT** in 6 months | [Mintlify post](https://www.mintlify.com/blog/the-value-of-llms-txt-hype-or-real) |
| **Anthropic** | Co-developed the llms-full.txt format with Mintlify; slim `/llms.txt` index → larger `/llms-full.txt` Markdown export of full Claude docs corpus | Two-tier pattern adopted by major dev-tools (Cursor, Coinbase, Pinecone, Windsurf, Cloudflare) | [Mintlify customer page](https://www.mintlify.com/customers/anthropic) |

**Methodology caveat (worth flagging):** in several AthenaHQ case studies, ~70% of cited content was *written by AthenaHQ itself*. Profound's enterprise customers (Ramp, MongoDB, Figma) wrote their own content, which makes Profound's evidence base methodologically cleaner. Both vendors publish only positive cases. To validate vendor-reported lift, run the same brand simultaneously across Profound + AthenaHQ + a third tool for 90 days and reconcile.

**Directional case studies (less rigorous, vendor-published):** Lago, 50% increase in demos from AI Search, AI Overview impressions 3% → 33%, citation rate 3.5% → 17%. Verito, 36% Share of Voice on ChatGPT in 6–8 weeks (vs. competitors 25–30× larger). AutoRFP.ai, 10× ChatGPT traffic, >30% of prospects from GenAI Search.

### Tools & Platforms

#### AEO/GEO tracking comparison (Q1 2026)

| Tool | Pricing | AI platforms tracked | Tracking method | Best for | Key limitation |
|---|---|---|---|---|---|
| **Profound** | Starter $99/mo (ChatGPT only); Growth $399/mo (3 engines); Enterprise $2K–$5K+/mo | ChatGPT, Perplexity, Google AIOs at Growth; +Claude, Gemini, Grok, Copilot at Enterprise | API + scraped hybrid (proprietary "Answer Engine Insights"); shows actual prompt **volume** | Enterprise (Target, Walmart, Figma, MongoDB, Ramp, Chime, U.S. Bank, Charlotte Tilbury) | High cost; lower-tier plans gate Claude/Gemini |
| **AthenaHQ** (formerly OtterlyAI) | $295/mo single plan with credits + Action Center | ChatGPT, Gemini, Google AIOs, Perplexity, Copilot | Scraped UI responses | Mid-market needing **content generation + tracking** in one tool; e-commerce/Shopify; published case-study leader | "Athena-authored" content credibility caveat (see Case Studies section) |
| **Peec AI** | €89/mo starter; €199/mo+ for higher volume | ChatGPT, Perplexity, Claude, Gemini, Google AIOs | UI scraping; "Earned Media" module tracks Reddit/Wikipedia/G2 sources | Tactical product marketing; SaaS/D2C; multi-language (115+) | Single-brand focus; limited exports |
| **Bluefish AI** | Quote-based / custom (raised $20M, 2025) | ChatGPT, Perplexity, Google AIOs, Gemini | Real-time monitoring; proprietary Impact Score + Influence Rank | Fortune 500 brand-safety + AI hallucination monitoring (Adidas, Tishman Speyer); AI Commerce module | Per-seat model; opaque tracking method |
| **SE Visible** (SE Ranking) | Bundled into SE Ranking subscription (no AI add-on charge) | ChatGPT, AI Mode, Perplexity, Gemini | Scraped | Teams already on SE Ranking; predictable cost | Not a dedicated AEO platform |
| **HubSpot AI Search Grader** | **Free**; no signup | GPT-5.2, Perplexity, Gemini (cross-validated) | One-shot diagnostic snapshot | First-touch diagnostic; small-team baselining | One-time, not continuous |
| **Conductor** | Enterprise quote | All major engines + AIOs | Proprietary aggregation (publisher of the 2026 Benchmarks Report) | Large enterprise SEO teams already on Conductor | Heavy platform; not a quick-buy |

**API-vs-scraped tracking warning** (per Mahmoud's [`aeo-geo-playbook.md`](../../.claude/skills/mahmouds-seo-guide-v3/references/aeo-geo-playbook.md)): API responses average 7 sources / 406 words; scraped web responses average 16 sources / 743 words. Brand overlap between API and scraped is only **24%**; source overlap is **4%**. Perplexity API vs. web overlap is just 8%. **Tools that rely on API tracking systematically under-report what real users see.** Of the platforms above, Peec AI, AthenaHQ, and SE Visible explicitly use UI scraping; Profound is hybrid; Bluefish's method is opaque.

**Hybrid SEO + AEO Tools**
- **Semrush**, adding LLM citation monitoring
- **Ahrefs**. SEO foundations + AI tracking expansion (publisher of the 38% / 12% citation studies)
- **Surfer SEO**, content optimization (now AEO-aware)
- **Sight AI**, content workflow + AI visibility (tracks brand mentions in ChatGPT/Claude/Perplexity + content gen + IndexNow)
- **Frase**, question-driven briefs (AEO-native approach); **GEO tracking across 5 AI platforms** at one-fourth Clearscope price

**First-party publisher tracking**
- **[Bing Webmaster Tools "AI Performance"](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview)**. Public preview launched Feb 10, 2026. Surfaces Total Citations, Average Cited Pages, **Grounding Queries** (the actual sub-queries LLMs fan out to retrieve content), and page-level citation activity. **Free, first-party, not behind any vendor's pay-wall.** This is now the Microsoft equivalent of Google Search Console for the AI search era, track it weekly.

**Schema & Technical**
- **Schema.org** validators
- **Google Rich Results Test**
- **llms.txt generators**

**PR & Citation Distribution**
- **PR Newswire AEO & GEO Brand Report** (Cision), citation-driven distribution
- **BusinessWire**
- **Muck Rack**, journalist relationships
- **HARO / Qwoted / Help A B2B Writer**, expert quote sourcing (citation-building)

### Notable Practitioners & Frameworks

- **Aleyda Solis (Orainti)**, global SEO + AEO authority
- **Lily Ray (Amsive)**. E-E-A-T, helpful content, Google updates
- **Marie Haynes (MHC)**. Google AI search analysis
- **Cyrus Shepard (Zyppy)**, modern SEO, internal linking
- **Brian Dean (Backlinko, sold to Semrush)**, content marketing
- **Kevin Indig**, growth-focused SEO
- **Mark Webster + Gael Breton (Authority Hacker)**. AI + SEO operations
- **Eli Schwartz**; *Product-Led SEO*; bottom-up SEO
- **Ross Simmonds (Foundation)**, content distribution + AI search

### Industry overlay (Q2 2026)

| Industry | ICP / motion difference | Tools that win | Biggest pitfall | Compliance overlay |
|---|---|---|---|---|
| **B2B SaaS** | ChatGPT (87% of AI referrals per Conductor), Perplexity, Google AIOs, Gemini. Vercel-style "% of new signups from ChatGPT" North Star applies | Profound or AthenaHQ for tracking; Bing Webmaster AI Performance (free); llms.txt + llms-full.txt; Reddit/G2/listicle citation building | Optimizing for keywords while ignoring grounding queries — pages that rank don't get cited (only 38% overlap with AIO) | None |
| **Biopharma** | Scientific buyers query PubMed, Embase, Cochrane, Wikipedia, UpToDate, KOL Twitter/Bluesky — *not* ChatGPT for clinical decisions. HCPs distrust LLM answers; they verify in PubMed | **PubMed/MeSH SEO**: Wikipedia/Wikidata entity work (highest-leverage asset for biopharma); Open Pharma's open-access publishing; Google Scholar profiles for thought leaders; OpenAlex | Optimizing biopharma marketing pages for ChatGPT citations on disease state queries — generates off-label promotion exposure. LLMs hallucinate dose/MoA; you cannot let your domain be the corroboration | Off-label promotion risk on AI-generated clinical content; FDA crackdown on AI-surveilled DTC (Sept 2025) targets AI-generated health content; ICMJE authorship rules for AI co-authored papers |
| **DTC** | Google AIOs + Pinterest visual + TikTok search are dominant; ChatGPT product recs growing. Reviews on Amazon/Trustpilot/Reddit drive LLM citations | Reddit reputation work; review velocity (Yotpo, Okendo); Pinterest SEO; GS1 product schema; Looka for product Q&A snippets | Letting Reddit complaints become the canonical AI-cited source for your brand — Profound found Reddit = 3.11% of all AI citations | FTC review authenticity rules (2023 update on undisclosed/fake reviews — $51K per violation) |
| **Dev tools** | LLMs ARE the buyer. Cursor/Windsurf/Claude Code + GitHub Copilot pull docs into context. **llms.txt + llms-full.txt mandatory.** Anthropic, Vercel, Cloudflare patterns are canon | Mintlify (docs + llms.txt native); Anthropic two-tier llms.txt pattern; OSS examples on GitHub; Stack Overflow answers; technical YouTube | Hiding API docs behind auth, JS-rendering them, or not publishing llms-full.txt — Cursor/Claude Code can't see your product, devs pick a competitor whose docs they can | None beyond standard |

**Key insight:** For biopharma, AEO is *inverted*, the goal is often to *not* be cited in clinical-decision LLM contexts where you'd be making implied off-label claims. Wikipedia and PubMed are the citation universe; treat ChatGPT/Perplexity as advisory channels for non-promotional corporate content (R&D pipeline, ESG, careers) only.

### Common Failure Modes

- **Optimizing for SEO and assuming AEO follows.** It doesn't. The pages that rank in Google often don't get cited by LLMs.
- **Ignoring server-side rendering.** Many AI crawlers can't execute JavaScript. Client-rendered content is invisible to them. (Mahmoud, your Space & Story site has been hit by exactly this problem.)
- **Treating AEO as a one-time content audit.** It's a continuous discipline. AI systems update; your content has to keep up.
- **Spamming press releases to chase citations.** LLMs detect low-quality PR distribution. Quality > volume.
- **Forgetting Wikipedia.** For B2B brands above a certain size, the Wikipedia entry is the single highest-leverage AEO/GEO asset. Earning one is hard; maintaining it is essential.
- **Optimizing only for ChatGPT.** Different LLMs cite different sources. A multi-platform strategy is required.

### KPIs

- **Citation rate**; % of target queries where you're cited by ≥1 LLM
- **LLM share of voice**, your share of citations vs. competitors, per query
- **Citation diversity**, citations across ChatGPT / Claude / Perplexity / Gemini / Copilot
- **AI Overview presence**; % of target queries where you appear in Google AI Overview
- **Sentiment in AI responses**, positive / neutral / negative framing
- **AI referral traffic**, traffic from AI search platforms (Perplexity, ChatGPT, etc.)
- **AI referral conversion rate**, typically 5x higher than Google organic; track per-platform
- **% of new signups from ChatGPT** (Vercel-style North Star), the highest-stakes outcome metric for B2B SaaS; Vercel went <1% → 10% in 6 months as the proof point.

### Tactical Playbooks

#### Playbook A; `llms.txt` template + maintenance cadence

**Real-world deployment patterns** (beyond the basic SaaS template in Mahmoud's [`aeo-geo-playbook.md` Section 9](../../.claude/skills/mahmouds-seo-guide-v3/references/aeo-geo-playbook.md)):

- **Anthropic two-tier pattern**. Slim `/llms.txt` index file (under 10KB) → links to a much larger `/llms-full.txt` Markdown export. Lets retrieval tools pick context depth. Use for content-heavy sites.
- **Vercel use-case-mapped pattern**. Organize by entry points that map to common developer questions, not by sitemap. Multi-product orgs win by structuring around use cases.
- **Cloudflare product-modular pattern**. One section per product (Workers, R2, D1) so AI fetches only the relevant slice.

**Maintenance cadence:**
1. Update `/llms.txt` whenever positioning, pricing, or top-level navigation changes (typically quarterly).
2. Update `/llms-full.txt` continuously (automate via Mintlify-style build).
3. Audit monthly with `curl https://yoursite.com/llms.txt` to confirm plain-text serving (no HTML wrapper, no auth gate).
4. Check server logs monthly for AI-agent fetches: GPTBot, PerplexityBot, ClaudeBot, ChatGPT-User, Googlebot-Extended, Applebot-Extended.
5. Tie updates to the Vercel North Star: **% of new signups from ChatGPT/Claude/Perplexity referrals**.

#### Playbook B. Multi-platform AI visibility tracking with scraped data (the right setup)

**Why scraped, not API:** API sources cover only 24% of brand overlap and 4% of source overlap with what users see. Anyone tracking API-only is reporting on a different question than users actually ask.

**Recommended stack architecture:**
1. **Free/diagnostic layer:** [HubSpot AI Search Grader](https://www.hubspot.com/ai-search-grader) (GPT-5.2, Perplexity, Gemini cross-validated, free). Run quarterly for directional brand baseline.
2. **First-party publisher layer:** Bing Webmaster Tools "AI Performance", free, surfaces actual grounding queries. Treat grounding queries as a new keyword universe (Mahmoud's playbook documents a 75-organic-click site that accumulated 33,000+ AI citations by ranking for grounding-query language).
3. **Paid scraped tracking layer:** Pick one based on tier. AthenaHQ ($295/mo) for mid-market with execution; Peec AI (€89/mo) for European/multi-language; Profound ($399 Growth, $2K+ Enterprise) for enterprise + multi-engine + prompt-volume; Bluefish for Fortune 500 brand-safety.
4. **Validation layer:** Manual incognito audits of the top 20 buyer-intent prompts in ChatGPT (web), Perplexity (web), Claude (web), Gemini, Copilot, done weekly. The only way to catch what no tool catches.
5. **Cross-validate:** Compare Bing AI Performance grounding queries against your scraped tracking tool's prompt list, fill gaps where Bing surfaces queries you're not tracking.

### Cross-References to Mahmoud's `aeo-geo-playbook.md`

The OS doc and Mahmoud's existing AEO playbook complement each other. Use this routing:

**Already deeply covered in `aeo-geo-playbook.md`, link, don't duplicate:**
- Query fanout mechanics (2–5 sub-queries; 66% appear once; 84% share Google URLs)
- API vs. scraped data gap (24% brand / 4% source overlap)
- Top GEO ranking factors (brand associations > backlinks; YouTube; freshness; topical authority)
- ChatGPT/Perplexity/Claude platform-specific tactics (Reddit citation rates, Wikipedia weights, money-pages 5-6× strategy)
- Multi-platform source-preference table (per platform)
- 14-item Quick Wins Checklist
- `/llms.txt` and `/pricing.md` baseline templates
- Princeton GEO study citation-boost metrics (+40% citations / +37% statistics / +30% quotations)

**Net-new for this OS doc (the strategic measurement layer):**
- Conductor 2026 benchmarks methodology + numbers (13,770 domains; 1.08% AI referral baseline; 87.4% ChatGPT share; industry-level variance from 4.48% Real Estate to 48.75% Healthcare)
- Bing Webmaster Tools "AI Performance" launch (Feb 2026), first-party publisher dashboard
- Tool comparison table (Profound, AthenaHQ, Peec AI, Bluefish, SE Visible, HubSpot Grader) with pricing + tracking-method transparency
- Named case studies with before/after numbers (Ramp 7×, Rootly 10×, Grüns 23× citation rate, Popl 1,561% ROI, Vercel <1%→10% ChatGPT signups)
- "Athena-authored content" credibility caveat (vendor-published cases need external validation)
- Kevin Indig's 1.2M-response Jan 2026 analysis (44.2% of citations from first 30% of page text; "publication date + statistics" universal signal pair)
- Mike King "Relevance Engineering" framework (iPullRank, 661% ChatGPT visibility for a Fortune 500 client)
- Lily Ray's "AI Slop Loop" (hallucination → republication → RAG-citation feedback failure mode)
- Real-world `llms.txt` deployment patterns (Anthropic two-tier; Vercel use-case-mapped; Cloudflare product-modular) beyond the single-template baseline
- Vercel-style "% of new signups from ChatGPT" North Star metric

**Routing rule:** for tactical depth on query fanout, ranking factors, money-pages strategy, multi-platform source preferences, and the implementation checklist → load `aeo-geo-playbook.md`. For the strategic measurement layer (benchmarks, tool procurement, case-study evidence, cross-functional KPIs) → use this file.

### Resources for Deeper Study

**YouTube channels**
- **Aleyda Solis**, global SEO + AEO
- **Ahrefs**, practical SEO + emerging AEO
- **Semrush Academy**, broad SEO/AEO education
- **Authority Hacker** (Gael Breton, Mark Webster). AI search workflows
- **Lily Ray**. E-E-A-T and Google updates
- **Marie Haynes**. Google AI analysis
- **Surfer SEO**, content optimization education
- **Ross Simmonds (Foundation)**, distribution + AI search

**Podcasts**
- *Search Off the Record* (Google Search Central)
- *The Search Engine Journal Show*
- *SEO Office Hours* (Aleyda Solis)
- *The Authority Hacker Podcast*

**Substacks & Newsletters**
- Kevin Indig's "The Growth Memo"
- Aleyda Solis's "SEOFOMO"
- Lily Ray's updates
- Marie Haynes Newsletter
- Conductor research reports (2026 AEO/GEO benchmarks)

**Books / Guides**
- *Product-Led SEO* (Eli Schwartz)
- *The Art of SEO* (Enge, Spencer, Stricchiola), foundational
- [Princeton/GT/Allen Institute/IIT Delhi GEO paper (Aggarwal et al., 2023, accepted KDD 2024)](https://arxiv.org/abs/2311.09735), foundational academic work; demonstrates 40% visibility lift from optimization tactics
- [Conductor 2026 AEO/GEO Benchmarks Report](https://www.conductor.com/academy/aeo-geo-benchmarks-report/), 13,770 enterprise domains; 3.5M unique prompts; 17M AI responses; 100M+ citations
- [Mike King (iPullRank); "The AI Search Manual"](https://ipullrank.com/ai-search-manual). Relevance Engineering framework; 661% ChatGPT visibility case for a Fortune 500 client
- [Kevin Indig; "State of AI Search Optimization 2026"](https://www.growth-memo.com/p/state-of-ai-search-optimization-2026), 1.2M ChatGPT responses analyzed; 44.2% of LLM citations come from first 30% of page text
- [Foundation Inc. + G2; "Answer Economy Report"](https://foundationinc.co/lab/g2-answer-economy-report/), how AI Search is rewiring B2B software buying
- [Aleyda Solis; "The State of AI Search Optimization 2025"](https://hub.seofomo.co/surveys/state-ai-search-optimization/), three goal shifts: growth → resilience, clicks → presence, Google SEO → ecosystem optimization

**Primary research / studies**
- [Ahrefs (Mar 2026); "38% of AI Overview Citations Pull From The Top 10"](https://ahrefs.com/blog/ai-overview-citations-top-10/)
- [Ahrefs (Aug 2025); "Only 12% of AI Cited URLs Rank in Google's Top 10"](https://ahrefs.com/blog/ai-search-overlap/)
- [Profound × Reddit 10M Search Study](https://www.samhogan.sh/blog/profound-10m-search-study). Reddit = 3.11% of all AI citations
- [Lily Ray; "The AI Slop Loop"](https://lilyraynyc.substack.com/p/the-ai-slop-loop)
- [Ross Simmonds; "Visibility in LLMs"](https://rosssimmonds.com/blog/visibility-llms/), distribution opens the gates to LLM citations

---

## v3 (shipped Apr 2026)

- [x] V1 reconciled, 38% (Ahrefs Mar 2026) / 80% (Ahrefs Aug 2025) / Perplexity 28.6% with methodology footnote
- [x] Solis + Ray + King verbatim quotes (incl. Ray's 'AI Slop Loop')
- [x] 6 named cases (Ramp 7× via Profound, Rootly 10× via AthenaHQ, Grüns 23× citation rate, Popl 1,561% ROI, Vercel <1%→10% ChatGPT signups, Anthropic llms-full.txt pattern)
- [x] Profound vs. AthenaHQ vs. Peec AI vs. Bluefish AI vs. SE Visible vs. HubSpot AEO Grader comparison
- [x] Bing Webmaster Tools 'AI Performance' launch (Feb 10, 2026) integrated as first-party publisher layer
- [x] llms.txt deployment patterns (Anthropic two-tier / Vercel use-case-mapped / Cloudflare product-modular)
- [x] API-vs-scraped tracking warning embedded; 'Athena-authored content' caveat called out
- [x] Industry overlay (biopharma overlay especially sharp. PubMed/Wikipedia not ChatGPT) + cross-references (6 inter-domain + 2 skills)

## v4 deferred

- [ ] Mahmoud's own Space & Story SSR migration case, needs Mahmoud's first-party AI-traffic before/after data
- [ ] Wikipedia/Wikidata entity-presence case with documented LLM-citation lift (currently Anthropic via llms-full.txt is the proxy)
- [ ] Bing Webmaster Tools 'AI Performance' usage patterns at scale (let it mature 6 months)

See [research-plan.md](research-plan.md) for the master v3 changelog and v4 forward plan.
---

## Frequently Asked Questions — Domain 5: AI Search & Answer Visibility

### What is the difference between SEO, AEO, GEO, and LLMO?

SEO is Search Engine Optimization (the original, ranking pages in Google). AEO is Answer Engine Optimization (structuring content for direct answer extraction in featured snippets and AI overviews). GEO is Generative Engine Optimization (visibility within LLM responses from ChatGPT, Claude, Perplexity, Gemini). LLMO is LLM Optimization (broader than GEO; includes entity-level presence in training data). 'AI SEO' is the umbrella term.

### What percentage of AI Overview citations come from Google's top 10?

Only 38% as of March 2026, down from 76% in July 2025 (Ahrefs, n=863K SERPs). For non-Google LLMs (ChatGPT, Gemini, Copilot), the gap is wider: ~80% of citations come from pages that don't rank in Google's top 100 for the original prompt (Ahrefs, August 2025, n=15K queries). Perplexity is the exception (28.6% in top 10). The decline reflects Google's increased reliance on fan-out subqueries — ranking still matters, but the bar is fan-out coverage and topical authority, not single-keyword top-10 placement.

### Should I publish llms.txt?

Yes, especially for content-heavy or developer-tool sites. Three deployment patterns are emerging: Anthropic's two-tier (slim /llms.txt index → larger /llms-full.txt Markdown export), Vercel's use-case-mapped (organized around developer questions, not sitemap), and Cloudflare's product-modular (one section per product). Proof point: Vercel went from <1% → 10% of new signups from ChatGPT in 6 months after publishing llms-full.txt via Mintlify. The pattern has been adopted by Cursor, Coinbase, Pinecone, Windsurf, and Cloudflare.

### Which AI citation tracking tool should I use?

Profound for enterprise (Target, Walmart, Figma, MongoDB, Ramp; $399/mo Growth, $2K-5K+ Enterprise; multi-engine + prompt-volume tracking). AthenaHQ for mid-market needing tracking + content generation in one tool ($295/mo flat). Peec AI for European/multi-language (€89-199/mo). HubSpot AI Search Grader for free first-touch diagnostic. Critical warning: API-based tracking misses 96% of what users see — brand overlap between API and scraped UI responses is only 24% (per Mahmoud's aeo-geo-playbook.md). Tools using UI scraping: Peec AI, AthenaHQ, SE Visible. Profound is hybrid; Bluefish is opaque.

