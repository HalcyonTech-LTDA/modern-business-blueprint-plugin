# Security Readiness & Vendor Assessment Checklist

This scorecard serves as an institutional pre-flight audit for the Corporate Architect Agent to verify SOC 2 Type II / ISO 27001 readiness, enterprise security posture, and vendor independence before engaging enterprise buying committees.

---

## 1. Enterprise Security Readiness Scorecard

| Domain | Control Specification | Target Standard | Status | Verification Evidence |
| :--- | :--- | :--- | :--- | :--- |
| **Cryptography** | Encryption at Rest | AES-256-GCM across all block, object, and database volumes. | Mandatory | KMS configuration & volume policy audit |
| **Cryptography** | Encryption in Transit | TLS 1.3 enforced on public endpoints; mTLS on inter-service traffic. | Mandatory | SSL Labs A+ rating, ingress TLS cipher profile |
| **Cryptography** | Key Management | KMS envelope encryption with automated 90-day rotation; no raw keys in code. | Mandatory | AWS/GCP KMS key rotation log |
| **Identity & Access** | MFA Enforcement | Hardware/FIDO2 MFA enforced on 100% of engineering & administrative accounts. | Mandatory | Okta / Google Workspace policy export |
| **Identity & Access** | Principle of Least Privilege | RBAC/ABAC role definitions with zero wildcard permissions (`*`). | Mandatory | IAM policy analyzer report |
| **Environment** | Boundary Isolation | Strict physical/VPC separation between Dev, Staging, and Prod. | Mandatory | Cloud VPC routing table & peering audit |
| **Environment** | Production Access | Zero standing SSH/console access for developers; break-glass logging enabled. | Mandatory | Bastion/Teleport session audit logs |
| **Deployment** | Immutable Artifacts | GitOps promotion pipeline; identical container image SHA across Staging & Prod. | Mandatory | GitHub Actions / CI digest verification |
| **Deployment** | Secret Management | Centralized secret vault (Vault/KMS); zero secrets committed to Git repositories. | Mandatory | GitGuardian / TruffleHog scan report |
| **Tenancy** | Tenant Isolation | Logical data isolation via schema partitioning or Row-Level Security (RLS). | Mandatory | Multi-tenant test suite assertion logs |
| **Compliance** | Audit Logging | Immutable, append-only audit trail capturing all user and system data access. | Mandatory | CloudTrail / audit log retention configuration |
| **Disaster Recovery**| RPO & RTO | RPO $\le 15 \text{ minutes}$; RTO $\le 2 \text{ hours}$ with automated failover testing. | Mandatory | Quarterly simulated disaster recovery drill report |

---

## 2. Structural Vendor Lock-In Audit Checklist

| Architectural Layer | Portability Standard | Verification Test | Pass / Fail |
| :--- | :--- | :--- | :--- |
| **Compute / Runtime** | OCI-compliant Docker containers running on standard Kubernetes / container runner. | Can images deploy locally via `docker run` or `compose.yaml` without cloud dependencies? | Pass / Fail |
| **Database** | Standard PostgreSQL / MySQL or ANSI SQL relational engines. | Can schema and data be dumped and restored to an unmanaged local instance? | Pass / Fail |
| **Event Bus** | Kafka / Redpanda compatible protocol. | Can producers/consumers run against local Redpanda or Kafka container without SDK changes? | Pass / Fail |
| **Storage** | S3-compatible blob API. | Can object storage client target MinIO locally with zero code changes? | Pass / Fail |
| **Authentication** | OpenID Connect (OIDC) / OAuth 2.0 standard tokens. | Can identity provider be swapped (e.g., Auth0 to Keycloak/Okta) via standard OIDC metadata? | Pass / Fail |
| **Data Export** | 100% of customer data exportable in open formats (Parquet, JSON Lines, CSV). | Does customer retain automated nightly export capability? | Pass / Fail |
