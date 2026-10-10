# Unit Economics & P&L Case Study: "Vortex Ledger"

This case study demonstrates the multi-year P&L trajectory and quantitative unit economics model for **Vortex Ledger** (Continuous Decision Intelligence Infrastructure for financial crime and sanctions screening).

---

## 1. 3-Year Consolidated Statement of Operations (P&L)

All figures in thousands of USD ($000s):

| Financial Line Item | Year 1 (Seed / Validation) | Year 2 (Commercialization) | Year 3 (Scale Expansion) |
| :--- | :--- | :--- | :--- |
| **REVENUE** | | | |
| 1.1 Software Platform License ARR (Layer 1) | $450 | $2,250 | $6,800 |
| 1.2 Continuous Entity Monitoring ARR (Layer 2) | $180 | $1,120 | $4,150 |
| 1.3 Usage & Metered Execution Fees (Layer 3) | $90 | $480 | $1,750 |
| 1.4 Derived Data Intelligence Fees (Layer 4) | $0 | $150 | $1,100 |
| **TOTAL REVENUE** | **$720** | **$4,000** | **$13,800** |
| | | | |
| **COST OF GOODS SOLD (COGS)** | | | |
| 2.1 Cloud Hosting & Compute (AWS EKS, Kafka) | $110 | $380 | $920 |
| 2.2 Third-Party Data Provider Feeds (Watchlists) | $75 | $240 | $510 |
| 2.3 Customer Reliability Ops / 24/7 SLA Delivery | $45 | $180 | $460 |
| **TOTAL COST OF GOODS SOLD** | **$230** | **$800** | **$1,890** |
| | | | |
| **GROSS PROFIT** | **$490** | **$3,200** | **$11,910** |
| **Blended Gross Margin %** | **68.1%** | **80.0%** | **86.3%** |
| **Software Gross Margin %** | **75.4%** | **83.6%** | **89.5%** |
| | | | |
| **OPERATING EXPENSES (OPEX)** | | | |
| 3.1 Research & Development (Engineering & Core) | $1,100 | $2,100 | $4,200 |
| 3.2 Sales & Marketing (AE Pods, Whitepapers, T&E)| $420 | $1,450 | $3,900 |
| 3.3 General & Administrative (Legal, Compliance) | $260 | $650 | $1,400 |
| **TOTAL OPERATING EXPENSES** | **$1,780** | **$4,200** | **$9,500** |
| | | | |
| **OPERATING INCOME / (LOSS) (EBIT)** | **($1,290)** | **($1,000)** | **$2,410** |
| **Ending Cash Balance** | $1,710 | $4,710 | $12,120 |
| **Total Capital Raised (Cumulative)** | $3,000 (Seed) | $7,000 (Series A) | $7,000 (Self-sustaining; optional Gate 4 Series B of $22M for hyper-growth scale) |

---

## 2. Quantitative Unit Economics Model & KPI Dashboard

### Customer Cohort Metrics (Enterprise Segment)

```
Average Contract Value (Initial ACV):           $85,000 / year
Blended Gross Margin % (Year 2):                80.0%
Annual Gross Contribution per Logo:             $85,000 * 0.80 = $68,000

Fully Loaded Customer Acquisition Cost (CAC):
- Sales Pod Allocation (1 AE + 0.5 FDSA):       $42,000
- Content, Technical Roundtables, T&E:          $14,000
- Legal Drafting & Contract Negotiation:        $6,000
- Marketing Ops & Tools Allocation:             $3,000
Total Fully Loaded CAC per Logo:                $65,000

CAC Payback Period Calculation:
CAC Payback = ($65,000 / $68,000) * 12 months = 11.47 months [HURDLE MET: <= 12 months]

Net Revenue Retention (NRR) Trajectory:
- Year 1 -> Year 2 Cohort Expansion:           124% NRR
- Year 2 -> Year 3 Cohort Expansion:           132% NRR
Driven by: +18% Monitored Entity growth + Module 2 AML Monitoring step-up.

Customer Lifetime Value (LTV):
- Annual Logo Churn:                           4.0% (Implied 25-year lifetime, conservatively modeled on a 5-year evaluation horizon)
- 5-Year Net Lifetime Revenue per Customer:    $85,000 * 1.25^3 * 0.80 = $385,000
- LTV / CAC Ratio (5-Year Horizon):            $385,000 / $65,000 = 5.92x [HURDLE MET: >= 3.0x - 5.0x]

Cloud & Data Cost per Revenue Ratio:
- Year 1: ($110k + $75k) / $720k = 25.7% (Pre-optimization)
- Year 2: ($380k + $240k) / $4,000k = 15.5% [HURDLE MET: <= 20%]
- Year 3: ($920k + $510k) / $13,800k = 10.4% [HURDLE MET: <= 15%]
```

---

## 3. Margin Expansion Drivers Over 36 Months

1. **Volume Tiering with Cloud Infrastructure**: AWS enterprise discount program and graviton instance switching reduce compute unit cost by $38\%$.
2. **Local Caching & Pre-Filtering**: $68\%$ of watchlist lookups resolved locally in memory in $< 5\text{ms}$, avoiding third-party per-query API egress charges.
3. **Layer 4 Derived Data Growth**: Anonymized cross-client consortium fraud risk score module scales to $\$1.1\text{M}$ ARR at $94\%$ gross margin, pulling up total company blended gross margin from $68.1\%$ to $86.3\%$.
