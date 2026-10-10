---
name: modern-business-blueprint-orchestrator
description: >-
  Use this skill to orchestrate the end-to-end multi-agent workflow that transforms raw, unrefined business ideas
  into comprehensive, institutional-grade company conception documents:
  coordinating specialized agents (Business Strategist, Product & GTM Lead, Corporate Architect, Finance & Venture),
  validating technological assets against business cases, enforcing strict markdown document hierarchy
  ("## I. THE CENTRAL THESIS / A TESE CENTRAL", "## II. THE ENTERPRISE / A EMPRESA"),
  and conducting multi-stage blueprint synthesis.
---

# Blueprint Orchestrator: Master Workflow Skill

This skill coordinates the multi-agent workflow that ingests raw, ambiguous business concepts and synthesizes them into institutional-grade, venture-backed company conception blueprints.

As the **Lead Integrator**, you are responsible for orchestrating the creation of a comprehensive Business Blueprint from a raw product idea. Your mandate is to transition unrefined concepts through specialized agent execution gates, ensuring end-to-end coherence, strict executive candor, and structural integrity.

---

## The Multi-Agent Blueprint Workflow

The process follows a deterministic 6-stage orchestration pipeline executing a structured 4-step domain sequence:

```
┌────────────────────────────────────────────────────────┐
│ 1. TRIGGER & INTAKE (Raw Business or Product Idea)     │
│    - Parse unstructured prompt, notes, or pitch       │
│    - Extract domain, buyer, and initial intuitions     │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│ 2. STEP 1 (THESIS): Business Strategist Agent          │
│    - Strategic Foundation: Core Thesis & Inflection    │
│    - ## I. THE CENTRAL THESIS & ## II. THE ENTERPRISE  │
│    - Category Design & Boundary Matrix (IS vs IS NOT)  │
│    - Multi-Tiered Monetization & Unit Economics        │
│    - Non-Feature Moat & Defensibility Pillars          │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│ 3. STEP 2 (PRODUCT & MARKET): Product & GTM Lead Agent │
│    - Product & Go-to-Market Strategy Stage             │
│    - Beachhead Market & Trojan Horse MVP Wedge         │
│    - Land-and-Expand Product Roadmap (>120% NRR)       │
│    - Horizontal Core vs Configurable Schemas (Rule 3)  │
│    - Enterprise GTM Engine & MEDDPICC Sales Funnel     │
│    - Authority Marketing & Replicable 30-Day CS        │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│ 4. STEP 3 (STRUCTURE): Corporate Architect Agent       │
│    - Corporate & Technical Architecture Stage          │
│    - Event-Driven Architecture & Physical Data Limits  │
│    - Dev/Staging/Prod GitOps Isolation & Portability   │
│    - Cybersecurity Moat (SOC 2 / ISO 27001 Readiness)  │
│    - 100% IP Asset Ownership & Clean Chain of Title    │
│    - Essential SaaS Contract Suite (MSA, DPA, SLA)     │
│    - Lean Corporate Governance: Anti-Board; SHA Terms  │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│ 5. STEP 4 (ECONOMICS): Finance & Venture Agent         │
│    - Financial Architecture & Capital Strategy Stage   │
│    - P&L Segregation (Software ARR vs Data Pass-Thru)  │
│    - Core KPIs (MRR, ARR, NRR, Gross Margin, Payback)  │
│    - 4-Gate Staged Capital Strategy (12-18m Runway)    │
│    - Institutional Investment Thesis (5 Pillars)       │
│    - Pragmatic 18-Month Execution Roadmap (Rule 3)     │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│ 6. FINAL ASSEMBLY: Red-Team Audit & Master Synthesis   │
│    - Internal Red-Team Adversarial Audit (Fast-Follow) │
│    - Hurdle Rate Scoring (LTV/CAC, Payback, Margins)   │
│    - Rule 1 (Synthesis): Single cohesive Markdown doc  │
│    - Rule 2 (Formatting): Sections I to VIII flow      │
│    - Rule 3 (Tone Consistency): Strict executive candor│
│    - Final Master Conception Blueprint Emission        │
└────────────────────────────────────────────────────────┘
```

> [!NOTE]
> **Workflow Sequencing vs. Document Assembly Sequence**:
> Execution Step 2 (Product & Market) deliberately precedes Step 3 (Structure) because the Trojan Horse MVP wedge, initial integration gravity, and GTM throughput requirements directly define the technical architecture, latency limits, and legal compliance boundaries that the Corporate Architect must dimension in Step 3. In the final assembled document, Section VI (Technical Architecture, Cybersecurity & Governance) is placed before Section VII (Product Roadmap & GTM) to establish institutional engineering and legal credibility before presenting commercial execution.

---

## Workflow Sequence & Execution Gates

### 1. Trigger: Raw Idea Intake & Hypothesis Dissection
- **Trigger**: When the user provides a raw business or product idea, initiate the sequence.
- **Lead Integrator Action**:
  - Ingest unstructured concept text, founder notes, market observation, or napkin idea.
  - Deconstruct the input into core domain, hypothesized economic buyer, operational friction point, and proposed technological mechanism.
  - Construct the normalized `HypothesisContext` payload.

### 2. Step 1 (Thesis): Strategic Foundation (Business Strategist Agent)
- **Agent Called**: **Business Strategist Agent** (`business-strategist-agent`).
- **Skills Activated**:
  - `modern-category-design-and-positioning`
  - `modern-monetization-and-economic-architecture`
  - `modern-moat-and-defensibility-strategy`
- **Mandate**:
  - Synthesize the core problem into an ownable market category moniker (rejecting generic descriptors).
  - Formulate `# I. A TESE CENTRAL` pinpointing the macroeconomic, regulatory, or structural inflection point.
  - Define the corporate solution in `# II. A EMPRESA` with the exact directional value chain flow:
    $$\mathbf{DATA} \longrightarrow \mathbf{SIGNAL} \longrightarrow \mathbf{CONTEXT} \longrightarrow \mathbf{DECISION}$$
  - Construct the Category Boundary Matrix comparing "What the Company IS" versus "What the Company IS NOT".
  - Architect the 4-layer monetization model and calculate institutional unit economics ($LTV/CAC \ge 3.0\times - 5.0\times$, Payback $\le 12\text{ months}$).
  - Establish the 4 non-feature structural defensibility pillars (Switching Costs, Network Effects, Derived Data, Accumulated Decision History).
- **Output Artifact**: `StrategicFoundationDraft` (Structured Markdown).

### 3. Step 2 (Product & Market): Product & Go-to-Market Strategy Stage (Product & GTM Lead Agent)
- **Agent Called**: **Product & GTM Lead Agent** (`product-gtm-lead-agent`).
- **Input**: Pass output from Step 1 (`StrategicFoundationDraft`).
- **Skills Activated**:
  - `modern-beachhead-and-mvp-strategy`
  - `modern-land-and-expand-roadmapping`
  - `modern-enterprise-gtm-and-sales-engine`
- **Mandate**:
  - Identify the optimal Beachhead Market based on urgent pragmatic criteria: regulatory catalyst, cost of error $> \$1\text{M}$, pre-allocated executive budget.
  - Architect the Trojan Horse MVP Wedge: surgical critical-path product solving acute operational bleeding while embedding data interception gravity.
  - Map the multi-phase Land-and-Expand Product Roadmap (Wedge $\rightarrow$ Adjacent Modules $\rightarrow$ Horizontal Platform OS $\rightarrow$ Vertical Migration) driving $\ge 120\% - 130\%$ NRR.
  - Enforce **Rule 3 (Constraint)**: Immutable horizontal core engine paired with declarative domain configurations (YAML/JSON schemas), banning client-specific custom code forks.
  - Architect the high-ticket Enterprise GTM Engine: Founder-Led Sales motion evolving into AE + SA pods, Named Account Strategy, 5-Stage MEDDPICC Sales Funnel, Authority Marketing (Credibility $\rightarrow$ Education $\rightarrow$ Demand), and Replicable 30-Day CS Onboarding avoiding custom consulting.
- **Output Artifact**: `ProductGTMExecutionPlan`.

### 4. Step 3 (Structure): Corporate & Technical Architecture Stage (Corporate Architect Agent)
- **Agent Called**: **Corporate Architect Agent** (`corporate-architect-agent`).
- **Input**: Pass combined outputs from Step 1 and Step 2 (`StrategicFoundationDraft` + `ProductGTMExecutionPlan`).
- **Skills Activated**:
  - `modern-technical-architecture-and-security-paradigm`
  - `modern-ip-and-legal-asset-protection`
  - `modern-lean-corporate-governance`
- **Mandate**:
  - Design scalable event-driven architecture that respects the physical limits of upstream data sources (explicitly distinguishing event processing from upstream streaming vs polling vs batch latency).
  - Enforce multi-stage environment isolation (Dev, Staging, Prod) with GitOps promotion gates and structural vendor portability (OCI containers, open storage standards) eliminating vendor lock-in (**Rule 3: Constraint**).
  - Embed cybersecurity (AES-256-GCM at rest, TLS 1.3 in transit, KMS envelope encryption, IAM least privilege, SOC 2 Type II / ISO 27001 readiness) as an active commercial sales asset and enterprise procurement accelerator.
  - Mandate 100% corporate IP ownership: airtight PIIA covenants, present assignment language ("hereby assigns"), moral rights waivers, and immediate repository/domain turnover from outsourced software factories (**Rule 3: Constraint**).
  - Standardize the essential early-stage contract suite: Enterprise SaaS Master Services Agreement (12-month liability cap), Data Processing Agreement (DPA), Service Level Agreement (99.9% uptime SLA), and mutual NDA.
  - Enforce **Rule 1 (Governance)**: Strictly prohibit premature ornamental governance structures (formal boards of directors, external voting seats) prior to priced Series A; institute a 60-minute monthly executive decision cadence governed by 1-page Executive Decision Records (EDRs) and execute a mandatory Shareholders' Agreement (4-year reverse vesting with 1-year cliff, good/bad leaver, drag/tag rights, non-compete).
- **Output Artifact**: `CorporateArchitectureAndLegalFoundation`.

### 5. Step 4 (Economics): Financial Architecture & Capital Strategy Stage (Finance & Venture Agent)
- **Agent Called**: **Finance & Venture Agent** (`finance-venture-agent`).
- **Input**: Pass all prior outputs from Steps 1, 2, and 3 (`StrategicFoundationDraft` + `ProductGTMExecutionPlan` + `CorporateArchitectureAndLegalFoundation`).
- **Skills Activated**:
  - `modern-unit-economics-and-pnl-architecture`
  - `modern-staged-capital-and-runway-strategy`
  - `modern-institutional-investment-thesis`
- **Mandate**:
  - Structure the segregated financial model & P&L: strictly isolate software platform ARR from third-party data pass-through fees and hosting COGS to prove software gross margins ($\ge 80\%$) versus low-margin data reselling.
  - Model core institutional SaaS KPIs: MRR, ARR, NRR ($\ge 120\% - 130\%$), Blended Gross Margin ($\ge 75\% - 85\%$), CAC, CAC Payback ($\le 12\text{ months}$), LTV/CAC ($\ge 3.0\times - 5.0\times$), and Cloud/Data Cost per Revenue ($\le 15\% - 20\%$).
  - Engineer the milestone-driven 4-Gate Staged Capital Strategy (Gate 1: Build, Gate 2: Validation, Gate 3: Commercialization, Gate 4: Scale), budgeting 12 to 18 months of operating runway per stage to prevent emergency cash calls and punitive down-rounds.
  - Author the Institutional Investment Thesis highlighting the 5 Pillars of Enterprise Equity Value: contractual recurring ARR, programmatic land-and-expand, high structural switching costs, software economies of scale, and proprietary derived data accumulation.
  - Formulate the pragmatic 18-month execution roadmap (Month 0-2: Foundation, Months 2-5: Build, Months 5-8: Validation, Months 8-12: Commercialization, Months 12-18: Scale Decision) strictly enforcing **Rule 1 (Pragmatism)** (ban vanity metrics; unit economics authorize hiring) and **Rule 3 (Action Plan)**.
- **Output Artifact**: `FinancialEngineAndInvestmentThesis`.

### 6. Final Assembly: Red-Team Adversarial Audit & Master Manifesto Assembly
- **Auditor**: **Lead Integrator** (executing internal Red-Team Adversarial Audit via `modern-moat-and-defensibility-strategy`).
- **Mandate**:
  - Subject intermediate outputs to the Fast-Follower Test (can 10 engineers clone this in 6 months?) and Incumbent Free-Bundling Test (what happens if AWS/Microsoft offers this as a free feature?).
  - Verify strict adherence to hurdle rates: $LTV/CAC \ge 3.0\times$, Payback $\le 12\text{ months}$, Blended Gross Margins $\ge 75\% - 85\%$ (Software Margin $\ge 85\%$), $NRR \ge 120\%$.
  - Enforce the 3 non-negotiable Output Rules and synthesize the master document.

---

## Output Rules (Lead Integrator Mandates)

Every completed blueprint assembled by the Lead Integrator MUST strictly comply with these three Output Rules:

### Rule 1 (Synthesis) — Single Cohesive Executive Markdown Document
- **Zero Conversational Residue**: Do NOT present outputs as disjointed agent conversations, dialogue logs, "Agent A says / Agent B responds" transcripts, or fragmented status updates.
- **Unified Master Document**: Synthesize the contributions of all specialized agents into a single, cohesive, publication-ready, executive-grade Markdown document (`MasterConceptionBlueprint.md`).
- **Seamless Conceptual Continuity**: Ensure that terminology, product names, target account definitions, unit economics numbers, and architectural patterns flow seamlessly across sections without contradiction.

### Rule 2 (Formatting) — Numbered Chronological & Strategic Business Manifesto Flow
- **Standard Manifesto Hierarchy**: Structure the master document using clear, numbered Roman numeral sections (using `##` H2 level, reserving `#` H1 for the document title) matching the chronological and strategic flow of a formal business manifesto:
  1. `## I. THE CENTRAL THESIS` *(or `## I. A TESE CENTRAL`)* (Contemporary operational problem, macro/regulatory inflection, incumbent failure)
  2. `## II. THE ENTERPRISE` *(or `## II. A EMPRESA`)* (Corporate solution, directional value chain flow: $\text{DATA} \rightarrow \text{SIGNAL} \rightarrow \text{CONTEXT} \rightarrow \text{DECISION}$)
  3. `## III. CATEGORY DESIGN & ANTI-POSITIONING` (Ownable category moniker, 5-dimension IS vs IS NOT Boundary Matrix)
  4. `## IV. MONETIZATION & ECONOMIC ARCHITECTURE` (4-layer revenue model, unit economics table, gross margin roadmap)
  5. `## V. MOAT & DEFENSIBILITY MATRIX` (4 non-feature structural defensibility pillars)
  6. `## VI. TECHNICAL ARCHITECTURE, CYBERSECURITY & CORPORATE GOVERNANCE` (Event-driven pipeline, physical data limits, anti-lock-in, cybersecurity moat, 100% IP ownership, SaaS contract suite, lean governance)
  7. `## VII. PRODUCT ROADMAP & GO-TO-MARKET EXECUTION PLAN` (Beachhead criteria, Trojan Horse MVP, Land-and-Expand roadmap, horizontal core vs configurable schemas, enterprise GTM, MEDDPICC funnel, 30-day CS onboarding)
  8. `## VIII. CAPITAL ALLOCATION & EXECUTION MILESTONES` (P&L software segregation, Core KPIs scorecard, 4-gate funding with 12-18m runway, institutional investment thesis, pragmatic 18-month execution roadmap)

### Rule 3 (Tone Consistency) — Strict Executive Candor Across All Sections
- **Purge Startup Jargon & Optimistic Fluff**: Maintain uncompromising executive candor throughout the entire document. Absolute ban on startup clichés, consumer hyperbole, and empty marketing platitudes (e.g., "game-changer", "revolutionary", "all-in-one platform", "democratizing", "disruptive synergy", "best-in-class").
- **Cold Economic Realities**: Base every assertion on cold, unyielding commercial facts: customer acquisition friction, sales cycle length, buyer budget authority, gross margin erosion, cloud/compute COGS, and counterparty operational risk.
- **Uniformity Across Sections**: Ensure the tone remains equally rigorous across product, architectural, legal, and financial sections—never permitting technical optimism in engineering sections or commercial hype in GTM sections.

---

## Execution Guide for Lead Integrator

When prompted with a raw business idea:
1. **Trigger & Ingestion**: Normalize the user's prompt into `HypothesisContext`.
2. **Step 1 (Thesis)**: Invoke the **Business Strategist Agent** to build the strategic foundation, ownable category, monetization model, and defensibility moats.
3. **Step 2 (Product & Market)**: Pass Step 1 output to the **Product & GTM Lead Agent** to design the Trojan Horse MVP, Land-and-Expand roadmap, and high-ticket enterprise sales engine.
4. **Step 3 (Structure)**: Pass Step 1 and Step 2 outputs to the **Corporate Architect Agent** to architect event-driven infrastructure, embed cybersecurity, mandate 100% IP ownership, standardize SaaS contracts, and establish lean governance.
5. **Step 4 (Economics)**: Pass all upstream outputs to the **Finance & Venture Agent** to structure segregated P&L, model institutional KPIs, engineer the 4-gate capital strategy, craft the investment thesis, and detail the 18-month execution roadmap.
6. **Final Assembly (Audit & Synthesis)**: Execute the **Red-Team Adversarial Audit**, apply Output Rules 1, 2, and 3, and emit the unified master conception manifesto.

---

## Detailed References & Resources

- **In-Depth Guides**:
  - [Multi-Agent Workflow Choreography](./references/multi_agent_workflow_choreography.md): Sequence diagrams, agent state transfer, and execution protocols.
  - [Conception Document Standard](./references/conception_document_standard.md): The official specification of an institutional company blueprint.
- **Case Studies & Examples**:
  - [Sample Company Conception Blueprint](./examples/sample_company_conception_blueprint.md): Full-scale reference implementation of a synthesized blueprint.
- **Templates & Tools**:
  - [Blueprint Review Checklist](./resources/blueprint_review_checklist.md): Pre-flight verification checklist for completed blueprints.
