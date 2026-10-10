# SaaS & Data Infrastructure KPI Methodology

This document details the exact mathematical formulas, calculation standards, and institutional audit benchmarks for enterprise SaaS and data infrastructure companies.

---

## 1. Top-Line Recurring Revenue KPIs

### Monthly Recurring Revenue (MRR) & Annual Recurring Revenue (ARR)
- **Mathematical Definition**:
  $$\text{MRR} = \sum_{i=1}^{N} \text{Contracted Recurring Software Subscription Fee}_i$$
  $$\text{ARR} = \text{MRR} \times 12$$
- **Strict Inclusions**: Base platform license fees, continuous entity surveillance fees, recurring tiered commitments.
- **Strict Exclusions**: One-time professional services, non-recurring setup fees, custom integration billings, and uncommitted overage spikes.

### Net Revenue Retention (NRR)
- **Mathematical Definition**:
  $$\text{NRR} = \frac{\text{ARR}_{\text{Beginning}} + \text{Expansion ARR} - \text{Contraction ARR} - \text{Churned ARR}}{\text{ARR}_{\text{Beginning}}} \times 100$$
- **Institutional Hurdle**:
  - Minimum acceptable: $110\%$
  - Target enterprise infrastructure benchmark: $\mathbf{\ge 120\% - 130\%}$
  - World-class compounding: $\ge 140\%$
- **Significance**: An NRR of $125\%$ means the company grows $25\%$ annually even if the new sales team signs zero new logos during the entire fiscal year.

### Gross Revenue Retention (GRR)
- **Mathematical Definition**:
  $$\text{GRR} = \frac{\text{ARR}_{\text{Beginning}} - \text{Contraction ARR} - \text{Churned ARR}}{\text{ARR}_{\text{Beginning}}} \times 100$$
- **Cap**: GRR cannot exceed $100\%$.
- **Institutional Hurdle**: $\ge 90\% - 95\%$. High GRR proves high structural switching costs and operational indispensability.

---

## 2. Unit Economics & Efficiency KPIs

### Fully Loaded Customer Acquisition Cost (CAC)
- **Mathematical Definition**:
  $$\text{CAC} = \frac{\text{Total S\&M Expenses}_{t-1}}{\text{New Customers Acquired}_t}$$
- **Audit Mandate (No Cheating)**:
  - Total S&M must include: Account Executive (AE) and Forward Deployed Solutions Architect (FDSA) base salaries + commissions, SDR salaries, sales management, travel & entertainment (T&E), legal contract negotiation costs, marketing collateral, software licenses (Salesforce, Apollo, Gong), and allocated overhead.
  - Ban on excluding sales engineering or founder sales hours during early stages.

### CAC Payback Period (Months)
- **Mathematical Definition**:
  $$\text{CAC Payback Period} = \frac{\text{CAC}}{\text{ARPU} \times \text{Blended Gross Margin \%}} \times 12$$
  *(Where ARPU is Average Contract Value / ARR per new customer).*
- **Institutional Hurdle**:
  - Capital-efficient benchmark: $\mathbf{\le 12\text{ months}}$ (Target: $6 - 9\text{ months}$).
  - Warning zone: $13 - 18\text{ months}$.
  - Fatal dilutive burn: $> 18\text{ months}$.

### Lifetime Value (LTV) and LTV/CAC Ratio
- **Mathematical Definition**:
  $$\text{LTV} = \frac{\text{ARPU} \times \text{Blended Gross Margin \%}}{\text{Annual Gross Logo Churn Rate}}$$
  $$\text{LTV / CAC Ratio} = \frac{\text{LTV}}{\text{CAC}}$$
- **Institutional Hurdle**:
  - Minimum viable hurdle: $\mathbf{\ge 3.0\times}$
  - Optimal enterprise software: $\mathbf{4.0\times - 6.0\times}$
  - Overly conservative (under-investing in GTM): $> 8.0\times$

---

## 3. Infrastructure & Margin KPIs

### Cloud & Data Cost per Revenue Ratio
- **Mathematical Definition**:
  $$\text{Cloud Infrastructure Ratio} = \frac{\text{Hosting, Compute, Storage \& Network COGS}}{\text{Total Revenue}} \times 100$$
  $$\text{Data Vendor Cost Ratio} = \frac{\text{Third-Party Feed \& API Ingestion COGS}}{\text{Total Revenue}} \times 100$$
  $$\text{Total Direct Infra Ratio} = \frac{\text{Cloud COGS} + \text{Data COGS}}{\text{Total Revenue}} \times 100$$
- **Institutional Hurdle**:
  - Total Direct Infra Ratio must remain $\mathbf{\le 15\% - 20\%}$ of Total Revenue.
  - Software Gross Margin must remain $\mathbf{\ge 85\% - 90\%}$.
  - Blended Gross Margin must remain $\mathbf{\ge 75\% - 85\%}$.

### Burn Multiple
- **Mathematical Definition**:
  $$\text{Burn Multiple} = \frac{\text{Net Cash Burn}}{\text{Net New ARR Added}}$$
- **Institutional Hurdle**:
  - Amazing efficiency: $< 1.0\times$ ($1.00 of net burn produces $> $1.00 of net new ARR).
  - Good efficiency: $1.0\times - 1.5\times$.
  - Mediocre efficiency: $1.5\times - 2.0\times$.
  - Distressed / Poor: $> 2.0\times$ (triggers capital freeze).
