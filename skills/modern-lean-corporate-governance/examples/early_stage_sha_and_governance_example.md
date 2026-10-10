# Early-Stage SHA & Governance Implementation Example

*Scenario: Three co-founders incorporate a enterprise continuous decision intelligence startup ("Sentinela Infrastructure Corp"). They execute an ironclad Shareholders' Agreement and establish a lean monthly executive decision cadence.*

---

## 1. Capitalization Table & Vesting Structure

### Initial Cap Table Allocation:
- **Founder A (CEO)**: 450,000 Common Shares (45.0%)
- **Founder B (CTO & General Counsel / Corporate Architect)**: 400,000 Common Shares (40.0%)
- **Founder C (VP of Product / CRO)**: 150,000 Common Shares (15.0%)
- **Total Authorized & Issued Shares**: 1,000,000 Common Shares (100.0%)
- **Unallocated ESOP Pool**: 150,000 Shares reserved on a fully diluted basis.

### Reverse Vesting Execution:
- **Vesting Commencement Date**: January 1, 2026.
- **Cliff Date**: December 31, 2026 (Month 12).
- **Vesting Schedule**:
  - Month 0 - 11: 0 shares vested.
  - Month 12: 25% of shares vest (Founder A: 112,500; Founder B: 100,000; Founder C: 37,500).
  - Months 13 - 48: Equal monthly vesting of 1/48th per month (e.g., Founder B vests 8,333 shares/month).
- **Acceleration**: Double-trigger acceleration upon Change of Control + termination without cause within 12 months (75% unvested equity accelerates).

---

## 2. Leaver Resolution Case Study

### Case Scenario:
At Month 15 (3 months post-cliff), Founder C decides to resign voluntarily to pursue an unrelated consumer venture.

### Application of SHA Terms:
1. **Classification**: Founder C departed voluntarily *after* the 1-year cliff, had completed all handover obligations, and caused no harm to the company. Classification: **Good Leaver**.
2. **Equity Calculation**:
   - Total Shares Issued: 150,000 shares.
   - Vested Equity at Month 15: $150,000 \times \left(\frac{15}{48}\right) = 46,875 \text{ shares}$.
   - Unvested Equity: $103,125 \text{ shares}$.
3. **Repurchase Execution**:
   - **Unvested Shares**: 103,125 unvested shares are immediately repurchased by Sentinela Infrastructure Corp at nominal value ($0.001 per share = $103.125 total) and returned to treasury.
   - **Vested Shares**: Under the SHA Good Leaver provisions, the company exercises its option to repurchase the 46,875 vested shares at Fair Market Value determined by the recent post-money Seed valuation ($0.50/share = $23,437.50), payable in 18 equal monthly installments.
4. **Result**: Cap table cleanly sanitized, 103,125 shares returned to pool for future executive hiring, zero shareholder dispute, and clean chain of title maintained.

---

## 3. Sample Monthly Executive Decision Record Log

```markdown
# EXECUTIVE DECISION RECORD: EDR-004

- **Date**: 2026-10-06
- **Meeting**: October 2026 Monthly Executive Decision Meeting (09:00 - 10:00 UTC)
- **Attendees**: CEO, CTO/Corporate Architect, CRO

---

### Agenda & Timings:
- **09:00 - 09:10: Financial Health & Runway**
  - Cash Balance: $1,420,000.
  - Net Burn: $42,500/month.
  - Runway: 33.4 months.
  - AR Aging: Zero invoices overdue > 30 days.

- **09:10 - 09:30: Strategic Decision Memos**
  - **EDR-004 Evaluated**: SOC 2 Type II Readiness Platform Selection.
  - Evaluated Options: Vanta ($18,000/yr) vs Drata ($19,500/yr) vs Manual Consultant ($45,000).
  - Decision: APPROVED Vanta. Reason: Automated AWS/GitHub continuous evidence collection saves 120 engineering hours and accelerates Tier-1 bank vendor risk audit by 4 months.

- **09:30 - 09:50: Operational Blockers**
  - Engineering: Upstream court gazette parser experiencing format jitter; batch parser containerized and isolated with dead-letter queue.
  - Commercial: Regional Bank prospect requested mutual limitation of liability cap of 2x fees; CTO countered with standard 1x fees paid in preceding 12 months. Prospect accepted.

- **09:50 - 10:00: Accountability Log & Commitments**
  - [CTO/Corporate Architect]: Complete Vanta agent deployment on AWS Staging VPC by Oct 20.
  - [CRO]: Deliver signed Master Services Agreement + DPA for Regional Bank by Oct 25.
  - [CEO]: File Delaware corporate franchise tax and confirm updated PIIA register by Oct 15.
```
