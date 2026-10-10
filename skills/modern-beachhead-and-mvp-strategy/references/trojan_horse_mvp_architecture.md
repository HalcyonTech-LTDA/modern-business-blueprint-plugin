# Trojan Horse MVP Architecture: Engineering the Wedge

This reference outlines the technical and product architecture required to design an enterprise MVP that solves an acute operational pain while establishing the persistent data and integration gravity necessary for platform expansion.

---

## The Trojan Horse Paradigm

A "Trojan Horse MVP" differs fundamentally from a traditional startup prototype:
- **Traditional MVP**: A lightweight, stripped-down application built to test whether users like a concept. Frequently superficial, isolated from core systems, and easily discarded.
- **Trojan Horse MVP**: An enterprise-grade surgical component designed to sit directly on the enterprise's mission-critical transaction highway. It is small in functional scope, but deep in integration depth.

```
                    ENTERPRISE INFRASTRUCTURE
┌─────────────────────────────────────────────────────────────────┐
│ Upstream Event Source (Core Ledger / Gateway / Data Lake)       │
└───────────────────────────────┬─────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────┐
│ [TROJAN HORSE MVP: THE CRITICAL-PATH WEDGE]                     │
│  - Ultra-low latency execution of single high-stakes transform  │
│  - Read/Write hooks into core transaction flow                  │
│  - Captures complete operational metadata & context exhaust     │
└───────────────────────────────┬─────────────────────────────────┘
                                │
         ┌──────────────────────┴──────────────────────┐
         ▼                                             ▼
┌─────────────────────────────┐           ┌─────────────────────────────┐
│ Downstream Operational Bus  │           │ PERSISTENT DATA GRAVITY     │
│ (Approved Action / Verdict) │           │ (Audit Graph / Context)     │
└─────────────────────────────┘           └──────────────┬──────────────┘
                                                         │
                                                         ▼
                                          ┌─────────────────────────────┐
                                          │ EXPANSION TERRITORY         │
                                          │ (Adjacent Modules 2, 3, 4)  │
                                          └─────────────────────────────┘
```

---

## Architectural Rules for the Trojan Horse Wedge

### 1. Ingress Point Placement (High-Leverage Interception)
The wedge must hook into an architectural bottleneck where telemetry cannot be bypassed:
- **API Proxy / Middleware Gateway**: Intercepting incoming RPC/HTTP requests before they hit legacy databases.
- **Event Streaming Consumer**: Tapping directly into Apache Kafka, AWS Kinesis, or Azure Event Hubs topic streams.
- **CDC (Change Data Capture) Stream**: Monitoring database state changes via Debezium/Kafka Connect.

### 2. Zero-Disruption Fail-Open / Fallback Design
Enterprise buyers are terrified that new software will cause systemic outages:
- The wedge must support an initial **"Shadow Mode" (Passive Ingestion)** where it evaluates live traffic concurrently with the legacy system without impacting production SLA latency.
- It must feature deterministic fail-open semantics: if the wedge encounters an unhandled exception, production traffic continues uninterrupted while telemetry logs the fault.
- This architecture enables 10-minute security approvals and eliminates months of integration paralysis.

### 3. Separation of Horizontal Core Engine from Vertical Configuration

```
┌─────────────────────────────────────────────────────────────────┐
│               CONFIGURABLE SOLUTION LAYER (YAML/JSON)           │
│  - Beachhead Rule Set & Policy Thresholds                       │
│  - Vertical Data Normalization Schemas (e.g. ISO 20022 / FHIR)  │
│  - Domain-Specific Notification & Webhook Handlers              │
├─────────────────────────────────────────────────────────────────┤
│               IMMUTABLE HORIZONTAL CORE ENGINE                  │
│  - High-Throughput Stream Ingestion (Zero-Copy Serialization)   │
│  - Deterministic Evaluation & Rule Graph Execution Engine       │
│  - Cryptographic Append-Only Audit Trail                        │
│  - Tenant Isolation, KMS Encryption & Strict RBAC               │
└─────────────────────────────────────────────────────────────────┘
```

- **Rule 3 Enforcement**: The core engine code is 100% agnostic to the customer's industry. All customer-specific logic is declared via schemas.
- If a customer demands a unique feature, it must be evaluated:
  - Can this feature be expressed as a generic configuration attribute in the schema?
  - If yes, implement it in the configuration compiler.
  - If no, reject it. Never fork the repository or maintain custom client branches.

### 4. Telemetry Exhaust and Expansion Anchors
Every execution of the MVP must persist structured metadata into an internal context store:
- **Entity Identity Graph**: Who was involved in the transaction?
- **Decision Context**: What rules fired, why, and what was the historical pattern?
- **Outcome Telemetry**: What was the subsequent downstream business impact?

This accumulated data exhaust creates the foundational dataset required to unlock the next product modules (e.g., continuous anomaly detection, predictive risk scoring, automated dispute resolution).
