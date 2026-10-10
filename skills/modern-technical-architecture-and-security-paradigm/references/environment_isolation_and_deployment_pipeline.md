# Environment Isolation & Deployment Pipeline Standards

## 1. The Multi-Stage Isolation Mandate

In enterprise-grade B2B infrastructure, environmental cross-contamination (e.g., test scripts touching production records, developers debugging with real customer PII on laptops) creates catastrophic compliance violations (GDPR, LGPD, SOC 2) and risks operational outages.

### Three Isolated Tiers:

| Environment | Purpose | Data Source | Network & Access Boundary | Promotion Requirement |
| :--- | :--- | :--- | :--- | :--- |
| **Development (Dev)** | Local & cloud-based feature development, unit testing, continuous integration. | 100% synthetic, procedurally generated mock fixtures. Zero production PII. | Ephemeral or shared non-production VPC. Developer-accessible via standard IAM. | PR review + automated lint/unit tests pass. |
| **Staging (Staging)** | Production-identical pre-release verification, load testing, integration with sandbox partner APIs. | High-fidelity sanitized fixtures; schema identical to production. | Fully isolated VPC mirroring production CIDR/topology. No public ingress except VPN/bastion. | All automated integration & contract tests pass + CISO/CTO sign-off. |
| **Production (Prod)** | Live customer tenant execution, real-world data processing, business transactions. | Live customer operational data and cryptographic ledgers. | Air-gapped VPC; default-deny ingress/egress. Zero direct developer SSH/database access. | Automated canary deployment via GitOps pipeline. |

---

## 2. GitOps & Trunk-Based Deployment Discipline

### Non-Negotiable Deployment Invariants:
1. **Ban on ClickOps**: Manual configuration changes in the cloud console or direct terminal manipulations on production servers are strictly prohibited.
2. **Infrastructure as Code (IaC)**: 100% of cloud resources, networking rules, security groups, and IAM policies must be declared declaratively in version-controlled templates (Terraform, OpenTofu, Bicep) stored in the primary infrastructure repository.
3. **Immutable Artifacts**: The exact container image (tagged with git commit SHA and verified cryptographic digest) tested and approved in Staging must be the identical image promoted to Production. Re-compiling or re-building artifacts between environments is banned.
4. **Automated Promotion Pipeline**:

```
[Developer PR Branch]
         │
         ▼
[Automated CI Quality Gate]
  ├── Static Code Analysis & Linting
  ├── Secret Scanning (prevent API key leaks)
  ├── Unit & Mutation Testing (100% pass)
  └── Container Vulnerability Scan (Trivy / Grype)
         │
         ▼
[Merge to Main / Trunk] ──> Automated Deploy to Staging
         │
         ▼
[Staging Verification Suite]
  ├── End-to-End Contract Testing
  ├── Performance & Latency Benchmark
  └── Automated Smoke Tests
         │
         ▼
[Production Promotion Gate]
  ├── Cryptographic Artifact Verification
  ├── Zero-Downtime Rolling / Canary Deploy
  └── Healthcheck Verification (Automated Rollback on Error)
```

---

## 3. Production Access & Secrets Governance

1. **Zero Standing Privileges**:
   - Engineers have read-only access to centralized, anonymized production logs (e.g., via Datadog, Grafana Loki, or CloudWatch) with sensitive PII automatically masked at ingestion.
   - Database credentials, API tokens, and private encryption keys are injected strictly at container runtime via centralized secret vaults (AWS Secrets Manager, HashiCorp Vault, Azure Key Vault) using short-lived credentials.
2. **Break-Glass Emergency Protocol**:
   - In catastrophic production incidents requiring live triage, engineers must request time-limited "break-glass" access.
   - Access requires dual-authorization (CTO or designated Lead Engineer), is capped at 60 minutes, and logs every keystroke and session command to an immutable audit ledger reviewed in the subsequent monthly executive meeting.
