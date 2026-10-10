# Replicable Customer Success & Onboarding: The Anti-Consulting Playbook

This reference establishes the standardized 30-day enterprise onboarding methodology that delivers rapid Time-to-Value (TTV) while strictly protecting gross margins and eliminating open-ended custom consulting (**Rule 3: Constraint**).

---

## The Danger of Custom Consulting in Customer Success

In enterprise software, low-margin professional services and open-ended "integration consulting" destroy company valuation:
- Custom integration consulting ties revenue growth directly to billable headcount.
- Customer Success becomes a reactive software customization shop rather than a scalable adoption engine.
- Deployments drag on for 9 to 18 months, delaying revenue recognition, frustrating executive sponsors, and increasing pre-revenue churn.

The goal of Modern Enterprise Customer Success is **Replicable Mechanical Onboarding**: transitioning every customer from signed contract to live, value-generating production in $\le 30$ business days using declarative configuration runbooks.

---

## The 30-Day Replicable Integration Schedule

```
┌────────────────────────────────────────────────────────────────────────┐
│ WEEK 1: SANDBOX PROVISIONING & DATA MAPPING                            │
│  - Automated tenant provisioning (Dedicated KMS key & VPC endpoint)    │
│  - Standardized JSON/YAML connector mapping via self-serve schema      │
│  - Ingestion of test synthetic transaction stream                      │
├───────────────────────────────────┬────────────────────────────────────┘
                                    │
                                    ▼
┌────────────────────────────────────────────────────────────────────────┐
│ WEEK 2: PASSIVE SHADOW MODE & PARALLEL RUN                             │
│  - Tap live production event stream in passive read-only shadow mode   │
│  - Concurrently evaluate traffic alongside customer's legacy system    │
│  - Automated variance reporting (Latency, False Positives, Misses)    │
├───────────────────────────────────┬────────────────────────────────────┘
                                    │
                                    ▼
┌────────────────────────────────────────────────────────────────────────┐
│ WEEK 3: PRODUCTION CUTOVER & SECURITY CLEARANCE                        │
│  - Verify 99.9% SLA uptime and < 30ms latency benchmarks               │
│  - Enable active writeback hooks into downstream core transaction bus   │
│  - Formal Sign-off from Chief Information Security Officer (CISO)      │
├───────────────────────────────────┬────────────────────────────────────┘
                                    │
                                    ▼
┌────────────────────────────────────────────────────────────────────────┐
│ WEEK 4: EXECUTIVE VALUE REALIZATION REVIEW                             │
│  - Deliver 30-Day Quantified ROI Report to the Economic Buyer          │
│  - Validate reduction in analyst hours and false positive drops        │
│  - Establish baseline telemetry metrics for Month 6 Modular Expansion │
└────────────────────────────────────────────────────────────────────────┘
```

---

## Core Invariants for Scalable Onboarding

### 1. The Declarative Configuration Runbook
- Every customer receives the identical **Standard Implementation Package**:
  - Pre-built OpenAPI specifications and Kafka topic consumers.
  - Pre-tested policy templates corresponding to their regulatory jurisdiction.
  - Automated smoke test suites that validate data mapping within 300 seconds.
- No software engineer is ever assigned to write client-specific production adapters. If a customer has an unusual internal data format, they map it using the platform's declarative transformation engine or normalize it on their side before sending.

### 2. Guardrails Against Professional Services Creep
- Contracts must explicitly limit onboarding support to a defined scope (e.g., "Up to 20 hours of Solutions Architecture guidance over 30 days").
- Any customer request for bespoke software development, manual data migration, or on-site staff augmentation is answered with:
  *"Our architecture is designed as a high-performance horizontal standard. We provide certified third-party systems integrator partners (e.g., Slalom, Accenture) if your organization requires dedicated external staff."*

### 3. Automated Health & Expansion Telemetry
Customer Success monitors account health through programmatic system metrics, not subjective phone check-ins:
- **Telemetry Metric 1 (Consumption Velocity)**: Daily transaction ingestion volume relative to contractual tier.
- **Telemetry Metric 2 (Execution Latency)**: P99 processing speed at the customer endpoint.
- **Telemetry Metric 3 (User Engagement)**: Weekly active users reviewing flagged exception cases.
- If usage falls below 70% of baseline, an automated triage alert routes to the Solutions Architect within 2 hours.
- If usage exceeds 85% of baseline, an automated expansion alert routes to the Account Executive.
