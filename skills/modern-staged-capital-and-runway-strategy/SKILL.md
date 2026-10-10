---
name: modern-staged-capital-and-runway-strategy
description: >-
  Use this skill when architecting a milestone-driven venture capitalization strategy, engineering 4-gate risk reduction financing
  (Gate 1: Build, Gate 2: Validation, Gate 3: Commercialization, Gate 4: Scale) rather than arbitrary valuations,
  planning 12-18 months of runway per stage to prevent emergency cash calls, and establishing burn rate discipline.
---

# Staged Capital & Runway Strategy

This skill provides the venture capitalization framework, risk-reduction gate architecture, and runway management discipline for the **Finance & Venture Agent** (acting as combined Chief Financial Officer and Tier-1 Venture Capital Partner) to systematically fund early-stage enterprise ventures based on demonstrable risk reduction rather than arbitrary valuation hype.

---

## Core Principles

### 1. Risk-Reduction Gates vs. Arbitrary Valuations
- **The Core Problem**: Founders often raise capital based on arbitrary valuation aspirations ("we want to raise at a $25M valuation because our peers did"), leading to mispriced rounds, aggressive liquidation preferences, painful down-rounds, and desperate cash calls when growth stalls.
- **The Risk-Reduction Reality**: In institutional venture capital, capital is allocated to systematically extinguish specific venture risks. Valuation is an **output** of risk extinction, not an input.
- **The Four Risk Gates**:
  1. **Gate 1: Build (Technology & Feasibility Risk)**:
     - *Objective*: Prove the horizontal core engine can be built and achieve performance SLAs ($< 30\text{ms}$ streaming hot-path / $< 250\text{ms}$ complex multi-hop graph query latency).
     - *Capitalization*: Pre-Seed / Core Build round ($500k - $1.5M).
     - *Runway*: 12 to 18 months.
     - *Team Profile*: 2-4 core system engineers + founders. Zero sales reps.
  2. **Gate 2: Validation (Product-Market & Value Risk)**:
     - *Objective*: Deploy the Trojan Horse MVP wedge in shadow mode with 2 to 4 design-partner enterprise customers; prove false-positive reduction $\ge 70\%$ and zero business disruption.
     - *Capitalization*: Seed round ($2.0M - $3.5M).
     - *Runway*: 12 to 18 months.
     - *Team Profile*: Engineering + Solutions Architect + Founder-Led Sales. Zero commission-based account executives.
  3. **Gate 3: Commercialization (Go-To-Market & Repeatability Risk)**:
     - *Objective*: Convert initial pilots into paying commercial contracts; sign 10-15 paying enterprise logos; reach $\$1.0\text{M} - \$2.0\text{M}$ ARR (exit hurdle $\ge \$1.0\text{M} - \$1.2\text{M}$ contracted ARR); establish verified CAC payback $\le 12\text{ months}$ and NRR $\ge 120\%$.
     - *Capitalization*: Late Seed / Series A ($5.0M - $10.0M).
     - *Runway*: 15 to 18 months.
     - *Team Profile*: Founder sales transitions to first AE + Solutions Architect pod; initial Customer Success onboarding engineer.
  4. **Gate 4: Scale (Execution & Market Dominance Risk)**:
     - *Objective*: Pour capital into a proven, capital-efficient distribution machine with predictable CAC and compounding NRR; expand to adjacent modules and horizontal platforms.
     - *Capitalization*: Series B+ ($15.0M - $30.0M+).
     - *Runway*: 18 to 24 months.
     - *Team Profile*: Multi-pod GTM engine, dedicated channel partnerships, and international expansion authorized strictly by verified unit economics.

### 2. The 12-18 Month Runway Discipline & Cash Call Prevention
- Every capital tranche must secure a minimum of **12 to 18 months of operating runway** based on the post-round budget, plus a **3 to 6-month contingency cushion**.
- **The Desperate Cash Call Trap**: Raising only 6-9 months of runway forces founders to spend 50%+ of their operational time constantly fundraising, creates fatal vulnerability to macro market freezes, and inevitably leads to predatory emergency bridge notes with $2\times - 3\times$ liquidation preferences, full-ratchet anti-dilution, and founder equity wipeouts.
- **The Capital Freeze Mechanism**: If a venture approaches 6 months of remaining runway without meeting the binary exit criteria of its current gate, discretionary hiring and expansion are automatically frozen, and operations switch to capital preservation mode.

---

## The Four Gates Architecture Matrix

| Gate Parameter | Gate 1: Build | Gate 2: Validation | Gate 3: Commercialization | Gate 4: Scale |
| :--- | :--- | :--- | :--- | :--- |
| **Primary Venture Risk Extinguished** | Technology Feasibility & Ingestion Architecture | Operational Value Realization & Shadow Validation | Commercial Repeatability & Sales Unit Economics | Market Expansion & Organizational Scalability |
| **Capital Tranche Target** | $\$500\text{k} - \$1.5\text{M}$ | $\$2.0\text{M} - \$3.5\text{M}$ | $\$5.0\text{M} - \$10.0\text{M}$ | $\$15.0\text{M} - \$30.0\text{M}+$ |
| **Required Operating Runway** | **12 - 18 Months** | **12 - 18 Months** | **15 - 18 Months** | **18 - 24 Months** |
| **Hiring Authorization Rule** | Founders + Core System Architects only | + Forward Deployed Engineer; NO Account Executives | + 1-2 AE Pods authorized strictly by 2+ converted pilots | Multi-pod sales scaling authorized strictly by Payback $\le 12\text{m}$ |
| **Target Milestone Deliverables** | - Core streaming bus online<br>- Benchmark SLA verified<br>- SOC 2 Type I readiness | - 2-4 design partner pilots<br>- Shadow mode operational<br>- $\ge 70\%$ false positive drop | - 10-15 enterprise logos<br>- $\$1\text{M} - \$2\text{M}$ ARR ($\ge \$1.0\text{M} - \$1.2\text{M}$ exit hurdle)<br>- CAC Payback $\le 12\text{m}$<br>- $\text{NRR} \ge 120\%$ | - $\$5\text{M} - \$10\text{M}+$ ARR<br>- Blended Gross Margin $\ge 80\%$<br>- Module 2/3 cross-sell proven |
| **Binary Exit Hurdle (Pass/Fail)** | Working deterministic engine meeting latency SLA under load. | Pre-signed conversion letters from $\ge 2$ enterprise design partners. | Verified blended gross margin $\ge 75\% - 85\%$ (software margin $\ge 85\%$) and customer payback $\le 12\text{ months}$ with $\ge \$1.0\text{M} - \$1.2\text{M}$ ARR. | Multi-product expansion yielding $>125\%$ NRR across 2 consecutive quarters. |

---

## Procedural Runway & Capital Planning Procedure

```
┌────────────────────────────────────────────────────────┐
│ STEP 1: Current Risk Gate Identification               │
│ Classify venture: Gate 1, Gate 2, Gate 3, or Gate 4    │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│ STEP 2: Zero Cash Date (ZCD) & Runway Calculation      │
│ Compute Net Monthly Burn & ensure 12-18 month runway  │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│ STEP 3: Binary Exit Criteria & Hurdle Formulation     │
│ Define quantitative milestone hurdles to unlock Gate+1 │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│ STEP 4: Headcount Pacing & Unit Economic Authorization │
│ Ban premature sales hiring until Gate 3 exit met      │
└───────────────────────────┬────────────────────────────┘
                            │
                            ▼
┌────────────────────────────────────────────────────────┐
│ STEP 5: Emergency Cash Call Defense                    │
│ Implement 6-month minimum reserve capital lock         │
└────────────────────────────────────────────────────────┘
```

---

## Detailed References & Resources

- **In-Depth Guides**:
  - [The Four Risk-Reduction Funding Gates](./references/four_risk_reduction_funding_gates.md): Detailed gate criteria, milestone deliverables, and investor governance.
  - [Runway Planning & Cash Call Prevention](./references/runway_planning_and_cash_call_prevention.md): Financial defense against cram-down bridge financing and runway compression.
- **Case Studies & Examples**:
  - [Staged Capital Allocation Model](./examples/staged_capital_allocation_model.md): Multi-stage capitalization plan, dilution schedule, and budget allocations.
- **Templates & Tools**:
  - [Capital Gate Qualification Rubric](./resources/capital_gate_qualification_rubric.md): Binary scorecard for gating capital tranches and authorizing headcount expansion.
