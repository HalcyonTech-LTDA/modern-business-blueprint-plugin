# Enterprise Expansion Roadmap Matrix

Use this matrix to structure, evaluate, and sequence the product evolution path from initial beachhead wedge to horizontal enterprise infrastructure and cross-vertical dominance.

---

## 1. Product Evolution & Expansion Matrix

| Horizon | Product Scope & Module Name | Target Buyer & User Persona | Data Substrate Reused | Configuration vs Core Primitives | Expansion Trigger Metric | Target ACV | Target Gross Margin |
| :--- | :--- | :--- | :--- | :--- | :--- | :---: | :---: |
| **Phase 1: The Wedge (Months 0-6)** | **[Wedge Name]**<br>Focused critical-path problem (e.g. Sanctions Screen) | Primary: [e.g. Head of Compliance]<br>User: [e.g. Compliance Analyst] | Raw operational event stream (e.g. Kafka transaction topic) | Core: Streaming ingestion + rule engine.<br>Config: Policy schema YAML. | Baseline live deployment & 14-day SLA proof | $\$50\text{k}-\$100\text{k}$ | $75\%-80\%$ |
| **Phase 2: Adjacent Modules (Months 6-18)** | **[Module 2 & 3]**<br>Adjacent operational workflow (e.g. Monitoring + Filing) | Primary: [e.g. VP Financial Crime]<br>User: [e.g. Lead Investigator] | $\ge 80\%$ reuse of Phase 1 transaction & entity graph | Core: State machine & event generator.<br>Config: Workflow routing rules. | Usage reaches 80% capacity or manual backlog surge | $\$150\text{k}-\$300\text{k}$ | $80\%-83\%$ |
| **Phase 3: Horizontal OS (Months 18-36)** | **[Enterprise Platform]**<br>Consortium graph, fraud rings, cross-BU decisioning | Primary: [e.g. CRO / CISO / CTO]<br>User: [e.g. Fraud, Credit, Legal] | 100% unified multi-department context & history graph | Core: Graph traversal & cross-tenant anonymizer.<br>Config: Cross-BU permission matrices. | Multiple departments independently query API | $\$400\text{k}-\$1\text{M}+$ | $83\%-87\%$ |
| **Phase 4: Vertical Scale (Months 24+)** | **[Vertical Packs]**<br>Adjacent industry adaptation (e.g. Crypto, Healthcare) | Primary: [e.g. Chief Compliance Officer in New Vertical] | Structural workflow mapping & event message parity | Core: 100% shared horizontal engine.<br>Config: Domain schemas (FHIR, ISO). | Industry regulatory alignment & peer referenceability | $\$250\text{k}-\$750\text{k}$ | $85\%-90\%$ |

---

## 2. Expansion Governance Checklist

Before advancing a product module from Phase $N$ to Phase $N+1$, verify:
- [ ] **Data Pipeline Reusability**: Does the new module reuse $> 75\%$ of existing customer integrations without requiring a new IT data pipeline?
- [ ] **Zero Code Forking**: Can the new module be enabled for an existing customer purely via license key flag and configuration schema?
- [ ] **Marginal COGS Efficiency**: Does the incremental gross margin of the new module exceed the existing company average gross margin?
- [ ] **Shorter Sales Cycle**: Can the existing account add this module via a simple Order Form amendment in $< 30$ days?
- [ ] **Lock-in Compounding**: Does adding this module increase the switching cost for the entire account?
