# Outsourced Development & SaaS Contract Suite Implementation Example

*Scenario: An enterprise decision infrastructure startup ("DecisionCore Inc.") contracts an external development studio ("ByteCraft Studio") to build initial data ingestion workers, and simultaneously commercializes its platform to a Tier-2 regional bank ("First Horizon Bank") under an Enterprise Master Services Agreement.*

---

## 1. Outsourced Development Handover & IP Assignment Execution

### Context:
DecisionCore engaged ByteCraft Studio for a 90-day sprint to engineer Kafka ingestion adapters and PostgreSQL schema migrations.

### Legal Architecture Implemented:
1. **Contract Structure**: ByteCraft signed DecisionCore's Master Contractor Agreement with strict Work-for-Hire and present assignment language prior to writing the first line of code.
2. **Repository & Infrastructure Custody**:
   - ByteCraft developers were issued individual enterprise GitHub accounts within the `github.com/decisioncore-infra` organization.
   - All commits were signed using GPG keys tied to `@decisioncore.com` contractor accounts.
   - Deployments executed exclusively to DecisionCore's isolated AWS Development VPC. ByteCraft had zero access to production credentials or customer staging databases.
3. **Formal Handover & Release Certificate**:
   - At Sprint completion, ByteCraft's Managing Director executed a formal **Certificate of Complete Assignment and Delivery**:
     - Explicitly assigning all copyright, patent rights, and moral rights in the delivered code.
     - Warranting that zero GPL or AGPL libraries were incorporated into the codebase.
     - Confirming complete deletion of all local codebase clones, database dumps, and credentials from ByteCraft hardware.

---

## 2. Customer Commercialization: First Horizon Bank Contract Suite

First Horizon Bank entered an enterprise subscription contract with DecisionCore for Continuous Transaction Screening.

### Contract Suite Components:

```
┌────────────────────────────────────────────────────────────────────────┐
│ DECISIONCORE ENTERPRISE CONTRACT SUITE                                 │
│                                                                        │
│ 1. Enterprise Master Services Agreement (MSA)                          │
│    - $120,000 Annual Contract Value (ACV)                              │
│    - Platform access license granted; 100% IP retained by DecisionCore │
│    - Mutual liability cap: Capped strictly at $120,000                 │
│    - Consequential damages waived for both parties                     │
│                                                                        │
│ 2. Data Processing Agreement (DPA)                                     │
│    - Customer = Controller; DecisionCore = Processor                   │
│    - Technical Safeguards: AES-256-GCM at rest, TLS 1.3 in transit     │
│    - Security breach notification window: Within 48 hours              │
│    - Sub-processor authorization: AWS, Datadog pre-approved            │
│                                                                        │
│ 3. Service Level Agreement (SLA)                                       │
│    - Monthly Uptime Target: 99.9%                                      │
│    - Severity 1 Response Time: < 15 minutes                            │
│    - Financial Remedy: Exclusive Service Credits capped at 20% / month │
│                                                                        │
│ 4. Mutual Non-Disclosure Agreement (NDA)                               │
│    - 5-year confidentiality for commercial terms                       │
│    - Perpetual confidentiality for DecisionCore rules engine source    │
│    - "Residuals" memory clause explicitly stricken                     │
└────────────────────────────────────────────────────────────────────────┘
```

### Procurement Outcome:
Because the contract suite arrived pre-aligned with institutional standards, bank procurement completed legal review in **16 calendar days** without redlining DecisionCore's core IP ownership or liability caps.
