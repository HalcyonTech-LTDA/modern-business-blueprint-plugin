---
name: modern-beachhead-and-mvp-strategy
description: >-
  Use this skill when identifying the optimal enterprise entry market and defining the beachhead MVP wedge:
  evaluating urgent pragmatic criteria (regulatory pressure, high cost of error, budget availability),
  architecting a highly focused first product solving acute operational pain, and serving as a trojan horse
  for a broader horizontal infrastructure platform.
---

# Beachhead & MVP Strategy

This skill provides the strategic frameworks, evaluation criteria, and architectural principles for the **Product & GTM Lead Agent** (VP of Product & CRO) to identify the optimal enterprise beachhead market and design an irresistible MVP wedge.

---

## Core Principles

1. **Pragmatic Beachhead Selection Criteria**:
   - Startups fail in enterprise markets when they target broad, horizontal audiences or generic customer segments that lack urgent buying catalysts.
   - The beachhead market must be chosen based on cold, pragmatic criteria where customer inertia is broken by external structural forces:
     - **Urgent Regulatory or Compliance Pressure**: Impending regulatory mandates, audit deadlines, or supervisory enforcement orders where non-compliance results in statutory penalties or operational suspension.
     - **Catastrophic Cost of Error**: Environments where a failure, manual mistake, or operational lag directly causes six- or seven-figure financial loss, fraud leakage, or existential liability.
     - **Pre-Allocated Budget Availability**: The target segment already spends millions on broken manual processes, legacy software maintenance, or outsourced consultants to solve this exact issue. Budget does not need to be created; it only needs to be reallocated.
     - **Concentrated ICP with Short Decision Cycles**: The target accounts share near-identical operational topologies, allowing rapid referenceability and predictable sales cycles.

2. **The Trojan Horse MVP Concept**:
   - The MVP is not an incomplete, low-quality version of the ultimate vision; it is a surgical wedge.
   - It solves a single, highly acute operational pain point with overwhelming superiority, requiring minimal customer change management to deploy.
   - Crucially, it serves as a **Trojan Horse**:
     - It embeds deeply into the customer's core transaction flow, data pipeline, or daily decision ledger.
     - It intercepts the enterprise's data exhaust and establishes sticky operational integration.
     - Once inside, it creates natural dependencies that make deploying adjacent modules mathematically and operationally obvious.

3. **Ruthless MVP Scoping & Critical-Path Focus**:
   - Enterprise MVPs fail when they attempt "feature parity" with multi-decade legacy incumbents.
   - The product must reject extraneous bells and whistles (dashboards, report builders, custom notifications) and execute the single high-value transform with extreme speed and reliability.
   - Focus 100% of engineering bandwidth on the critical path: input ingestion $\rightarrow$ deterministic execution $\rightarrow$ downstream writeback.

4. **Horizontal Core Engine with Solution Configuration**:
   - Even at the MVP stage, the architecture must separate the immutable horizontal core engine (data ingestion, rule evaluation, event streaming, audit logging, security) from domain-specific configuration schemas.
   - Never write bespoke client-specific code or build custom software per account. Deliver customized behavior exclusively through declarative configurations and connectors.

---

## Step-by-Step Beachhead & MVP Strategy Procedure

```
┌─────────────────────────────────────────────────────────────────┐
│ STEP 1: Beachhead Candidate Identification & Scoring            │
│ (Filter against Regulatory Pressure, Cost of Error, Budget)     │
└───────────────────────────────┬─────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────┐
│ STEP 2: Acute Pain Diagnosis & Friction Deconstruction          │
│ (Isolate the bleeding neck operational failure mode)            │
└───────────────────────────────┬─────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────┐
│ STEP 3: Trojan Horse MVP Wedge Definition                       │
│ (Define minimal critical-path product & data interception hook) │
└───────────────────────────────┬─────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────┐
│ STEP 4: Horizontal Core Engine vs Configuration Demarcation    │
│ (Strictly ban custom client code; enforce declarative schemas)  │
└───────────────────────────────┬─────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────┐
│ STEP 5: Wedge Integration Gravity & Value Verification Metrics  │
│ (Define 14-day time-to-value proof and operational lock-in)     │
└─────────────────────────────────────────────────────────────────┘
```

### Step 1: Beachhead Candidate Identification & Scoring
Evaluate candidate market sub-sectors across five pragmatic vectors using the [Beachhead Scoring Rubric](./resources/beachhead_scoring_rubric.md):
1. *Regulatory/Statutory Catalyst*: Is there an external deadline forcing action within 6-12 months?
2. *Quantified Cost of Inaction*: Does doing nothing cost the buyer $> \$1\text{M}$ annually in direct losses or fines?
3. *Discretionary Budget Ownership*: Does an identifiable executive (e.g., CRO, CTO, Chief Compliance Officer) have immediate sign-off authority?
4. *Homogeneous Operational Stack*: Can 20 accounts use identical integration connectors without custom adaptation?
5. *Incumbent Vulnerability*: Are incumbents hamstrung by legacy batch architectures or consultative delivery models?

### Step 2: Acute Pain Diagnosis & Friction Deconstruction
Pinpoint the specific workflow choke point within the target beachhead:
- Identify who touches the problem daily and how long resolution takes.
- Quantify the latency, human error rate, or financial leakage under the status quo.
- Formulate the sharp value proposition: e.g., *"Reduce cross-border transaction compliance review latency from 4 hours to 180 milliseconds while cutting false positives by 74%."*

### Step 3: Trojan Horse MVP Wedge Definition
Architect the wedge product:
- **The Core Transform**: The single input $\rightarrow$ output contract executed autonomously.
- **Data Interception Hook**: How the MVP ingests live operational traffic (e.g., webhook listener, read-only replica, Kafka consumer).
- **The Trojan Horse Vector**: What data or workflow territory the MVP secures that enables horizontal platform expansion (e.g., capturing full counterparty payment history).

### Step 4: Horizontal Core Engine vs Configuration Demarcation
Enforce **Rule 3 (Constraint)**:
- Define the reusable horizontal engine:
  - High-throughput ingestion bus.
  - Decision/rule compilation engine.
  - Cryptographic audit trail.
  - Role-based access control and tenant isolation.
- Define the configuration schema:
  - Declarative YAML/JSON rule templates for the beachhead vertical.
  - Standardized integration adapters.
  - Reject all requests for bespoke one-off software builds.

### Step 5: Wedge Integration Gravity & Value Verification Metrics
Define concrete proof of value:
- **Deployment Velocity**: Initial live deployment in $\le 14$ business days.
- **Measurable Value Realization**: Quantifiable reduction in operational cost or risk demonstrated within 30 days of live traffic.
- **Expansion Telemetry**: Programmatic telemetry tracking volume growth to trigger expansion milestones.

---

## Detailed References & Resources

- **In-Depth Guides**:
  - [Beachhead Selection Matrix](./references/beachhead_selection_matrix.md): Pragmatic criteria, evaluation dimensions, and selection methodologies.
  - [Trojan Horse MVP Architecture](./references/trojan_horse_mvp_architecture.md): Engineering the minimal viable wedge that embeds deep operational integration gravity.
- **Case Studies & Examples**:
  - [Beachhead MVP Case Study](./examples/beachhead_mvp_case_study.md): Real-world dissection of an enterprise B2B infrastructure wedge landing in high-risk fintech compliance.
- **Templates & Tools**:
  - [Beachhead Scoring Rubric](./resources/beachhead_scoring_rubric.md): Quantitative scorecard for evaluating and ranking potential entry markets.
