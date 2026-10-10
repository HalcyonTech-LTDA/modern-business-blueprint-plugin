# P&L & Unit Economics Audit Worksheet

Use this quantitative worksheet and red-flag audit checklist to stress-test any company conception financial model before presenting to an institutional investment committee.

---

## 1. Quantitative Input Worksheet

```markdown
### A. Top-Line Metrics
- Contracted Base Platform Fee (Annual):           $[ _______ ]
- Monitored Entity Fee (Annualized):              $[ _______ ]
- Programmatic Usage Volume (Annualized):         $[ _______ ]
- High-Margin Derived Data Fees (Annualized):     $[ _______ ]
--------------------------------------------------------------
TOTAL ANNUAL RECURRING REVENUE (ARR):             $[ _______ ]

### B. Direct COGS Breakdown
- Cloud Hosting & Compute Infrastructure:         $[ _______ ]
- Upstream Third-Party Data Provider Feeds:       $[ _______ ]
- Customer Reliability Ops & SLA Support:         $[ _______ ]
- Direct Network / Egress / Encryption Costs:     $[ _______ ]
--------------------------------------------------------------
TOTAL COST OF GOODS SOLD (COGS):                  $[ _______ ]

### C. Gross Profit & Margins
- Gross Profit ($) = Total ARR - Total COGS:       $[ _______ ]
- Blended Gross Margin %:                         [ _______ ]%  (Target: >= 75-85%)
- Software Gross Margin %:                        [ _______ ]%  (Target: >= 85-90%)

### D. Customer Acquisition & Economics
- Total Annualized S&M Budget:                    $[ _______ ]
- New Enterprise Logos Acquired per Year:         [ _______ ]
- Blended Fully Loaded CAC:                       $[ _______ ]
- Initial Average Contract Value (ACV):           $[ _______ ]
- CAC Payback Period (Months):                    [ _______ ] mo (Target: <= 12 mo)
- Projected Annual Net Revenue Retention (NRR):   [ _______ ]%  (Target: >= 120-130%)
- Projected Annual Gross Logo Churn:              [ _______ ]%  (Target: <= 5%)
- Estimated LTV ($):                              $[ _______ ]
- LTV / CAC Ratio:                                [ _______ ]x  (Target: >= 3.0x - 5.0x)

### E. Infrastructure Guardrail Ratios
- (Cloud COGS + Data COGS) / Total Revenue:        [ _______ ]%  (Target: <= 15-20%)
- Monthly Net Cash Burn:                          $[ _______ ]
- Ending Cash on Balance Sheet:                   $[ _______ ]
- Zero Cash Date (Runway in Months):              [ _______ ] mo (Target: 12-18 mo)
```

---

## 2. Institutional VC Red-Flag Audit Checklist

Mark `[PASS]` or `[FAIL]` against each institutional hurdle:

- [ ] **Data Reseller Red Flag**: Are third-party data fees bundled into subscription revenue without distinct COGS isolation? *(PASS = Segregated; FAIL = Blended)*
- [ ] **Gross Margin Threshold**: Is the 24-month projected gross margin $\ge 75\%$? *(PASS $\ge 75\%$; FAIL $< 75\%$)*
- [ ] **CAC Payback Velocity**: Is the CAC payback period $\le 12\text{ months}$ based on gross margin dollars? *(PASS $\le 12\text{m}$; FAIL $> 12\text{m}$)*
- [ ] **Retention Compounding**: Is NRR modeled at $\ge 120\%$ through verifiable operational drivers (entity growth or module expansion)? *(PASS $\ge 120\%$; FAIL $< 120\%$)*
- [ ] **Infrastructure Ratio**: Does the direct cloud and data vendor cost remain $\le 20\%$ of total revenue? *(PASS $\le 20\%$; FAIL $> 20\%$)*
- [ ] **Runway Discipline**: Does the current round provide $\ge 12 - 18\text{ months}$ of runway to extinguish the designated risk gate? *(PASS $\ge 12\text{m}$; FAIL $< 12\text{m}$)*
- [ ] **Headcount Pacing**: Is hiring strictly gated by verified ARR milestones rather than prospective fundraising? *(PASS = Milestone-Gated; FAIL = Calendar-based)*
