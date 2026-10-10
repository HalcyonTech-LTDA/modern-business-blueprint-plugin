# Beachhead MVP Case Study: Real-Time Sanctions & AML Screening Wedge

This case study illustrates how an enterprise B2B infrastructure startup used the **Beachhead & MVP Strategy** to capture regional cross-border payment processors before expanding into a multi-million-dollar financial crime decision platform.

---

## 1. Beachhead Selection & Qualification

### Candidate Markets Evaluated
1. *Tier-1 Global Megabanks*: Enormous budgets, but 24-month procurement cycles, bespoke mainframes, and entrenched incumbents (Fiserv, NICE Actimize). **Result: DISQUALIFIED.**
2. *Retail Neo-banks*: Agile tech stacks, but low willingness to pay, high churn risk, and limited transaction volume. **Result: DISQUALIFIED.**
3. *Cross-Border Payment Remittance FinTechs & Regional Sponsor Banks*: Processing $10B+ annually, regulated by FinCEN/OCC, facing escalating cross-border AML screening penalties, operating on modern AWS/Kafka stacks, and bleeding millions in manual compliance analyst headcount. **Result: SELECTED BEACHHEAD.**

### Pragmatic Criteria Scorecard
- **Regulatory Pressure (Score: 10/10)**: Upcoming FinCEN Anti-Money Laundering Rule requiring real-time counterparty screening before transaction clearing (ending batch end-of-day checks).
- **Cost of Error (Score: 10/10)**: Single sanctions breach resulted in minimum $250k statutory fines and potential revocation of sponsor bank clearing licenses.
- **Pre-Allocated Budget (Score: 9/10)**: Target accounts spent an average of $680k annually on a team of 8 offshore manual compliance reviewers who reviewed flagged transactions with a 4-hour SLA.
- **Architectural Homogeneity (Score: 9/10)**: 85% of targets ran standard ISO 20022 payment messages streamed via Kafka or AWS SQS.
- **Trojan Horse Data Gravity (Score: 10/10)**: Intercepting the real-time payment instruction captures complete originator, beneficiary, routing, and device metadata.

---

## 2. The Trojan Horse MVP: "StreamShield Wedge"

### The Acute Pain Solved
Legacy screening tools generated a **92% false positive rate**, forcing human analysts to manually verify thousands of benign transactions. This introduced a 4-hour processing delay for customers and cost $55 per manual review.

### The MVP Scope
- **Input**: Ingests ISO 20022 `pacs.008` payment stream via Kafka topic.
- **Core Transform**: Deterministic fuzzy-matching entity graph combined with a zero-copy rule evaluation engine running in $< 25\text{ms}$.
- **Output**: Returns binary verdict (`APPROVE` with cryptographic audit token or `FLAG` with exact matched sanction entity and risk score) back to Kafka.
- **What Was Deliberately Omitted**: No user administration portals, no custom workflow case managers, no complex PDF report exporters. The integration was 100% headless API and webhook-driven.

### The Trojan Horse Mechanism
By sitting in the critical path between payment ingestion and ledger execution:
1. The MVP achieved **Shadow Mode deployment in 7 business days** (listening passively to Kafka without blocking payments).
2. Proved a **71% reduction in false positives** within 14 days of shadow evaluation.
3. Once switched to active mode, it became the mandatory statutory system of record for all regulatory audits.
4. It silently indexed every cross-border counterparty network, creating the foundational graph for Module 2: Continuous Fraud Ring Detection.

---

## 3. Commercial Impact

- **Initial ACV**: $85,000 base platform fee + $0.08 per screened transaction.
- **Average Year-1 Contract**: $135,000.
- **Time to First Value**: 11 business days.
- **Engineering Overhead**: Zero custom client branches. All compliance rule customizations configured via JSON policy schemas.
- **Beachhead Penetration**: Captured 18 regional remittance processors in 14 months, establishing uncontested market dominance in the sub-sector.
