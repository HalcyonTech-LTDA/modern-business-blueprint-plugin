# The Institutional Company Conception Document Standard

This standard defines the mandatory schema, structure, and quality standards for all company conception blueprints produced within the Modern Business Blueprint ecosystem.

As enforced by the **Lead Integrator**, every finalized blueprint must be synthesized into a single, cohesive, publication-grade document following formal business manifesto conventions.

---

## 1. Structural Schema Mandate

All generated conception documents MUST follow this exact Markdown header hierarchy:

```markdown
# [COMPANY NAME]: [CATEGORY MONIKER]
*Executive Conception Blueprint & Economic Architecture*

## I. THE CENTRAL THESIS
[The contemporary business problem, macroeconomic/regulatory inflection, and structural incumbent failure]

## II. THE ENTERPRISE
[The proprietary solution and exact value chain flow: DATA -> SIGNAL -> CONTEXT -> DECISION -> ACTION -> EVIDENCE -> LEARNING -> IMPROVEMENT -> LOOP]

## III. CATEGORY DESIGN & ANTI-POSITIONING
[The rejection of generic labels, definition of the ownable category, and the IS vs IS NOT Boundary Matrix]

## IV. MONETIZATION & ECONOMIC ARCHITECTURE
[The multi-layered revenue model: Base Platform + Entity Surveillance + Usage + Derived Data]
[Unit economics math: CAC, LTV, Payback Period, Gross Margins, and NRR targets]

## V. MOAT & DEFENSIBILITY MATRIX
[The four non-feature defensibility pillars: Switching Costs, Network Effects, Derived Data, Accumulated History]

## VI. TECHNICAL ARCHITECTURE, CYBERSECURITY & CORPORATE GOVERNANCE
[Event-driven architecture respecting physical data limits, Dev/Staging/Prod GitOps isolation, vendor portability, cybersecurity moat (AES-256, TLS 1.3, KMS, SOC 2/ISO 27001 readiness), 100% IP ownership, early-stage contract suite (SaaS MSA, DPA, SLA, NDA), and lean corporate governance (prohibition of premature boards, 60-min monthly executive cadence, and mandatory SHA terms)]

## VII. PRODUCT ROADMAP & GO-TO-MARKET EXECUTION PLAN
[Beachhead entry market, Trojan Horse MVP wedge, Land-and-Expand 4-horizon roadmap with Rule 3 horizontal core invariant, enterprise GTM engine with authority marketing, and 5-stage MEDDPICC sales funnel with replicable 30-day CS onboarding]

## VIII. CAPITAL ALLOCATION & EXECUTION MILESTONES
[Financial Model & P&L Structure separating software revenue from data consumption costs, Core KPIs Scorecard (MRR, ARR, NRR, Gross Margin, CAC, Payback, Cloud/Data Cost), Funding Strategy across 4 risk-reduction gates with 12-18 months runway per stage, Institutional Investment Thesis across 5 defensibility pillars, and Pragmatic 18-Month Execution Roadmap (Foundation -> Build -> Validation -> Commercialization -> Scale Decision)]
```

---

## 2. Lead Integrator Output Rules

The Lead Integrator enforces three non-negotiable Output Rules:

### Rule 1 (Synthesis) — Single Cohesive Executive Markdown Document
- The output MUST NOT contain disjointed agent chat transcripts, agent handoff notes, or dialogue fragments.
- All contributions from the Business Strategist Agent, Product & GTM Lead Agent, Corporate Architect Agent, and Finance & Venture Agent must be synthesized into a single, cohesive, publication-ready executive document (`MasterConceptionBlueprint.md`).
- Vocabulary, metrics, pricing tiers, and account definitions must be fully harmonized across sections.

### Rule 2 (Formatting) — Numbered Chronological & Strategic Business Manifesto Flow
- The document must be structured using Roman numerals (`I` through `VIII`) reflecting the logical progression of an institutional corporate manifesto:
  - From macro problem (`I. THE CENTRAL THESIS` / `A TESE CENTRAL`) to proprietary solution (`II. THE ENTERPRISE` / `A EMPRESA`), market category (`III`), monetization (`IV`), moats (`V`), infrastructure/legal foundation (`VI`), commercial GTM (`VII`), and capital allocation/execution milestones (`VIII`).

### Rule 3 (Tone Consistency) — Strict Executive Candor Across All Sections
- Startup clichés, optimistic exaggerations, and marketing fluff are strictly banned across all sections.
- The voice must maintain the analytical rigor and cold commercial objectivity of an institutional managing partner evaluating cash flow timing, customer acquisition friction, sales cycles, buyer budget authority, gross margins, and compute COGS.

---

## 3. Content Standards by Section

### Section I: A TESE CENTRAL
- Must describe the real-world operational friction in cold, commercial terms.
- Must identify the specific macro catalyst (regulatory change, technological inflection, cost structure collapse).
- Must avoid generic statements like "the world is moving fast" or "data is growing exponentially".

### Section II: A EMPRESA
- Must state the company's identity in a single, unyielding sentence.
- Must feature an explicit directional arrow flow:
  $$\mathbf{DATA} \longrightarrow \mathbf{SIGNAL} \longrightarrow \mathbf{CONTEXT} \longrightarrow \mathbf{DECISION}$$
- Must explain the exact transformation that occurs at each node of the flow.

### Section III: CATEGORY DESIGN & ANTI-POSITIONING
- Must contrast the new category against at least two generic labels.
- Must provide a detailed Markdown table with at least 5 distinct dimensions comparing "What the Company IS" versus "What the Company IS NOT".

### Section IV: MONETIZATION & ECONOMIC ARCHITECTURE
- Must delineate all four layers of the revenue model with dollar/percentage figures.
- Must include a complete quantitative unit economics model with calculated Payback (months) and LTV/CAC ratio.
- Must provide the line-item COGS breakdown and the 3-year gross margin expansion roadmap.

### Section V: MOAT & DEFENSIBILITY MATRIX
- Must address all four non-feature defensibility pillars.
- Must explicitly demonstrate how time and transaction volume increase customer switching costs.

### Section VI: TECHNICAL ARCHITECTURE, CYBERSECURITY & CORPORATE GOVERNANCE
- Governed by the **Corporate Architect Agent** (`corporate-architect-agent`):
  - Must design scalable event-driven architecture that respects physical limits of upstream data sources (streaming vs polling vs batch).
  - Must enforce Dev/Staging/Prod environment isolation, GitOps promotion gates, and structural vendor independence (**Rule 3: Constraint**).
  - Must embed cybersecurity controls (AES-256-GCM, TLS 1.3, KMS envelope encryption, IAM least-privilege) and establish SOC 2 Type II / ISO 27001 readiness as an active commercial sales asset.
  - Must mandate 100% corporate IP ownership, present assignment covenants, and contractor repository custody (**Rule 3: Constraint**).
  - Must define the essential early-stage contract suite: Enterprise SaaS MSA (12-mo liability cap), DPA, 99.9% uptime SLA, and mutual NDA.
  - Must enforce **Rule 1 (Governance)**: Strictly prohibit premature ornamental boards of directors, establish a 60-minute monthly executive decision cadence, and detail mandatory Shareholders' Agreement terms (4-yr vesting, good/bad leaver, drag/tag rights, non-compete).

### Section VII: PRODUCT ROADMAP & GO-TO-MARKET EXECUTION PLAN
- Governed by the **Product & GTM Lead Agent** (`product-gtm-lead-agent`):
  - Must define the optimal Beachhead Market based on urgent pragmatic criteria (regulatory pressure, cost of error $> \$1\text{M}$, budget ownership).
  - Must architect the Trojan Horse MVP Wedge solving an acute critical-path pain with a stream interception hook that secures data gravity.
  - Must map the 4-horizon Land-and-Expand Product Roadmap (Wedge $\rightarrow$ Adjacent Modules $\rightarrow$ Horizontal Platform OS $\rightarrow$ Vertical Migration) driving $\ge 120\% - 130\%$ NRR.
  - Must enforce **Rule 3 (Constraint)**: Strictly separate the immutable horizontal core engine from domain-specific declarative configuration schemas, banning bespoke client software development.
  - Must architect the high-ticket Enterprise GTM Engine: Founder-Led sales motion, Named Account Strategy, and Authority Marketing strictly positioned as **Credibility $\rightarrow$ Education $\rightarrow$ Demand**.
  - Must establish the 5-Stage Enterprise Sales Funnel governed by binary exit criteria and MEDDPICC deal qualification.
  - Must define the Replicable 30-Day Time-to-Value Customer Success onboarding process, strictly banning custom integration consulting.

### Section VIII: CAPITAL ALLOCATION & EXECUTION MILESTONES
- Governed by the **Finance & Venture Agent** (`finance-venture-agent`), enforcing strict P&L software segregation, 4-gate staged capitalization, institutional investment underwriting, and 18-month execution milestones:
  - *Financial Model & P&L Structure*: Strictly separates software ARR from third-party data pass-through fees and hosting COGS to prove software gross margins ($\ge 80\%$) vs data reselling.
  - *Core KPIs Scorecard*: Explicit mathematical targets for MRR, ARR, NRR ($\ge 120\% - 130\%$), Blended Gross Margin ($\ge 75\% - 85\%$), CAC, CAC Payback ($\le 12\text{ months}$), LTV/CAC ($\ge 3.0\times - 5.0\times$), and Cloud/Data Cost per Revenue ($\le 15\% - 20\%$).
  - *Funding Strategy (The 4 Gates)*: Milestone-driven capitalization funding Gates 1-4 (Build, Validation, Commercialization, Scale) with 12 to 18 months of operating runway per stage to prevent emergency cash calls.
  - *Institutional Investment Thesis*: Formulates the 5 pillars of venture equity value (recurring revenue, land-and-expand, high switching costs, software scale economies, and proprietary derived data accumulation).
  - *Pragmatic 18-Month Execution Roadmap (Rule 3 Action Plan)*: Concrete 5-phase timeline: Month 0-2 (Foundation), Months 2-5 (Build), Months 5-8 (Validation), Months 8-12 (Commercialization), and Months 12-18 (Scale Decision).
