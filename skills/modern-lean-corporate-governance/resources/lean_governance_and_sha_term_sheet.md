# Lean Governance & Shareholders' Agreement Term Sheet Template

This document provides the Corporate Architect Agent with an institutional term sheet checklist and the standard schema for monthly executive decision logs.

---

## 1. Shareholders' Agreement (SHA) Governance Term Sheet Checklist

| Governance Dimension | Standard Term Specification | Verification Criteria | Status |
| :--- | :--- | :--- | :--- |
| **Vesting Term** | 48 months (4 years) total duration. | Vesting Commencement Date explicitly defined. | Mandatory |
| **Cliff Period** | 12 months (1 year) cliff; 0% vests prior to month 12. | 25% vests at month 12; 1/48th monthly thereafter. | Mandatory |
| **Acceleration** | Double-trigger acceleration upon Change of Control + termination without cause within 12 months. | Single-trigger acceleration strictly prohibited. | Mandatory |
| **Bad Leaver Definition** | Felony, intentional fraud, embezzlement, uncurable material breach of SHA/PIIA, or resignation before cliff. | Objective statutory trigger criteria specified. | Mandatory |
| **Bad Leaver Buyback** | Unvested shares forfeited; vested shares repurchased at lower of nominal par value or 50% book value. | Price calculation formula clearly specified. | Mandatory |
| **Good Leaver Definition** | Involuntary termination without cause, death, permanent incapacity, or resignation post-cliff. | Leaves on mutually agreed terms. | Mandatory |
| **Good Leaver Buyback** | Vested shares retained or repurchased at Fair Market Value (FMV) in 12-24 monthly installments. | Valuation method & installment schedule defined. | Mandatory |
| **Drag-Along Right** | Compulsory sale triggered if $\ge 75\%$ of voting shares (including lead founder) approve bona fide acquisition. | Binds 100% of minority shareholders. | Mandatory |
| **Tag-Along Right** | Pro-rata co-sale right for minority shareholders on 100% identical pricing and terms. | Complete liquidity & pricing parity. | Mandatory |
| **Preemption / ROFR** | Company right of first refusal, followed by existing shareholders pro-rata. | 30-day notice and exercise period. | Mandatory |
| **Non-Compete** | 12 to 24 months post-departure non-compete within operating market category. | Geographic and business category bounds defined. | Mandatory |
| **Exclusivity** | 100% full-time commitment required during tenure. | Zero unauthorized outside commercial activity. | Mandatory |

---

## 2. Monthly Executive Decision Record (EDR) Schema

```markdown
# EXECUTIVE DECISION RECORD: EDR-[NUMBER]

- **Date**: YYYY-MM-DD
- **Meeting Cadence**: Monthly Executive Decision Meeting
- **Participants**: [CEO Name], [CTO/Corporate Architect Name], [CRO/COO Name]
- **Time Allocated**: 20 Minutes

---

### 1. Decision Title
[Unambiguous decision summary, e.g., "Selection of Primary Cloud Provider & Kubernetes Orchestration Engine"]

### 2. Context & Commercial Friction
[What operational problem, budget constraint, or procurement requirement demands a decision?]

### 3. Evaluated Options Matrix

| Option | Architecture / Provider | Marginal COGS Impact | Implementation Time | Vendor Lock-In Risk |
| :--- | :--- | :--- | :--- | :--- |
| **Option A** | [Description] | [$ / month] | [Weeks] | [Low / Med / High] |
| **Option B** | [Description] | [$ / month] | [Weeks] | [Low / Med / High] |

### 4. Final Verdict & Justification
- **Verdict**: [APPROVED / REJECTED / DEFERRED]
- **Selected Option**: [Option Name]
- **Rationale**: [Explain alignment with Rule 3 constraint and capital efficiency]

### 5. Accountability Contract
- **Single Accountable Owner**: [Name & Title]
- **Deliverable Milestone**: [Concrete measurable artifact]
- **Review Date**: [Next Monthly Executive Meeting Date]
```
