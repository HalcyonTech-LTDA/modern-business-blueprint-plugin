# Multi-Agent Workflow Choreography: The Blueprint Conception Engine

This reference details the inter-agent communication, state transitions, and evaluation boundaries required to orchestrate a multi-agent workflow that turns raw ideas into institutional company conception documents.

---

## 1. Agent Topology & Specialization

The orchestration relies on specialized agent roles, with the **Business Strategist Agent** serving as the core strategic brain:

```
                  ┌───────────────────────────────────────────────┐
                  │    Blueprint Orchestrator Agent (Lead)        │
                  │    - Ingestion, Routing, Synthesis & Assembly │
                  └───────────────────────┬───────────────────────┘
                                          │
         ┌────────────────────────────────┼────────────────────────────────┐
         ▼                                ▼                                ▼
┌─────────────────────────┐   ┌─────────────────────────┐   ┌─────────────────────────┐
│ Business Strategist     │   │ Systems & Architecture  │   │ Go-to-Market & Growth   │
│ Agent (Core Strategic)  │   │ Agent (Tech Validation) │   │ Agent (Distribution)    │
│ - Tier-1 VC Partner     │   │ - Constraint Rule 3     │   │ - CAC & Sales Velocity  │
│ - Category Design       │   │ - COGS Optimization     │   │ - NRR Drivers           │
│ - Monetization & Moats  │   │ - Monetizable Tech      │   │ - ICP Budget Authority  │
└─────────────────────────┘   └─────────────────────────┘   └─────────────────────────┘
```

---

## 2. State Progression & Handoff Contracts

### State 1: Raw Idea Ingestion
- **State Payload**: Unstructured concept text, domain, hypothesized users, raw notes.
- **Orchestrator Action**: Parses raw input and constructs the `HypothesisContext` payload. Dispatches call to `Business Strategist Agent`.

### State 2: Strategic Conception (Business Strategist Agent)
- **Input**: `HypothesisContext`.
- **Processing**:
  - Synthesizes core problem into an ownable category moniker.
  - Formulates `# I. A TESE CENTRAL`.
  - Maps solution and directional value chain into `# II. A EMPRESA`.
  - Establishes the Boundary Matrix (IS vs IS NOT).
  - Drafts 4-layer monetization architecture and unit economics.
  - Architects 4 non-feature defensibility pillars.
- **Output Artifact**: `StrategicFoundationDraft` (Structured Markdown).

### State 3: Technical & Economic Feasibility Review (Systems Agent)
- **Input**: `StrategicFoundationDraft`.
- **Processing**:
  - Analyzes every architectural component against **Rule 3 (Constraint)**.
  - Verifies that proposed data pipelines, databases, and AI models have a direct monetization mechanism or quantified risk reduction.
  - Calculates line-item COGS and models the path to 80%+ gross margin.
- **Output Artifact**: `ValidatedTechnicalArchitecture` with verified COGS and tech-to-revenue mapping.

### State 4: Go-to-Market & Unit Economics Review (GTM Agent)
- **Input**: `StrategicFoundationDraft` + `ValidatedTechnicalArchitecture`.
- **Processing**:
  - Verifies sales motion, target buyer persona, and CAC payback timeline.
  - Confirms expansion drivers supporting $\ge 120\%$ NRR.
- **Output Artifact**: `ValidatedGTMStrategy`.

### State 5: Synthesis & Executive Assembly
- **Input**: All intermediate artifacts.
- **Processing**:
  - Enforces **Rule 1 (Tone)**: Strips all remaining buzzwords, startup jargon, and unsubstantiated optimism.
  - Validates **Rule 2 (Structure)**: Ensures document starts cleanly with `I. A TESE CENTRAL` and `II. A EMPRESA`.
  - Compiles the final institutional blueprint.
