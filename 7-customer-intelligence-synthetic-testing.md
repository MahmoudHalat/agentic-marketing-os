<!--
seo:
  title: Synthetic Testing & Digital Twins for Marketing Research — Domain 7
  description: Pre-launch validation, audience simulation, digital twins. CVS 100K agentic twins, Park 2024 (85% accuracy), Toubia Funhouse Mirrors critique, Wynter / Simile / PyMC Labs comparison.
  primary_keyword: synthetic market research
  secondary_keywords: [digital twins, synthetic personas, Wynter B2B, Simile, PyMC Labs, Park generative agents]
-->
## Domain 7: Customer Intelligence & Synthetic Testing

> **TL;DR.** Pre-launch validation, audience simulation, message testing — the newest standalone domain. **Anchor stat: 85% accuracy on the General Social Survey (Park et al. 2024) — NOT 94%** (the 94% is a widespread miscitation). **Critical counter-data: average twin-to-human correlation 0.197 in the Columbia "Funhouse Mirrors" mega-study (Toubia et al. 2025)** — synthetic narrows what to test, never decides. **Tools that win:** Wynter for live B2B (~$799+/mo), PyMC Labs for Bayesian rigor, Custom Claude Project for first-party-data personas, Simile / Aaru / Evidenza for enterprise. **Canonical case: CVS Health × Simile** — 2.9M consented responses → 100K+ "agentic twins" with explicit "doesn't replace real-world research" governance. **What changed in v3:** corrected the 85% (not 94%) Park stat, added Funhouse Mirrors critique with 0.197 correlation, added 5 named cases (CVS, EY×Evidenza 95%, Aaru NY primary, PandaDoc×Wynter, PyMC validation), pure-play vs. embedded vs. B2B-specific tooling comparison.

> *"It's the struggling moment where they can't do something that causes them to take the leap."* — Bob Moesta, [Inside Intercom podcast](https://www.intercom.com/blog/podcasts/bob-moesta-on-unpacking-customer-motivations-with-jobs-to-be-done/), May 17, 2018

> *"People buy things to help them make progress."* — Bob Moesta, same Intercom interview

**See also:** Mahmoud's [`customer-research-playbook`](skill) for interview craft and JTBD methodology, Mahmoud's [`competitor-research-playbook`](skill) for synthetic competitor-persona patterns, [Domain 1 (Sensing)](1-sensing-intelligence.md) for sales-call mining as Domain 7 fuel, [Domain 2 (Strategy)](2-strategy-positioning.md) for synthetic + Wynter sequencing on positioning shifts, [Domain 3 (Content)](3-content-creative-production.md) for customer-language vector store, [Domain 8 (Measurement)](8-measurement-attribution.md) for synthetic-to-live correlation as continuous KPI, [Domain 0 (AgentOps)](0-agentops.md) for governance on synthetic outputs in regulated industries.

### Definition and Scope

Pre-launch validation, audience simulation, message testing, customer behavior modeling. The newest standalone domain, qualitatively new work that wasn't possible at this scale or speed before generative AI.

Owns: synthetic personas (AI-generated audience profiles for concept testing), digital twins of customers (continuously evolving models), synthetic panels (large-scale simulated audiences for survey-style research), message testing pre-launch, packaging and pricing simulation, and the validation infrastructure that determines what you ship vs. what dies in a draft folder.

### Why It Matters Now

McKinsey estimates agentic AI could support up to two-thirds of current marketing activities, including synthetic audience testing. The technology has attracted **over $1B in disclosed venture capital across 2023–2026**, with confirmed major rounds: [Simile $100M Series A (Feb 2026, Index Ventures + Bain Capital + A* + angels Fei-Fei Li and Andrej Karpathy)](https://www.indexventures.com/perspectives/life-the-universe-and-simile-leading-similes-series-a/); [Aaru ~$50M+ Series A at $1B headline (Dec 2025, Redpoint)](https://techcrunch.com/2025/12/05/ai-synthetic-research-startup-aaru-raised-a-series-a-at-a-1b-headline-valuation/), though Aaru's ARR is still <$10M; Listen Labs $69M (2025), Outset $17M Series A (8VC), Keplar $3.4M (Kleiner Perkins, 2025).

Real evidence of capability:
- [Park et al. (2024) "Generative Agent Simulations of 1,000 People"](https://arxiv.org/abs/2411.10109): n=1,052 participants; two-hour AI interviews; agents replicated participants' GSS responses **85%** as accurately as participants replicated their own answers two weeks later. Combined interview + survey agents reached **86%** vs. demographic-only at **74%**. Reduced racial/ideological bias by 36–62%. *(The frequently cited "94% accuracy" figure is a miscitation, the Park paper number is 85%.)*
- [Toubia et al. (2025) "Twin-2K-500"](https://arxiv.org/abs/2505.17479), 2,058 US participants, 500+ questions across 4 waves; reference dataset for digital-twin validation.
- [Toubia et al. (2025) "Digital Twins are Funhouse Mirrors: Five Systematic Distortions"](https://arxiv.org/abs/2509.19088) (Columbia, Wharton), current state-of-the-art critique. Average twin-to-human correlation **0.197** (≈ height vs. intelligence). Twin standard deviation lower than human in **93.9%** of cases.
- Booking.com used Qualtrics Edge Audiences to drill down on hard-to-reach subgroups in Travel Trends study without expanding human panel. Qualtrics positions this as "around 50% cost reductions vs. human-only panels." Treat as vendor-told, directional.

But the field is real and the cautions are real. The canonical critique: [Conjointly / Nik Samoylov; "Synthetic Respondents Are the Homeopathy of Market Research"](https://conjointly.com/blog/synthetic-respondents-are-the-homeopathy-of-market-research/), income variance $111,348 → $272,014 from prompt rephrasing alone. [NN/G (Nielsen Norman Group)](https://www.nngroup.com/articles/synthetic-users/) is the most-cited UX-research authority's stance: "synthetic users help with hypothesis generation, not validation." The truth is in the middle: synthetic is a useful pre-test layer for narrowing concepts before live validation. **Not a substitute for talking to real customers.**

### Sub-Domains

**7.1 Synthetic Persona Generation**
- Building AI personas from first-party data (CRM, surveys, customer interviews)
- Demographic and psychographic modeling
- Behavioral profile construction
- Scenario testing (how does a persona react under different conditions?)

**7.2 Concept & Message Testing**
- Pre-launch concept validation
- Headline / value-prop A/B testing against synthetic audiences
- Pricing point sensitivity
- Packaging and bundling concepts
- Ad creative pre-testing

**7.3 Digital Twin Modeling**
- Continuously evolving models trained on individual customer data
- Personalization at scale
- Behavioral prediction
- Customer experience simulation

**7.4 Synthetic Panels & Survey-Style Research**
- Large-scale simulated audiences (n=1,000–5,000+)
- Demographic-representative sampling
- Market-segment analysis
- Niche audience exploration (where real recruiting is hard)

**7.5 Validation Infrastructure**
- Calibration against real customer data
- Bias detection and correction
- Methodology documentation (transparency requirements)
- Hand-off to live research for high-stakes decisions

**7.6 Customer Voice Capture**
- Interview transcript synthesis
- Review mining for verbatim language
- Sales call analysis (Domain 1 overlap)
- Support ticket pattern recognition

### Best Practices in 2026

**Use synthetic audiences as a front-end filter, not a finish line.** They are excellent at producing testable hypotheses, useful for narrowing 20 concepts to 3 before live testing. They are not validated truth. The strongest teams use synthetic + live in sequence, not as substitutes.

**Build personas on real data, not imagination.** "Garbage in, garbage out" applies aggressively. Reliable persona generation starts with first-party data: customer interviews, CRM patterns, support logs, social listening, behavioral data. Personas built only from public data (and an LLM's training) reflect the LLM's bias, typically toward younger, more educated, more liberal demographics.

**Validate before consequential use.** For regulated sectors (healthcare, finance, products involving minors), synthetic persona output should never be the sole basis for messaging or product decisions. Human review, legal review, and live research remain critical.

**Calibrate continuously.** A synthetic persona is a model. Models drift. Compare synthetic predictions to real customer behavior on every campaign or product launch, then adjust. This is the difference between "homeopathy" and rigorous applied research.

**Document the inputs.** When a team says "the persona predicts strong adoption," they should also explain why, based on what inputs, and with what limitations. Transparency is essential for trust.

**Use synthetic for breadth; use live for depth.** Synthetic panels are unmatched for testing many variations quickly (50 ad creatives in a day). Live research remains unmatched for understanding the why behind reactions, cultural nuance, and tacit knowledge.

### Tools & Platforms

**Pure-Play Synthetic Research Platforms**
- **Simile** ($100M from Index Ventures, Feb 2026). Founded by Stanford's Joon Sung Park (inventor of generative agents), Michael Bernstein, Percy Liang. The deepest pedigree in the space.
- **Aaru**, synthetic audiences with a focus on consumer behavior
- **Ditto** (askditto.io), research platform with extensive market mapping
- **Evidenza**, synthetic research for B2B
- **SYMAR**, synthetic market research
- **Synthetic Users**. UX-research-focused
- **Ask Rally**, virtual focus groups, GenPop panel calibrated on real interviews
- **Delve AI**, persona generation + digital twin chat

**Embedded in Survey Platforms**
- **Qualtrics Edge Audiences**, synthetic respondents in the world's largest survey platform; fine-tuned on 25+ years of Qualtrics research data
- **Toluna HarmonAIze**, synthetic respondents from 79M-member panel data
- **YouGov (via Yabble acquisition)**. AI-augmented insights

**Hybrid AI + Human Panels**
- **Quantilope**. AI for analysis and survey design, human respondents
- **Remesh**. AI moderation, real participants
- **Conjointly**, pricing and feature research

**B2B-Specific**
- **Wynter**, message testing with verified B2B audience pools (~$299–$1,000+/mo)
- **PyMC Labs**. Bayesian-modeled synthetic consumers; Fortune 500 deployments

**Custom Builds**
- **Anthropic Claude / OpenAI GPT** with custom system prompts + structured persona docs
- **Retell AI / Vapi**, voice-based synthetic interviews

### Notable Practitioners & Frameworks

- **Joon Sung Park (Stanford, now Simile)**. Pioneer of generative agents. The Park et al. 2024 paper (1,000 People) is the foundational reference.
- **Michael Bernstein, Percy Liang (Stanford)**. Co-architects of generative agents.
- **PyMC Labs team**. Bayesian methodology. ["LLMs Reproduce Human Purchase Intent" (2025)](https://www.pymc-labs.com/blog-posts/AI-based-Customer-Research). Semantic Similarity Rating method; 57 surveys, 9,300 human responses (Colgate-Palmolive collaborators); 90% correlation on product ranking, 85%+ distributional similarity.
- **Bob Moesta**. JTBD (real-customer-research; informs synthetic).
- **Indi Young**. Listening as a research practice (the "why" that synthetic can't fully replicate).
- **Olivier Toubia (Columbia)**. Lead author on Twin-2K-500 + Funhouse Mirrors; the academic counter-weight to vendor claims.
- **Ray Poynter (NewMR)**, practitioner-side critic on synthetic-data limits.

### Named Case Studies

| Case | What they did | Result | Notes |
|---|---|---|---|
| **CVS Health × Simile** | Built generative agents on **2.9M consented responses from 400,000+ participants across 200+ behavioral scenarios**. Operates **100,000+ "agentic twins"** | Use case: medication adherence drivers — twins surfaced trust/confidence/convenience as primary; barriers as confusion/refill anxiety/prior frustration | Critical caveat from CVS's own announcement: *"simulations don't replace real-world research"* — they prioritize what to test. Governance monitors tone, fairness, safety. Strongest consumer-healthcare example |
| **EY × Evidenza** | C-suite executive research; "Synthetic CMO" feature with Sharp/Ritson/Binet/Field clones | EY CMO Toni Clayton-Hine reported **95% correlation** with EY's actual Global Brand Survey of C-suite execs. Confirmed clients: BlackRock, Microsoft, JP Morgan, Salesforce, Dentsu, ServiceNow | Self-reported correlations not externally audited; pricing ~$50K–$100K/yr |
| **Aaru — 2024 NY Democratic primary** | ~5,000 AI agents predicting election | Within **<400 votes** of actual at ~1/10 the cost of traditional polls | Strongest *prediction-validation* in public record; weakest is one-off election results don't prove repeatable methodology (Nate Silver's team published critical "AI polls are fake polls" piece) |
| **Park 1,000 People + NN/G three-study evaluation (calibration)** | Where synthetic & real agreed: directional preferences, demographic patterns, personality dimensions (Big Five 0.80) | Where they diverged: behavioral data (online courses — synthetic claimed completion when real users hadn't), drone delivery (synthetic favorable, real users impractical), dog-food purchase intent (synthetic SD lower than human; magnitude off) | Twin-to-human correlation averaged **0.197** in Columbia mega-study |
| **PandaDoc × Wynter** (the anti-synthetic control) | 50-person verified B2B marketing panel on PandaDoc messaging | Found "on-brand docs" was confusing/generic for the ICP — *live human* responses caught what synthetic might have missed | 12–48 hour turnaround |
| **Regulated-industry limit** | No FDA regulation specifically governs synthetic personas. CVS's pattern (never sole-basis decision-making, governance layer) is the de facto regulated-industry playbook | Pharma firms using synthetic for HCP message testing keep human IRB-approved validation pass on every consequential decision | FDA's 2024 draft guidance on AI in drug development is silent on synthetic respondents |

### Tools & Platforms, head-to-head

#### Pure-play synthetic platforms

| Platform | Pedigree | Pricing | Best fit | Watch for |
|---|---|---|---|---|
| **Simile** | Stanford founders (Park/Bernstein/Liang); $100M Index | Enterprise (undisclosed) | Fortune 100 longitudinal twins; CVS-style 100K-agent deployments | Newest; bandwidth limited to large accounts |
| **Aaru** | Teen-founder team; $1B headline; Redpoint | Enterprise | Election-style large-N consumer simulations; corporate executive simulations (Lumen) | <$10M ARR; valuation ahead of revenue |
| **Ditto / FishDog** | 300K pre-built population-true personas | $50K–$75K/yr unlimited | Self-serve consumer brand testing; Figma/Canva/Framer integrations | Now FishDog after rename |
| **Synthetic Users** | Kwame Ferreira; UX focus | $2–$27 per interview, +$5 RAG | UX hypothesis generation; pre-research scoping | NN/G explicitly cautions against using as research replacement |
| **Evidenza** | Lombardo + Weinberg ex-LinkedIn B2B Institute | ~$50K–$100K/yr | B2B CMO-level brand strategy; "Synthetic CMO" feature | No self-serve, no API, 72-hour turnaround |
| **Ask Rally** | Calibrated GenPop panel via Turing test | Mid-market | Rapid small-to-medium decision testing | Calibration is per-persona; uneven coverage |

#### Embedded-in-platform

| Platform | Approach | Source pool |
|---|---|---|
| **Qualtrics Edge Audiences** | Fine-tuned proprietary LLM on 25+ yrs of Qualtrics studies | Booking.com, Dollar Shave Club, Gabb |
| **Toluna HarmonAIze** | Each persona = individual synthetic respondent (not segment average) | 19.4M-member US panel (now expanding UK/FR) |
| **YouGov (via Yabble)** | AI insight layer on existing panel | YouGov panel |

#### B2B-specific

| Platform | Method | Numbers |
|---|---|---|
| **Wynter** | Verified human B2B panel (saturation methodology, 12–13 responses) | 70K–80K verified B2B professionals; LinkedIn + corporate-email verified; from $798/mo, 12–48hr |
| **PyMC Labs** | Bayesian-modeled synthetic + Semantic Similarity Rating | Custom; 90% product-ranking correlation, 85%+ distributional similarity |

**Decision frame:** **Wynter** when you need real B2B humans on your ICP for high-stakes message/positioning/pricing decisions. **PyMC Labs** when you need scientifically grounded synthetic at scale and can invest in custom Bayesian validation. **Evidenza** when buying committee is C-suite Fortune 500 and you can absorb $50K+ engagements.

#### Critical distinction: AI-interview hybrid ≠ synthetic

[Listen Labs ($69M Sequoia)](https://venturebeat.com/technology/listen-labs-raises-usd69m-after-viral-billboard-hiring-stunt-to-scale-ai), Outset ($17M 8VC), Keplar ($3.4M Kleiner Perkins) all use AI to interview *real humans* at scale. These are **NOT synthetic**, they are AI-moderated qualitative. The distinction is often lost in press coverage.

### Tactical Playbooks

#### Playbook A. Synthetic persona from first-party data (Claude Project build)

1. Export to Markdown: 30 customer interview transcripts + last 90 days of support tickets + last 200 sales-call transcripts (Gong/Fireflies) + open-ended NPS verbatims.
2. Cluster by JTBD using Claude (3–5 distinct jobs).
3. For each job, build a Claude Project with: ICP firmographics, top-3 quotes per pain dimension, top-3 trigger events, observed-language vocabulary list, list of objections actually voiced (verbatim).
4. **System prompt:** *"You are [Persona]. Answer ONLY using language and frames from the provided transcripts. If asked something outside these transcripts, say 'I don't know' rather than inventing."* (Explicitly defends against the sycophancy problem NN/G flagged.)
5. **Validate quarterly:** pose the same 5 questions to 3 real customers and compare. If correlation drops, refresh the corpus.

**Cross-link:** This is the bridge between Mahmoud's [`customer-research-playbook`](skill) (real interviews) and synthetic, the playbook produces the inputs; the Project produces the simulator.

#### Playbook B, 50 ad creatives in a day, narrowed to 3

- Generate 50 ad-creative variations (Claude or Midjourney); store in spreadsheet
- Run synthetic panel on Ditto/Ask Rally for each variant: predicted CTR rank, recall rank, brand-fit rank
- Filter to top 10 (kill bottom 80% on synthetic alone; *"front-end filter, not finish line"*)
- Expert review (PMM + creative director) prunes 10 → 5
- Live test 5 on Wynter (B2B) or Meta CBO-test (B2C)
- Final 2–3 get media spend

**Why this works:** synthetic is high-recall low-precision; live is low-recall high-precision. The funnel respects each layer's strengths.

#### Playbook C. Synthetic + live in sequence

- **Discover (live):** 12–15 customer interviews. Bob Moesta switch interviews, Indi Young listening sessions
- **Hypothesize (synthetic):** Translate findings into 5–10 testable concepts; run on synthetic panel for directional ranking
- **Validate (live):** Top 2–3 concepts go to Wynter / focus groups / live A/B
- **Calibrate (continuous):** After every launch, compare synthetic prediction vs. live result; track synthetic-to-live correlation as a KPI. **If it decays past 0.7, the persona corpus is stale.**

### Cross-References to Mahmoud's Skills

- **`customer-research-playbook`** owns interview craft, JTBD, switch interviews, listening, mental models. **Domain 7 does not duplicate any of that.** Domain 7 picks up where the playbook ends, when you have 30 real interviews, what synthetic layer should you build, and where does it break?
- Domain 1 (Sensing) overlap, sales-call mining is a Domain 1 input that becomes Domain 7 fuel.
- Domain 8 (Measurement) overlap, synthetic-to-live correlation IS the measurement metric for Domain 7.

### Industry overlay (Q2 2026)

| Industry | ICP / motion difference | Tools that win | Biggest pitfall | Compliance overlay |
|---|---|---|---|---|
| **B2B SaaS** | Synthetic personas built on Gong + Zendesk + interview corpus; Wynter for B2B panel validation; calibrate quarterly | Wynter ($799+/mo verified B2B); PyMC Labs for Bayesian rigor; Claude Project personas from first-party data; Synthetic Users for UX | Treating synthetic as truth — Park 1,000 People shows 85% replication ceiling, Toubia "Funhouse Mirrors" finds 0.197 average correlation. **Front-end filter only** | None |
| **Biopharma** | Synthetic HCP/patient personas are **advisory only** — never substitute for IRB-approved research. CVS × Simile is the published pattern. EY × Evidenza for C-suite | Simile (Stanford pedigree, $100M Index); Evidenza (~$50-100K, "Synthetic CMO" with KOL clones); **real KOL advisory boards (gold standard)**; patient panels via Rare Patient Voice/Carenity | Using synthetic patient response to drive a label change, MoA messaging, or clinical claim — regulator views it as inadequate basis; payer tie-in falls apart | FDA Mar 2026 NAM draft guidance allows digital twins in trials; IRB review on patient-facing tests; HIPAA on synthetic patient cohorts built from real PHI; ABPI/PhRMA Code on HCP simulation |
| **DTC** | Synthetic ad pre-test → 50 creatives → 10 → 5 → live Meta CBO; concept ranking before media spend | Ditto/FishDog (300K personas, $50-75K/yr); Ask Rally; Suzy for human panel; Meta Advantage+ Lift Studies for live | Trusting synthetic CTR predictions and running media — DTC results vs. synthetic correlation breaks at scale; always live-test top-3 | FTC truth-in-advertising on testing claims if marketed externally |
| **Dev tools** | Synthetic developers are weakest area — LLMs can't simulate "I tried it, the SDK threw an error." Real DX testing on Discord/beta lists wins | Real beta programs; UserTesting.com with engineer-screen; Maze for unmoderated dev research; Synthetic Users only for hypothesis generation | Using synthetic devs to validate API ergonomics — they say what reads well, not what compiles. Will mislead DX decisions | None beyond standard |

**Key insight:** Biopharma's synthetic-testing posture is uniquely **advisory only**. CVS Health's own framing is that 100K-twin simulations *prioritize what to test next*, never replace IRB-approved research. Any synthetic output that informs a clinical claim, label, or HCP message must pass through human medical review. This is the single sharpest compliance overlay across all 8 domains.

### Common Failure Modes

- **Treating synthetic as truth.** Synthetic outputs are plausible-sounding by design; that doesn't make them right.
- **Bias amplification.** LLMs underrepresent older, more conservative, less-educated demographics. Synthetic panels built on default LLM behavior reproduce this bias.
- **Skipping real-customer validation for high-stakes decisions.** Pricing, positioning shifts, and product launches need real-world confirmation, not just synthetic confidence.
- **Static personas.** Audiences change. A persona built in 2024 may be wrong in 2026. Refresh the underlying data.
- **Conflating synthetic personas with digital twins.** Personas are abstract; digital twins are individual. Different tools for different jobs.

### KPIs

- **Concept hit rate** (% of concepts that pass synthetic + advance to live testing)
- **Synthetic-to-live correlation** (how often does synthetic prediction match live results?)
- **Time-to-validated-concept** (synthetic compresses this dramatically)
- **Cost-per-validated-concept** (synthetic should be 10x+ cheaper than traditional)
- **Concept abandonment rate before media spend** (synthetic should kill more bad ideas, sooner)

### Resources for Deeper Study

**YouTube channels**
- **PyMC Labs**, methodological depth
- **Stanford HAI**, academic foundation
- **NN/g (Nielsen Norman Group)**. UX research foundations
- **Marketing Science Institute**, academic marketing research

**Podcasts**
- *Marketing Today with Alan Hart*
- *The Bob Moesta Show* (Jobs-to-be-Done)
- *Indi Young's Listening podcast*

**Books**
- *Demand-Side Sales 101* (Bob Moesta)
- *When Coffee and Kale Compete* (Alan Klement)
- *Practical Empathy* (Indi Young)
- *Interviewing Users* (Steve Portigal)

**Foundational Papers**
- Park et al. (2023), "Generative Agents: Interactive Simulacra of Human Behavior". Stanford foundational paper
- More recent papers on synthetic respondent calibration and validation

---

## v3 (shipped Apr 2026)

- [x] Park 85% accuracy correction (was miscited as 94%)
- [x] Toubia 'Funhouse Mirrors' critique (0.197 average twin-to-human correlation, 93.9% twin-SD-lower-than-human)
- [x] 5 named cases (CVS Health × Simile 100K twins, EY × Evidenza 95% correlation, Aaru NY primary <400 votes, PandaDoc × Wynter live caught what synthetic missed, PyMC Labs 90%/85% validation)
- [x] Pure-play vs. embedded vs. B2B-specific tooling comparison (Simile / Aaru / Ditto / Synthetic Users / Evidenza / Qualtrics Edge / Wynter / PyMC)
- [x] AI-interview-hybrid distinction explicitly called out (Listen Labs / Outset / Keplar are NOT synthetic)
- [x] Moesta verbatim quotes (incl. 'It's the struggling moment where they can't do something that causes them to take the leap')
- [x] $1B+ disclosed VC across 2023-2026 reframed (was '$1.5B' without sourcing)
- [x] 3 tactical playbooks (synthetic persona from first-party data, 50→3 ad creatives, synthetic+live in sequence)
- [x] Industry overlay (biopharma 'advisory only' framing especially sharp) + cross-references (5 inter-domain + 2 skills)

## v4 deferred

- [ ] Continuous-calibration methodology (synthetic-to-live correlation tracking as a continuous KPI) with a named-brand case
- [ ] First regulated-industry public failure case to clarify boundaries (FDA/SEC enforcement action)

See [research-plan.md](research-plan.md) for the master v3 changelog and v4 forward plan.
---

## Frequently Asked Questions — Domain 7: Customer Intelligence & Synthetic Testing

### What's the actual accuracy of synthetic personas?

Park et al. (2024) Generative Agent Simulations of 1,000 People: agents replicated participants' GSS responses **85%** as accurately as participants replicated their own answers two weeks later. NOT 94% — the 94% figure widely cited online is a miscitation. Combined interview + survey agents reached 86% vs. demographic-only at 74%. Counter-data: Toubia et al. (2025) 'Funhouse Mirrors' found average twin-to-human correlation of 0.197 (≈ height vs. intelligence) and twin standard deviation lower than human in 93.9% of cases. Synthetic narrows what to test; it doesn't decide.

### Synthetic personas vs. live B2B panels — which wins?

Sequence them. Synthetic (Custom Claude Project, Synthetic Users, Ask Rally) for hypothesis generation and rapid concept screening — narrow 50 ad creatives to 3 in a day. Live B2B panels (Wynter, $799+/mo, 70K-80K verified B2B professionals) for validation before consequential decisions. PyMC Labs offers Bayesian-grounded synthetic with documented validation (90% correlation on product ranking, 85%+ distributional similarity across 57 surveys, 9,300 human responses). NN/G's stance: 'synthetic users help with hypothesis generation, not validation.'

### How does CVS Health use 100,000 synthetic twins?

CVS built generative agents on **2.9M consented responses from 400,000+ participants across 200+ behavioral scenarios** (announced 2025). Operates 100,000+ 'agentic twins' for journey-friction analysis, hard-to-reach population testing, and product testing at speed. Critical caveat from CVS's own announcement: *simulations don't replace real-world research.* Governance monitors tone, fairness, safety. This is the canonical regulated-industry pattern: synthetic prioritizes what to test next, never the sole basis for clinical or messaging decisions.

### Are AI-interview platforms (Listen Labs, Outset) the same as synthetic research?

No. Listen Labs ($69M Sequoia, 2025), Outset ($17M 8VC), and Keplar ($3.4M Kleiner Perkins) use AI to interview *real humans* at scale. They are AI-moderated qualitative research, not synthetic respondents. The distinction matters and is often lost in press coverage: AI-interview hybrids interview humans; synthetic research generates plausible responses without humans. Different tools for different jobs.

