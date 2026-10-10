# Land and Expand Case Study: 36-Month Account Compounding

This case study demonstrates how an enterprise B2B infrastructure company expanded a single regional payment institution from a $65,000 initial beachhead contract to a $640,000 annual multi-module enterprise deployment across 36 months, generating a Net Revenue Retention (NRR) of 215% within the account.

---

## 1. Account Profile
- **Client**: Global RemitCorp (Cross-border payments provider operating across 42 countries).
- **Initial Pain**: FinCEN real-time sanctions screening mandate; legacy provider generated 94% false positive rate.
- **Initial Buyer**: VP of Regulatory Compliance.

---

## 2. The 36-Month Expansion Timeline

```
Year 1 (Month 0):
  └── Module 1: Sanctions Screening Wedge
      └── ACV: $65,000 ($45k base + $20k volume)
      └── Buyer: VP of Regulatory Compliance

Year 2 (Month 12):
  ├── Module 1: Volume Growth ($35k volume step-up)
  ├── Module 2: Real-Time Transaction Monitoring ($85k add-on)
  └── Module 3: Automated SAR Filing Agent ($45k add-on)
      └── Total ACV: $230,000 (253% YoY Expansion)
      └── Buyers: VP Compliance + Head of Financial Crimes

Year 3 (Month 24):
  ├── Modules 1-3: Volume Growth & Enterprise Commitment ($310k)
  ├── Module 4: Fraud Ring & Counterparty Graph Intelligence ($180k)
  ├── Module 5: Benchmark & Consortium Risk Feed ($75k)
  └── Cross-BU: Credit Risk Engine Integration ($75k)
      └── Total ACV: $640,000 (178% YoY Expansion)
      └── Buyers: Chief Risk Officer (CRO) + CTO + Chief Legal Officer
```

---

## 3. Detailed Expansion Breakdown

### Phase 1: Year 1 — The Clean Beachhead Landing ($65k ACV)
- **Deployment**: Integrated Module 1 (Sanctions Screening) via Kafka stream in 12 days.
- **Immediate Outcome**: False positives dropped from 94% to 18%; review latency dropped from 3 hours to 45ms.
- **Footprint Established**: The platform was now ingesting 100% of RemitCorp's raw international payment volume (4.2M transactions/month), capturing full counterparty, device, and beneficiary graphs.

### Phase 2: Year 2 — Intra-Account Modular Expansion ($230k ACV)
- **The Trigger**: Month 8 automated review showed RemitCorp's compliance team spending 450 hours per month writing manual Suspicious Activity Reports (SARs) based on transaction monitoring alerts.
- **The Pitch**: RemitCorp was already piping all transactions through the core engine. By activating **Module 2 (Continuous Transaction Monitoring)** and **Module 3 (Automated SAR Filing)**, their manual case backlog would be eliminated with zero additional IT integration work.
- **The Result**: 14-day add-on activation; ARR increased to $230,000. Customer reduced manual operational overhead by $320,000.

### Phase 3: Year 3 — Cross-Departmental Enterprise Transformation ($640k ACV)
- **The Trigger**: The Fraud Operations and Credit Underwriting teams were struggling with chargeback syndicates and requested access to the Counterparty Entity Graph built during Modules 1 & 2.
- **The Migration**: Upgraded RemitCorp from a departmental agreement to an **Enterprise Platform License (EPL)**.
- **New Modules Added**:
  - *Module 4: Fraud Syndicate Graph Intelligence* ($180k).
  - *Module 5: Derived Data Consortium Risk Feed* ($75k).
  - *Credit Risk API Integration* ($75k).
- **Contract Value**: $640,000 ARR with a 3-year committed term ($1.92M TCV).

---

## 4. Key Architectural Takeaways

1. **Zero Custom Engineering**: Throughout all 36 months, the core engineering team never created a RemitCorp-specific branch or customized binary. Every rule, scoring weight, and SAR template was declared in JSON/YAML configuration schemas.
2. **Data Gravity Preempted Incumbents**: When Fiserv and NICE Actimize attempted to displace the platform during Year 2 procurement renewals, RemitCorp rejected them because rebuilding the entity graph and real-time Kafka integration would take 18 months and cost $> \$1.2\text{M}$.
3. **High Gross Margins**: Delivered at an 84% gross margin; compute costs scaled linearly with transaction volume while software licensing expanded exponentially.
