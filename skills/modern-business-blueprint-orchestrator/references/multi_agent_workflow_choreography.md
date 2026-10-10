# Multi-Agent Workflow Choreography: The Blueprint Conception Engine

This reference details the inter-agent communication, state transitions, handoff contracts, and evaluation boundaries required to orchestrate the multi-agent workflow that turns raw ideas into institutional company conception documents.

---

## 1. Agent Topology & Lead Integrator Role

As the **Lead Integrator**, the **Blueprint Orchestrator Agent** directs the sequential execution of four specialized domain agents and executes the internal adversarial review (Red-Team Audit):

```
                  ┌─────────────────────────────────────────────────────────┐
                  │          Blueprint Orchestrator Agent (Lead)            │
                  │          - Role: Lead Integrator & Workflow Director    │
                  │          - Ingestion, Sequential Routing & Synthesis    │
                  └────────────────────────────┬────────────────────────────┘
                                               │
            ┌─────────────────────┬────────────┴────────┬─────────────────────┐
            ▼                     ▼                     ▼                     ▼
┌─────────────────────┐┌─────────────────────┐┌─────────────────────┐┌─────────────────────┐
│ Business Strategist ││ Product & GTM Lead  ││ Corporate Architect ││ Finance & Venture   │
│ Agent (Step 1)      ││ Agent (Step 2)      ││ Agent (Step 3)      ││ Agent (Step 4)      │
│ - Category Design   ││ - Beachhead MVP     ││ - Tech & Security   ││ - Segregated P&L    │
│ - Monetization & Moat││ - Land & Expand     ││ - 100% IP Ownership ││ - 4 Funding Gates   │
│ - Core Value Chain  ││ - Enterprise GTM    ││ - Lean Gov & SHA    ││ - 18-Mo Action Plan │
└─────────────────────┘└─────────────────────┘└─────────────────────┘└─────────────────────┘
```

> [!NOTE]
> **Execution Flow vs. Document Layout Sequence**:
> Execution Step 2 (Product & Market) deliberately runs before Step 3 (Structure) because the Trojan Horse MVP wedge and GTM pipeline requirements determine the technical throughput, event-handling latency, and compliance requirements that the Corporate Architect must solve in Step 3. In the final synthesized document (`MasterConceptionBlueprint.md`), the Lead Integrator arranges Section VI (Technical Architecture & Governance) prior to Section VII (Product Roadmap & GTM) to ground the company in rigorous infrastructure and legal governance before demonstrating the commercial go-to-market engine.

### Multi-Agent Roster & Specialization

The Modern Business Blueprint system consists of 5 executable agent personas, coordinated by the Lead Integrator:

| Agent Name | Specialized Role | Primary Directive | Key Artifact Produced |
| :--- | :--- | :--- | :--- |
| **Blueprint Orchestrator Agent** | Lead Integrator & Workflow Director | Coordinates agent execution, manages sequential handoffs, executes internal Stage 6 Red-Team audit, and compiles final master manifesto adhering to Output Rules 1, 2, 3. | `MasterConceptionBlueprint.md` |
| **Business Strategist Agent** | Tier-1 VC Partner & Serial Entrepreneur | Defines the core economic engine, ownable market category, defensible moat, and strategic thesis. | `StrategicFoundationDraft.md` |
| **Product & GTM Lead Agent** | VP of Product & Chief Revenue Officer | Defines beachhead entry market, Trojan Horse MVP wedge, land-and-expand roadmap, and high-ticket sales engine. | `ProductGTMExecutionPlan.md` |
| **Corporate Architect Agent** | Combined CTO & General Counsel | Designs scalable event-driven architecture, embeds cybersecurity as a moat, mandates 100% IP ownership, standardizes contract suites, and defines lean governance. | `CorporateArchitectureAndLegalFoundation.md` |
| **Finance & Venture Agent** | Combined CFO & Tier-1 VC Partner | Structures segregated P&L, models institutional KPIs, engineers 4-gate staged capital strategy, crafts investment thesis, and enforces 18-month execution roadmap. | `FinancialEngineAndInvestmentThesis.md` |

*(Note: The Red-Team adversarial audit is executed internally by the Blueprint Orchestrator Agent during Stage 6 rather than as a separate agent process, ensuring lean execution without communication overhead.)*

---

## 2. Sequential State Progression & Handoff Contracts

The execution follows a deterministic 6-stage pipeline executing 4 sequential domain steps:

### State 1: Trigger & Raw Idea Ingestion (Lead Integrator)
- **Trigger**: When the user provides a raw business or product idea, initiate the sequence.
- **State Payload**: Unstructured concept text, domain intuition, hypothesized users, raw notes, or napkin pitch.
- **Lead Integrator Action**: Parses raw input, identifies apparent friction and technical mechanisms, and constructs the normalized `HypothesisContext` payload. Dispatches call to `Business Strategist Agent`.

### State 2: Step 1 (Thesis) — Strategic Foundation (Business Strategist Agent)
- **Input**: `HypothesisContext`.
- **Processing**:
  - Synthesizes core problem into an ownable category moniker (rejecting generic labels).
  - Formulates `# I. A TESE CENTRAL` (Contemporary operational friction and macroeconomic/regulatory inflection).
  - Maps proprietary solution and directional value chain into `# II. A EMPRESA` ($\mathbf{DATA} \rightarrow \mathbf{SIGNAL} \rightarrow \mathbf{CONTEXT} \rightarrow \mathbf{DECISION}$).
  - Establishes the Boundary Matrix (What the Company IS vs What it IS NOT).
  - Drafts 4-layer monetization architecture (Platform, Monitoring, Usage, Derived Data) and unit economics targets ($LTV/CAC \ge 3.0\times - 5.0\times$, Payback $\le 12\text{ months}$).
  - Architects 4 non-feature structural defensibility pillars (Switching Costs, Network Effects, Derived Data, History Graph).
- **Output Artifact**: `StrategicFoundationDraft` (Structured Markdown).

### State 3: Step 2 (Product & Market) — Product & Go-to-Market Strategy (Product & GTM Lead Agent)
- **Input**: Pass output from Step 1 (`StrategicFoundationDraft`).
- **Processing**:
  - Identifies optimal beachhead market via urgent pragmatic criteria (statutory regulatory pressure, cost of error $> \$1\text{M}$, pre-allocated budget).
  - Defines the Trojan Horse MVP wedge solving acute critical-path pain while securing data interception gravity.
  - Maps the 4-phase Land-and-Expand product roadmap, enforcing horizontal core engine scalability without custom client forks (**Rule 3: Constraint**).
  - Architects the high-ticket B2B enterprise sales engine: Founder-led sales motion evolving into AE + SA pods, named account tiering, MEDDPICC 5-stage funnel, authority marketing (Credibility $\rightarrow$ Education $\rightarrow$ Demand), and replicable 30-day CS onboarding avoiding custom consulting (**Rule 1: Focus**).
- **Output Artifact**: `ProductGTMExecutionPlan`.

### State 4: Step 3 (Structure) — Corporate & Technical Architecture (Corporate Architect Agent)
- **Input**: Pass combined outputs from Step 1 and Step 2 (`StrategicFoundationDraft` + `ProductGTMExecutionPlan`).
- **Processing**:
  - Designs scalable event-driven architecture respecting physical data limits (streaming vs polling vs batch registers).
  - Establishes Dev/Staging/Prod environment isolation, GitOps promotion gates, and anti-lock-in portability (OCI containers, open storage protocols) (**Rule 3: Constraint**).
  - Embeds cybersecurity (AES-256-GCM, TLS 1.3, KMS envelope encryption, IAM least privilege, SOC 2 / ISO 27001 readiness) as an active commercial sales asset.
  - Secures 100% corporate IP ownership, present assignment covenants ("hereby assigns"), moral rights waivers, and contractor repository custody (**Rule 3: Constraint**).
  - Standardizes the essential early-stage contract suite (Enterprise SaaS MSA with 12-month liability cap, DPA, 99.9% uptime SLA, NDA).
  - Enforces **Rule 1 (Governance)**: Prohibits premature ornamental boards of directors, establishing a 60-minute monthly executive decision cadence with 1-page EDRs and mandatory Shareholders' Agreement terms (4-year reverse vesting with 1-year cliff, good/bad leaver, drag/tag rights, non-compete).
- **Output Artifact**: `CorporateArchitectureAndLegalFoundation`.

### State 5: Step 4 (Economics) — Financial Architecture & Capital Strategy (Finance & Venture Agent)
- **Input**: Pass all prior intermediate artifacts (`StrategicFoundationDraft` + `ProductGTMExecutionPlan` + `CorporateArchitectureAndLegalFoundation`).
- **Processing**:
  - Formulates segregated financial model and P&L strictly separating software revenue from data consumption costs (`modern-unit-economics-and-pnl-architecture`) to prove software gross margins ($\ge 80\%$).
  - Calculates core institutional KPIs: MRR, ARR, NRR ($\ge 120\% - 130\%$), Blended Gross Margin ($\ge 75\% - 85\%$), CAC, CAC Payback ($\le 12\text{ months}$), LTV/CAC ($\ge 3.0\times - 5.0\times$), and Cloud/Data Cost per Revenue ($\le 15\% - 20\%$).
  - Architects the 4-Gate Staged Capital Strategy (Gate 1: Build, Gate 2: Validation, Gate 3: Commercialization, Gate 4: Scale) with 12 to 18 months runway per stage (`modern-staged-capital-and-runway-strategy`).
  - Crafts the Institutional Investment Thesis highlighting the 5 Defensibility Pillars (`modern-institutional-investment-thesis`).
  - Defines the pragmatic 18-month execution roadmap (Foundation $\rightarrow$ Build $\rightarrow$ Validation $\rightarrow$ Commercialization $\rightarrow$ Scale Decision) enforcing **Rule 1 (Pragmatism)** and **Rule 3 (Action Plan)**.
- **Output Artifact**: `FinancialEngineAndInvestmentThesis`.

### State 6: Adversarial Red-Team Audit & Master Assembly (Lead Integrator Synthesis)
- **Input**: All validated intermediate artifacts.
- **Processing**:
  - Subject intermediate outputs to Fast-Follower Test (10 engineers / 6 months) and Incumbent Free-Bundling stress test.
  - Audit hurdle rates ($LTV/CAC \ge 3.0\times$, Payback $\le 12\text{ months}$, Blended Margins $\ge 75\% - 85\%$ [Software Margins $\ge 85\%$], $NRR \ge 120\%$).
  - Apply the **Lead Integrator Output Rules**:
    - **Rule 1 (Synthesis)**: Synthesize into a single, cohesive, publication-grade Markdown document (`MasterConceptionBlueprint.md`), completely eliminating fragmented conversational dialogue or agent transcripts.
    - **Rule 2 (Formatting)**: Structure using clear Roman numeral sections (`I` through `VIII`) following formal business manifesto flow.
    - **Rule 3 (Tone Consistency)**: Enforce strict executive candor and cold analytical business language, purging startup buzzwords across all sections.
  - Emit the finalized master company conception blueprint.

---

## 3. Communication Protocols & Quality Gates

1. **State Immutability**: Intermediate state payloads passed between stages are strictly additive and immutable. Downstream agents must not alter upstream category monikers or value chain definitions.
2. **Lead Integrator Output Rules**:
   - **Rule 1 (Synthesis)**: The Lead Integrator must never output disjointed agent conversational logs; all outputs must be synthesized into a single cohesive executive document (`MasterConceptionBlueprint.md`).
   - **Rule 2 (Formatting)**: Clear Roman numeral numbering (`I` through `VIII`) matching formal business manifesto structure.
   - **Rule 3 (Tone Consistency)**: Uncompromising executive candor and cold economic reality maintained uniformly across all sections.
3. **Deterministic Veto Power**: The Lead Integrator (via internal Stage 6 Red-Team audit), Corporate Architect Agent, Product & GTM Lead Agent, and Finance & Venture Agent possess absolute veto authority:
   - If the Corporate Architect Agent detects ambiguous IP ownership, external agency IP retention, unmitigated vendor lock-in, or premature ornamental governance (violating Rule 1 or Rule 3), the plan is immediately halted for remediation.
   - If the Corporate Architect Agent or Product Lead detects custom software for individual clients or technology lacking economic justification (violating Rule 3), the component is excised.
   - If the Product Lead detects B2C marketing tactics or undefined enterprise decision-makers (violating Rule 1 Focus), the commercial plan is rejected for redesign.
   - If the Finance & Venture Agent detects vanity metrics, unsegregated low-margin data pass-through revenue, or undercapitalized runway ($< 12\text{ months}$), the economic model is rejected for restructuring.
   - If the Lead Integrator's internal Red-Team audit detects low defensibility ($< 15/20$) or negative unit economics, the blueprint is returned for redesign.
4. **Executive Voice Consistency**: The Lead Integrator guarantees that the voice across all generated sections maintains the strict executive candor and cold analytical perspective of a Tier-1 Venture Capital Partner, CFO, CTO, General Counsel, VP of Product, and CRO.
