# Horizontal Core Engine vs Configurable Solutions: The Scalability Invariant

This reference defines the architectural pattern that enables enterprise B2B infrastructure to deliver deeply tailored customer outcomes while strictly maintaining a single, unified, scalable codebase (**Rule 3: Constraint**).

---

## The Fatal "Consulting Trap" in Enterprise B2B

Many enterprise startups suffer from the "Consulting Trap":
1. An enterprise customer offers a large $250k contract, but demands: *"Can you customize your data parser for our custom internal schema, change your algorithm to match our legacy calculation, and add custom UI screens for our risk team?"*
2. The engineering team agrees, writing bespoke code in the core repo or spinning up a custom deployment branch.
3. Soon, each enterprise customer runs a divergent fork.
4. Product velocity collapses to zero because every update breaks five customer-specific branches. Gross margins collapse from 80% to 35% because engineers spend all their time on maintenance and custom professional services.

---

## The Architectural Solution: Two-Layer Decoupling

```
┌────────────────────────────────────────────────────────────────────────┐
│                      CONFIGURABLE SOLUTION LAYER                       │
│                                                                        │
│  [YAML / JSON Declarative Schemas]                                     │
│  ├── Domain Entity Definitions (Fields, Types, Normalizations)         │
│  ├── Rule & Policy Logic (Declarative Expressions & Boolean Trees)     │
│  ├── Workflow State Machines (States, Triggers, SLA Deadlines)         │
│  └── Connector Configs (Authentication, Endpoints, Mapping Rules)      │
└───────────────────────────────────┬────────────────────────────────────┘
                                    │ Evaluated dynamically at runtime
                                    ▼
┌────────────────────────────────────────────────────────────────────────┐
│                   IMMUTABLE HORIZONTAL CORE ENGINE                     │
│                                                                        │
│  ├── Ingestion & Message Pipeline (High-throughput streaming bus)      │
│  ├── Generalized Rule Evaluation Runtime (Compiled DAG interpreter)   │
│  ├── Graph Database & Context Index (Immutable relationship nodes)     │
│  ├── Cryptographic Audit Engine (Tamper-evident append-only ledger)    │
│  ├── Multi-Tenant Orchestration (KMS key per tenant, VPC isolation)    │
│  └── Telemetry & Metering Service (Usage billing & SLA monitoring)    │
└────────────────────────────────────────────────────────────────────────┘
```

---

## Technical Invariants for Configurable Solutions

### Invariant 1: Declarative Schema-Driven Customization
- All domain-specific logic must be expressed as declarative configuration (YAML, JSON, or DSL) rather than compiled procedural code.
- Customizations are stored as tenant-specific configuration assets in the database, not code in Git.
- An update to the platform engine automatically benefits all tenants without breaking existing configurations.

### Invariant 2: Standard Connector Manifests
- Data integrations must be handled via standardized connector specifications.
- Instead of writing bespoke code to ingest Customer X's bespoke transaction feed, the platform provides a configurable **Data Normalization Adapter**:
  ```yaml
  connector: kafka-stream
  topic: raw-payments-v1
  mappings:
    transactionId: payload.tx_ref_id
    amount: payload.financials.cents / 100
    currency: payload.financials.iso_curr
    timestamp: payload.meta.processed_at
  ```
- Adding a new connector or mapping requires zero engineering deploys.

### Invariant 3: Sandboxed Logic Execution
- When complex calculations are required that exceed standard boolean rules, they must run inside isolated, sandboxed execution runtimes (e.g., WebAssembly / V8 isolates or sandboxed Python engines) with strict memory and CPU quotas.
- Customer-provided scripts can never crash the core engine or leak data across tenant boundaries.

### Invariant 4: Continuous Productization of Customer Requests
- When a customer requests a feature that cannot be configured with existing schemas:
  - The VP of Product evaluates whether this capability represents a generalizable pattern needed by 80% of enterprise accounts.
  - If yes, engineering builds the generic capability into the core engine or configuration schema compiler.
  - If no, the request is politely declined. The customer may use external webhooks or APIs to perform their unique proprietary calculation downstream.
