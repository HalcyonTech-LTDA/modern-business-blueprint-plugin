# High-Ticket Enterprise Sales Funnel & MEDDPICC Qualification

This reference outlines the 5-stage enterprise sales funnel, deterministic exit criteria, and MEDDPICC deal governance required to close $50k to $500k+ ACV contracts with high predictability and low pipeline slippage.

---

## 1. The 5-Stage Enterprise Sales Funnel

Enterprise deals must never advance based on sales rep hope or conversational politeness. Every stage transition requires **concrete, customer-verified actions**.

```
┌─────────────────────────────────────────────────────────────────┐
│ STAGE 1: EXECUTIVE DISCOVERY & PAIN QUANTIFICATION              │
│ Objective: Identify quantified cost of status quo with Champion │
│ Exit Criteria: Documented economic pain ($> $500k/yr);          │
│                Introduction to Economic Buyer confirmed.        │
└───────────────────────────────┬─────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────┐
│ STAGE 2: ARCHITECTURAL QUALIFICATION & MEDDPICC SCRUTINY        │
│ Objective: Validate technical feasibility & map decision tree   │
│ Exit Criteria: Architecture review passed; InfoSec pre-cleared; │
│                MEDDPICC scorecard $\ge 80\%$; PoC Charter agreed.│
└───────────────────────────────┬─────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────┐
│ STAGE 3: TIMEBOXED PROOF OF CONCEPT (PoC / PILOT)               │
│ Objective: Prove technical & financial superiority in shadow mode│
│ Exit Criteria: Pre-agreed success metrics met in $\le 14$ days; │
│                Written confirmation from Economic Buyer.        │
└───────────────────────────────┬─────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────┐
│ STAGE 4: COMMERCIAL, SECURITY & LEGAL FINALIZATION              │
│ Objective: Finalize enterprise terms and regulatory compliance  │
│ Exit Criteria: Redlined MSA & DPA approved by Legal;            │
│                Security questionnaire signed; PO issued.        │
└───────────────────────────────┬─────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────┐
│ STAGE 5: CLOSED-WON CONTRACT EXECUTION & ONBOARDING KICKOFF     │
│ Objective: Secure signature and transition to Customer Success │
│ Exit Criteria: Executed Order Form; Invoiced Day 1;             │
│                Kickoff call scheduled within 3 business days.   │
└─────────────────────────────────────────────────────────────────┘
```

---

## 2. MEDDPICC Deal Qualification Framework

Every enterprise deal with an ACV $> \$50\text{k}$ must be audited weekly against the 8 MEDDPICC vectors:

| Letter | Dimension | Enterprise Qualification Standard | Disqualification / Slippage Flag |
| :---: | :--- | :--- | :--- |
| **M** | **Metrics** | What is the quantified financial outcome the buyer expects? (e.g., "$450k saved in analyst hours, 85% false positive reduction"). | Vague goals like "improve efficiency" or "modernize our stack" without hard dollar figures. |
| **E** | **Economic Buyer** | Has the person with final P&L budget authority (CRO, CFO, CEO) personally validated the business case? | Selling exclusively to mid-level managers who say "I need to check with my VP". |
| **D** | **Decision Criteria** | What are the exact technical, operational, and commercial criteria used to evaluate vendors? | Customer has not defined formal scoring criteria or criteria favor an incumbent's legacy RFP. |
| **D** | **Decision Process** | What is the step-by-step roadmap from demo to contract signature, including board approvals? | "We will review it next month and let you know what the next steps are." |
| **P** | **Paper Process** | Who handles legal redlines, procurement review, security questionnaires, and invoicing? | Sales rep has not contacted procurement or legal by Stage 3. |
| **I** | **Identify Pain** | What is the bleeding-neck catastrophe if they do nothing for the next 12 months? | "Our current system works fine, but we're curious about new technologies." |
| **C** | **Champion** | Is there an internal leader who has access to the Economic Buyer and actively sells on our behalf? | A friendly contact who likes the demo but has zero organizational influence or access to power. |
| **C** | **Competition** | Who else is competing (Incumbent vendor, internal build, status quo/inaction)? | Assuming "there is no competition" when the #1 competitor is always customer inertia and internal IT. |

---

## 3. The 14-Day Scored PoC Protocol

The Proof of Concept (PoC) is the most dangerous stage in an enterprise sales cycle: without strict discipline, PoCs drift into 6-month unpaid science experiments that exhaust engineering resources.

### The Mandatory Rules of Enterprise PoCs:
1. **Never Start Without a Signed PoC Charter**: The charter must explicitly state:
   - Exactly three quantifiable success criteria (e.g., latency $< 50\text{ms}$, accuracy $\ge 98\%$, zero false negatives on historical sample).
   - The test dataset size and delivery date.
   - The exact contractual statement: *"If the system meets the three criteria defined herein, Customer agrees to execute the Order Form for Year 1 subscription within 10 business days."*
2. **Strict Timebox ($\le 14$ Business Days)**: Enterprise infrastructure that requires more than two weeks to evaluate in sandbox or shadow mode is either too complex or poorly engineered.
3. **Daily Executive Telemetry Checkpoints**: Daily automated Slack/email summaries of test stream performance sent directly to the Technical Champion and Economic Buyer.
