# Enterprise Target Account & MEDDPICC Deal Qualification Matrix

Use this worksheet to evaluate and score prospective enterprise target accounts, qualify deal health across the sales funnel, and eliminate pipeline slippage.

---

## 1. Named Account Profile Scorecard

| Account Attribute | Evaluation Criteria | Ideal Enterprise Target Profile | Disqualification Red Flag | Account Status |
| :--- | :--- | :--- | :--- | :--- |
| **Annual Core Throughput** | Scale of operations (e.g. transactions, active users, assets) | $> \$2\text{B}$ in processed transactions or $> 1\text{M}$ active entities | Small scale ($< \$50\text{M}$ volume); cannot justify $> \$50\text{k}$ ACV | [ PASS / FAIL ] |
| **Regulatory Oversight** | Direct regulatory examination exposure | Regulated by FinCEN, OCC, SEC, PRA, BaFin, or CFPB | Unregulated or operating in jurisdictional grey zone | [ PASS / FAIL ] |
| **Current Tech Architecture** | Modern cloud & API event infrastructure | AWS / Azure / GCP with Kafka, SQS, or modern REST/gRPC | Legacy on-prem mainframe requiring custom binary builds | [ PASS / FAIL ] |
| **Existing Spend / Pain** | Quantifiable manual or legacy software costs | $> \$400\text{k}$ spent on manual review teams or legacy maintenance | No dedicated budget or problem resolved by 1 junior employee | [ PASS / FAIL ] |

---

## 2. MEDDPICC Deal Health Audit

Complete for all pipeline opportunities in Stages 2 through 4. Deals must score $\ge 14 / 16$ points before progressing to formal PoC.

| MEDDPICC Element | Score (0 - 2 Points) | Evidence / Verification Standard | Deal Notes |
| :--- | :---: | :--- | :--- |
| **Metrics (M)** | [ 0 / 1 / 2 ] | **2**: Dollar impact quantified and validated in writing by customer.<br>**1**: Internal metric estimated, not confirmed by buyer.<br>**0**: Qualitative goals only. | |
| **Economic Buyer (E)** | [ 0 / 1 / 2 ] | **2**: Direct 1-on-1 meeting completed with CRO/CFO/CEO; funding confirmed.<br>**1**: Economic Buyer identified but no direct access.<br>**0**: Unknown or unconfirmed. | |
| **Decision Criteria (D)** | [ 0 / 1 / 2 ] | **2**: Formal technical and commercial evaluation rubric shared in writing.<br>**1**: Informal criteria discussed verbally.<br>**0**: Undefined. | |
| **Decision Process (D)** | [ 0 / 1 / 2 ] | **2**: Documented timeline with named reviewers, committee dates, and board approvals.<br>**1**: General timeline without named milestones.<br>**0**: "We'll let you know". | |
| **Paper Process (P)** | [ 0 / 1 / 2 ] | **2**: Legal counsel and procurement lead identified; MSA/DPA templates exchanged.<br>**1**: Procurement process described verbally.<br>**0**: Unknown. | |
| **Identify Pain (I)** | [ 0 / 1 / 2 ] | **2**: Bleeding-neck catastrophic risk or fine if not resolved within 6 months.<br>**1**: Moderate inconvenience.<br>**0**: Low priority or aspirational project. | |
| **Champion (C)** | [ 0 / 1 / 2 ] | **2**: Senior internal stakeholder actively selling internally and providing coaching.<br>**1**: Friendly user without political power.<br>**0**: No internal advocate. | |
| **Competition (C)** | [ 0 / 1 / 2 ] | **2**: Incumbent, internal IT, and competitor strengths/weaknesses fully mapped.<br>**1**: Competitor names known without strategy.<br>**0**: "No competition". | |
| **TOTAL SCORE** | **[ ___ / 16 ]** | **Passing Hurdle: $\ge 14 / 16$ for PoC stage authorization** | |

---

## 3. Buying Committee Stakeholder Alignment Map

| Stakeholder Role | Name & Title | Core Buying Concern | Addressed Value Proposition | Alignment Status |
| :--- | :--- | :--- | :--- | :---: |
| **Economic Buyer** | [ Name, CRO / CFO ] | Bottom-line ROI, budget payback $< 6$ mos, risk reduction | Reallocates $680k manual spend to $120k software license | [ Confirmed / Pending ] |
| **Technical Champion** | [ Name, CTO / VP Eng ] | Zero downtime, $< 30$ms latency, clean API architecture | High-throughput streaming core; headless Kafka integration | [ Confirmed / Pending ] |
| **Operational User** | [ Name, Head of Ops ] | Alert fatigue, false positive rate, manual workload | Drops false positives by $> 70\%$; intuitive exception handling | [ Confirmed / Pending ] |
| **Risk / Gatekeeper** | [ Name, CISO / CCO ] | Data security, audit compliance, SOC2/ISO certification | Dedicated KMS tenant encryption, immutable cryptographic audit trail | [ Confirmed / Pending ] |
| **Procurement / Legal** | [ Name, Lead Counsel ] | Standard terms, indemnification, pricing predictability | Predictable annual platform tier + usage caps | [ Confirmed / Pending ] |
