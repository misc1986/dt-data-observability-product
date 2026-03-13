# Dynatrace – Organizational & Operating Model (Solutions–Capabilities)

> **Context for Data Observability Capability**  
> Simplified reference focusing on relevant Solutions, Capabilities, and collaboration patterns.  
> Source: Internal org structure documentation (simplified, names removed to prevent staleness)

---

## Executive Summary

Dynatrace organizes product development using a **Solutions–Capabilities** model:

- **Solutions** define **strategy and outcomes** for target personas and use cases (market‑facing and internal)
- **Capabilities** are **reusable technical product components** and their people, serving multiple Solutions (m:n relationship)
- **Value Creation Teams (VCTs)** are **time‑bounded**, cross‑org teams with charters to achieve measurable goals
- The **Value Creation Guide (VCG)** codifies roles, artifacts, and alignment mechanisms

**For Data Observability:** We are a **Capability** under the **Business Observability Solution**, collaborating heavily with **Platform** capabilities.

---

## Operating Model

### Solutions
- Own: **vision → key themes → value packs → value increments**
- Market‑facing (e.g., Business Observability) or internal‑facing (e.g., Platform)
- Measure: ARR/adoption (market), internal adoption/reuse (internal)

### Capabilities  
- Groupings of dev teams owning technical components and quality
- Serve multiple Solutions; balance m:n demands with feasibility and technical excellence
- Examples: Grail, OpenPipeline, Business Data Experience (Data Observability)

### Value Creation Teams (VCTs)
- Time‑scoped, chartered teams with measurable goals; disband upon completion
- Used for cross‑org initiatives requiring dedicated focus

### Governance
- **Quarterly Capability Reviews (QCRs)**: Health, priorities, improvement areas
- **Jira hierarchy**: Solution EPICs link to Capability EPICs for cross‑capability traceability
- **Steering Committee**: Resolves investment conflicts across Solutions

---

## Relevant Solutions

### Business Observability (our parent Solution)
**Scope:** Executive insights, KPI↔IT mapping, process analytics, cost & carbon monitoring, compliance analytics  
**Capabilities:** Business Analytics, **Business Data Experience (Data Observability)**  
**Why relevant:** Data Observability is a capability within this Solution

### Platform (critical dependency)
**Scope:** Platform backbone — Grail (data lake), AppEngine, AutomationEngine, OpenPipeline (PPX), Platform Services (IAM, Documents, Platform Management), Platform Apps (PAPA - Dashboards, Notebooks, Search, SmartScape)  
**Why relevant:** All Data Observability telemetry flows through Platform capabilities (Grail storage, OpenPipeline ingestion, Smartscape topology, PAPA dashboards)

### Delivery, Reliability, Security (DRS) (governance & quality)
**Scope:** SDLC guardrails, product quality/security/privacy, ops excellence  
**Key Capabilities:** QSP (Quality, Security, Privacy), SRE (Site Reliability Engineering)  
**Why relevant:** Release gates, security reviews, reliability requirements

---

## Key Platform Capabilities (Dependencies)

**Grail** — Unified data lake for all observability data; DQL query engine  
**OpenPipeline (PPX)** — Unified ingest, semantic normalization, routing for logs/metrics/traces/events  
**Platform Apps (PAPA)** — Dashboards, Notebooks, Search, **Smartscape** (topology visualization)  
**Platform Services (PS)** — IAM, tokens, documents, platform management, serverless runtime  
**Data Intelligence** — Davis AI, Copilot backend, anomaly detection, causal analysis  

**Business Analytics** — Business event analysis, KPI correlation  
**Business Data Experience (BDX)** — **Data Observability capability** (our team)  

**QSP** — Quality, Security, Privacy gates and standards  
**SRE** — Site Reliability Engineering, production operations standards

---

## Cross-Capability Dependencies

**Critical for Data Observability:**

- **OpenPipeline (PPX) ↔ Data Observability**: Pipeline telemetry flows through OpenPipeline for ingestion, normalization, and routing
- **Grail ↔ Data Observability**: All pipeline data stored in Grail; queries via DQL
- **Smartscape (PAPA) ↔ Data Observability**: Data pipelines as first-class topology entities with dependency mapping
- **Davis AI (Data Intelligence) ↔ Data Observability**: Anomaly detection, causal RCA for pipeline failures
- **Business Analytics ↔ Data Observability**: Correlate data pipeline health with business KPIs
- **QSP/SRE ↔ All**: Reliability gates, security reviews, operational standards

---

## Planning & Execution Flow

### Roadmap Flow (Value Packs → Value Increments)

1. **Ideation** — Solution defines Value Pack (problem, outcomes, KPIs, personas)
2. **Discovery** — Feasibility consultation with impacted Capabilities; architectural alignment
3. **Planning** — Value Pack broken into Value Increments; Jira linking (Solution EPIC ↔ Capability EPICs)
4. **Execution** — Demo cadence, feature flags, progress dashboards
5. **Governance** — QCRs (quarterly), Steering (as needed for conflicts)
6. **Release** — SRE for release readiness; QSP for security/privacy gates

### Key Roles

- **Solution Lead** — Vision, key themes, value packs, outcome definition
- **Product Lead/PM** — Pack definition, scope, KPIs, prioritization
- **Capability Lead** — Component roadmap, quality, feasibility, resourcing
- **Delivery Lead** — Planning & execution across teams; risk & dependency mitigation
- **Architect** — Feasibility, cross-capability design, non-functionals

### VCT (Value Creation Team) Model

- Used for cross-org initiatives requiring dedicated focus
- Charter includes: goal, KPIs, timeline, dependencies, resourcing, exit criteria
- Dissolves upon completion

---

## Contact Channels (Slack)

**Platform Capabilities:**
- `#help-grail` — Grail data lake queries and storage
- `#help-openpipeline-ppx` — OpenPipeline ingestion and processing
- `#help-dashboards-app` — PAPA Dashboards
- `#help-notebooks-app` — PAPA Notebooks
- `#help-smartscape` — Topology and entity modeling
- `#help-platform-services` — IAM, tokens, platform mgmt
- `#help-iam` / `#help-oauth` — Identity and access

**Business Observability:**
- Business Observability Solution channels (internal comms)

**Governance:**
- QSP — Quality, Security, Privacy reviews
- SRE — Reliability and operational standards

---

## Key Takeaways for Data Observability

1. **We are a Capability** (Business Data Experience) within the **Business Observability Solution**
2. **Critical dependencies**: Grail (storage), OpenPipeline (ingestion), Smartscape (topology), Davis AI (anomaly detection)
3. **Planning flow**: Value Packs → Value Increments → Capability EPICs with cross-capability linking
4. **Governance touchpoints**: QSP (security), SRE (reliability), QCR (quarterly reviews)
5. **Contact via Slack** `#help-*` channels for platform capabilities

```

