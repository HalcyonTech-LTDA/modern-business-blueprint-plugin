# Early-Stage Enterprise Contract Framework

Enterprise customer contracts determine enterprise valuation. A single unvetted customer contract with uncapped liability, intellectual property assignments, or perpetual warranties can kill a venture financing round or acquisition.

The Corporate Architect Agent must implement and enforce four standardized, mutually reinforcing contractual pillars.

---

## 1. Enterprise SaaS Master Services Agreement (MSA)

The MSA governs the primary commercial subscription relationship between the company and enterprise customers.

### Key Structural Provisions:
1. **License Grant vs. Sale of Software**:
   - The customer receives a non-exclusive, non-sublicensable, non-transferable, revocable right to access and use the cloud-hosted platform during the Subscription Term.
   - Explicitly state: *"Nothing in this Agreement constitutes a sale or transfer of any software, source code, or intellectual property."*
2. **Intellectual Property Reservation & Data Rights**:
   - **Customer Data**: The customer retains 100% ownership of raw data submitted to the platform.
   - **Platform & System IP**: The company retains 100% ownership of the platform, source code, documentation, APIs, algorithms, model weights, and rules engines.
   - **Aggregated / De-Identified Telemetry**: The company must retain the irrevocable, royalty-free right to collect, aggregate, and analyze anonymized operational metadata and usage telemetry to improve system performance, benchmarks, and threat intelligence models.
3. **Limitation of Liability (The Institutional Standard)**:
   - **Aggregate Cap**: Each party’s total aggregate liability arising out of or related to the Agreement is strictly capped at the total amount paid by the customer in the preceding 12 months.
   - **Waiver of Consequential Damages**: Neither party shall be liable for indirect, incidental, special, exemplary, or consequential damages (including loss of profits, revenue, or business interruption).
   - **Carve-Outs**: Narrowly confined strictly to: (a) willful misconduct or gross negligence, (b) breach of confidentiality obligations, or (c) third-party IP indemnification obligations.
4. **Third-Party IP Indemnification Defense**:
   - The company defends the customer against third-party claims alleging that the platform directly infringes a valid patent or copyright, subject to:
     - Prompt written notification from the customer.
     - Sole control of defense and settlement by the company.
     - Exclusions if the customer modifies the platform, combines it with unauthorized software, or uses it contrary to documentation.

---

## 2. Data Processing Agreement (DPA)

Required under global data privacy regimes (GDPR Article 28, LGPD Article 39, CCPA/CPRA) whenever the platform processes personal data on behalf of enterprise customers.

### Mandatory DPA Standards:
1. **Classification of Roles**: Customer acts as the Data Controller; the company acts as the Data Processor (or Service Provider).
2. **Security Safeguards**: The company warrants technical and organizational measures (TOMs) including AES-256 encryption at rest, TLS 1.3 in transit, automated vulnerability scanning, and SOC 2 / ISO 27001 controls.
3. **Sub-Processor Governance**:
   - The company maintains a published list of sub-processors (e.g., AWS, Cloudflare, Datadog).
   - The company must notify the customer $\ge 14-30$ days prior to engaging a new sub-processor, giving the customer reasonable grounds to object on data privacy grounds.
4. **Security Incident & Breach Notification**:
   - The company commits to notifying the customer without undue delay, and in any event within 48 to 72 hours, after becoming aware of a confirmed personal data breach.
5. **Data Deletion / Return upon Termination**:
   - Within 30 to 60 days of termination, the company deletes or returns all customer personal data, certifying destruction in writing, except where retention is required by applicable statutory record-keeping laws.

---

## 3. Service Level Agreement (SLA)

The SLA defines the availability commitments and operational support response times for the enterprise infrastructure.

### Essential SLA Architecture:
1. **Target Availability Percentage**:
   - Standard Enterprise Tier: $\mathbf{99.9\%}$ monthly uptime (allows $\approx 43.8$ minutes of unplanned downtime per month).
   - Mission-Critical High-Availability Tier: $\mathbf{99.95\%}$ monthly uptime (allows $\approx 21.9$ minutes of unplanned downtime per month).
2. **Standard Measurement Exclusions**:
   - Planned scheduled maintenance announced at least 48 hours in advance during off-peak hours (e.g., weekends 02:00-06:00 UTC).
   - Force majeure events, upstream cloud provider region-wide outages, or customer network/DNS misconfigurations.
3. **Severity Classification Matrix**:

| Severity Level | Definition | Target First Response | Target Workaround / Resolution |
| :--- | :--- | :--- | :--- |
| **Severity 1 (Critical)** | Core decision engine completely down; all transactions blocked. | $\le 15 \text{ minutes}$ | $\le 2 \text{ hours}$ |
| **Severity 2 (High)** | Major feature unavailable; system operational with workarounds. | $\le 1 \text{ hour}$ | $\le 8 \text{ hours}$ |
| **Severity 3 (Medium)** | Non-critical component degraded; analytics or export delayed. | $\le 4 \text{ hours}$ | $\le 24 \text{ hours}$ |
| **Severity 4 (Low)** | Minor cosmetic or documentation inquiries. | $\le 1 \text{ business day}$ | Next scheduled release |

4. **Sole & Exclusive Remedy Clause**:
   - SLA failures must result strictly in **Service Credits** applied against future invoices (e.g., 5% credit for $<99.9\%$, 10% for $<99.5\%$, capped at 20% of monthly fee).
   - The contract must explicitly state: *"Service credits are Customer's sole and exclusive financial remedy for any failure to meet the Service Level Commitments."*

---

## 4. Non-Disclosure Agreement (NDA)

An early-stage enterprise company must execute bilateral (mutual) NDAs during enterprise customer discovery, partner discussions, and vendor procurement.

### Critical NDA Protections:
1. **Bilateral Symmetry**: Protects both customer operational data and company source code, technical roadmaps, unit economics, and architecture designs.
2. **Indefinite Trade Secret Protection**: Standard confidential information obligations expire after 3 to 5 years, but **Trade Secrets** must remain confidential perpetually for as long as they qualify as trade secrets under law.
3. **Rejection of "Residuals" Clauses**: Enterprise buyers often slip in a "Residuals" clause allowing them to freely use ideas and concepts retained in the "unaided memory" of employees. The Corporate Architect Agent must reject residuals clauses, as they create an unmonitored back door to replicate proprietary rules engines and algorithms.
