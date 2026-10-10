# Intellectual Property Ownership & Chain-of-Title Framework

## 1. The Critical Nature of Clean Chain-of-Title

In institutional venture financing (Series Seed, Series A) and technology M&A exits, legal due diligence begins and ends with the **Chain of Title**. 

If a single former developer, outsourced agency, or co-founder contributed code, architecture schemas, or algorithms without an airtight, irrevocable assignment of intellectual property, the operating company does **not** legally own its technology. 

Under global IP jurisprudence (including US Copyright Act § 201, European copyright directives, and Brazilian Lei de Software nº 9.609/98):
- Independent contractors and external dev houses own the copyright to software they create by default, unless explicitly assigned in writing through a valid present assignment.
- An agreement that merely promises to assign in the future (e.g., *"the developer agrees to assign"*) does not transfer legal title automatically, requiring subsequent legal intervention or costly litigation.

---

## 2. Managing Outsourced Software Development Factories

Startups frequently leverage software agencies or outsourced nearshore/offshore development shops to build early prototypes. To satisfy **Rule 3 (Constraint)**, the Corporate Architect Agent must enforce five mandatory covenants before work commences:

### 1. Present-Tense Assignment Language:
Contracts must use explicit present assignment: *"The Contractor hereby irrevocably, unconditionally, and exclusively assigns, transfers, and conveys to the Company all right, title, and interest worldwide in and to all Deliverables, Inventions, Works of Authorship, Source Code, and related Intellectual Property."*

### 2. Full Waiver of Moral Rights:
In jurisdictions that recognize moral rights (e.g., France, Germany, Brazil, UK), authors retain paternity and integrity rights that cannot be assigned. The contract must contain a formal, irrevocable waiver of moral rights to the fullest extent permissible by applicable law.

### 3. Immediate Source Code & Custody Turnover:
- Code must be committed directly to corporate-owned version control repositories (e.g., GitHub, GitLab) under the company’s enterprise organization account.
- Storing code on agency-owned repositories or personal developer accounts is strictly prohibited.
- Payment milestones must be contractually tied to verified pull request merges and security/dependency audits.

### 4. Background Technology & Third-Party Library Carve-Outs:
- If the development agency uses pre-existing internal libraries or scaffolding ("Background Technology"), the agency must grant the company a perpetual, irrevocable, worldwide, royalty-free, fully paid-up, transferable, sublicensable license to use, modify, and commercialize such technology as part of the software.
- The agency must warrant that no proprietary agency tools create operational lock-in or prevent migration.

### 5. Open-Source Software (OSS) License Hygiene:
- Strict prohibition of viral copyleft licenses: The agency is prohibited from incorporating open-source code governed by GPL (General Public License v2/v3), AGPL (Affero GPL), or SSPL into the proprietary codebase.
- Permissible licenses are restricted to standard permissive licenses: MIT, Apache 2.0, BSD 2-Clause, and BSD 3-Clause.

---

## 3. The Founder & Employee PIIA Standard

Every founder, technical co-founder, and employee must execute a **Proprietary Information and Inventions Agreement (PIIA)** on their first day of association:

1. **Prior Inventions Schedule**: The individual must declare in writing any pre-existing code, patents, or projects created prior to joining the company. Any item not explicitly scheduled is legally deemed company property if created during the relationship.
2. **Duty of Disclosure**: Mandatory obligation to immediately disclose all inventions, improvements, and architectural concepts developed during the tenure.
3. **Power of Attorney (Attorney-in-Fact)**: If the company cannot secure the individual's signature to file a patent, copyright registration, or trademark after diligent effort (e.g., incapacity or resignation), the agreement appoints the company's officers as the individual’s attorney-in-fact to execute the filings.
4. **Post-Termination IP Cooperation**: Obligation to reasonably cooperate with the company in defending or perfecting intellectual property rights post-employment.
