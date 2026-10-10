# Beachhead Market Qualification & Scoring Rubric

Use this quantitative rubric to evaluate and score potential enterprise entry markets. Candidate markets must achieve a total score of $\ge 40 / 50$ to qualify as an institutional beachhead.

---

## 1. Quantitative Evaluation Matrix

| Vector | Scoring Criteria (0 - 10 Points) | Weight | Minimum Hurdle | Candidate Score |
| :--- | :--- | :---: | :---: | :---: |
| **1. Statutory Regulatory Pressure** | **10**: Binding legal mandate enforced within 12 months with severe statutory fines.<br>**5**: Anticipated guideline or optional compliance framework.<br>**0**: No regulatory driver; purely discretionary purchase. | $1.0$ | **7 / 10** | [ ___ / 10 ] |
| **2. Asymmetric Cost of Error** | **10**: Single failure costs $> \$1\text{M}$ in fines, fraud loss, or business halt.<br>**5**: Failure costs $\$50\text{k}-\$250\text{k}$ with operational disruption.<br>**0**: Minor nuisance; failure costs $<\$10\text{k}$. | $1.0$ | **7 / 10** | [ ___ / 10 ] |
| **3. Pre-Allocated Budget Availability** | **10**: Identifiable C-level buyer spending $> \$300\text{k}$ annually on manual/legacy workarounds.<br>**5**: Budget exists in adjacent department but requires cross-functional approval.<br>**0**: No existing budget line item; requires new capital justification. | $1.0$ | **8 / 10** | [ ___ / 10 ] |
| **4. Architectural Homogeneity** | **10**: 80%+ of target accounts use standardized modern APIs, message buses, and cloud infrastructure.<br>**5**: Mix of cloud and legacy systems requiring moderate adapter configuration.<br>**0**: Highly heterogeneous mainframe/on-prem environments demanding bespoke code. | $1.0$ | **7 / 10** | [ ___ / 10 ] |
| **5. Trojan Horse Data Gravity** | **10**: Sits in direct path of core transactional, financial, or user flow; captures complete metadata.<br>**5**: Processes secondary batches; retains moderate analytical context.<br>**0**: Peripheral point tool; zero retained data exhaust or integration gravity. | $1.0$ | **8 / 10** | [ ___ / 10 ] |

---

## 2. Decision Logic & Qualification Thresholds

- **Total Score $\ge 40$**: **APPROVED BEACHHEAD**. High urgency, rapid sales velocity, strong expansion potential, and zero custom consulting trap.
- **Total Score $30 - 39$**: **CONDITIONAL HOLD**. Review gating vector scores. If Architectural Homogeneity or Budget is $< 7$, reject immediately.
- **Total Score $< 30$**: **DISQUALIFIED**. Market will suffer from elongated sales cycles ($> 12$ months), low willingness to pay, and high churn.

---

## 3. Disqualification Veto Triggers

Regardless of total score, an entry market is **immediately vetoed** if any of the following conditions exist:
1. **The Custom Code Trap**: Serving the account requires deploying bespoke branches or client-specific compiled code (violating Rule 3).
2. **Diffuse Decision Authority**: Closing a contract requires consensus from more than two independent business units before initial deployment.
3. **Absence of a Quantifiable Downside**: The customer cannot articulate a concrete dollar amount lost when the status quo fails.
