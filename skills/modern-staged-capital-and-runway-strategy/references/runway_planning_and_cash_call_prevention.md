# Runway Planning & Cash Call Prevention

In venture-backed enterprise companies, running out of money before hitting risk-extinction milestones triggers disastrous down-rounds or predatory emergency cash calls. This reference outlines the financial modeling mechanics to maintain 12-18 months of runway and prevent emergency financing traps.

---

## 1. The Mathematics of Runway & Cash Depletion

### Key Formulas:
- **Gross Monthly Burn**:
  $$\text{Gross Burn} = \text{Total Cash Outflows (Payroll + Rent + Cloud + Subscriptions + Taxes)}$$
- **Net Monthly Burn**:
  $$\text{Net Burn} = \text{Gross Burn} - \text{Cash Inflows from Customer Receipts}$$
- **Zero Cash Date (ZCD)**:
  $$\text{Runway (Months)} = \frac{\text{Cash Balance} - \text{Minimum Reserve Buffer}}{\text{Net Monthly Burn Rate}}$$

### The 6-Month Hard Floor Invariant:
- Institutional venture governance mandates a **Minimum Reserve Buffer** equal to at least **3 to 6 months of Net Operating Burn**.
- **Why**: Enterprise sales cycles take 3 to 9 months, and institutional Series A/B fundraising rounds take 4 to 6 months from initial partner pitch to cash in bank.
- If cash drops below the 6-month buffer, the company is effectively insolvent from a fundraising leverage perspective, forcing the board to seek desperate bridge financing on predatory terms.

---

## 2. Anatomy of an Emergency Cash Call (The Down-Round Trap)

When a company raises only 6-9 months of runway or ramps spending based on narrative rather than proven unit economics, it hits the "Cash Call Trap":

```
[Month 0: Raise $1.5M with 8 mo runway]
       │
       ▼
[Month 4: Product delayed by 60 days]
       │
       ▼
[Month 6: Only 2 months cash left ($300k); zero closed deals]
       │
       ▼
[THE DESPERATE CASH CALL]
       ├── Existing VCs demand Cram-Down Recapitalization
       ├── Valuation cut by 70% ($15M -> $4.5M)
       ├── Senior 3x Liquidation Preference attached
       └── Founders suffer 50%+ equity dilution in 14 days
```

### Protective Covenant: The 12-18 Month Rule
By mandating **12 to 18 months of runway per stage**, the company gains:
1. **Breathing Room for Operational Reality**: Enterprise pilots often encounter 4-week infosec reviews or budget freeze cycles. An 18-month runway absorbs these without panic.
2. **Fundraising Leverage**: Founders start Series A discussions with 7-9 months of cash in bank, allowing them to walk away from bad term sheets.
3. **Option for Self-Sufficiency**: If macro venture markets shut down, the company can trim non-essential expenses and achieve cash flow break-even on contracted ARR.

---

## 3. Headcount Pacing Governed by Unit Economics (Rule 1 Enforcement)

Premature hiring is the #1 killer of early-stage enterprise ventures. The table below details the strict unit economic authorization hurdles required before opening new headcount requisitions:

| Role / Function | Minimum Runway Required | Required Unit Economic Hurdle to Authorize Requisition |
| :--- | :--- | :--- |
| **Founding Engineers (1-2)** | 12+ Months | Gate 1 Build entry; technical architecture specification signed off. |
| **Solutions Architect / FDSA** | 12+ Months | Gate 2 Validation entry; at least 1 design partner agreement signed. |
| **Enterprise Account Executive (Pod 1)** | 15+ Months | Gate 3 Commercialization entry; $\ge 2$ design partners converted to paid ARR. |
| **Customer Success Engineer** | 14+ Months | Contracted ARR $> \$500\text{k}$; at least 5 live enterprise deployments. |
| **Enterprise Account Executive (Pod 2)** | 16+ Months | Pod 1 AE at $\ge 80\%$ quota; verified CAC Payback $\le 12\text{ months}$. |
| **Marketing / SDR Outbound Specialist** | 18+ Months | Sales capacity constrained by qualified lead volume, not closing ability. |
