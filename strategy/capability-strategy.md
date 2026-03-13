# Data Observability — Solution Strategy (2026)

> **Owner:** Hermann Hans — Product Lead, Data Observability  
> **Solution:** Business Observability  
> **Capability:** Business Data Experience (BDX)  
> **Last updated:** 2026-02-23  
> **Sources:** Distilled from `FY27_Data_Observability_Business_Plan.md`, `dynatrace-data-observability-vision.md`, `PRODUCT-16280-action-plan.md`, and `DYNATRACE-STRATEGY.md`.

---

## Vision & Positioning

- **Vision:** Unified observability for the modern data platform — where data pipelines are **first-class citizens** alongside applications and infrastructure.
- **Differentiator:** **Platform convergence** (Grail + Smartscape topology + Davis AI causal RCA) → one platform for apps, infra, and data — not another point solution. **definity.ai partnership** for deep Lakehouse/Spark specialization → speed without build-from-scratch risk.
- **North Star:** When a data pipeline fails, the team sees the failure, the root cause, the downstream app/AI impact, and the fix path — in one place, powered by one AI.

---

## Platform Strategy Alignment (non-negotiables)

Data Observability must be compatible with the Dynatrace platform direction:

- **Collection-agnostic value via data contract:** requirements specify fields/semantics + desired outcomes, not "must be OneAgent." Support extension-based, API-based, and OpenTelemetry/OpenLineage collection.
- **OpenPipeline as enforcement point:** pipeline telemetry flows through central mapping/enrichment/routing/governance — we don't bypass it.
- **Smartscape integration:** data pipelines become first-class topology entities with dependency edges to applications, infrastructure, and consumers.
- **Unified tagging:** primary Grail fields + primary tags for routing, permissions, segmentation, and cost attribution.
- **Davis AI at scale:** pipeline anomalies feed into causal AI for cross-domain root cause analysis — not siloed alerting.

---

## Strategy Themes (2026)

### 1) Data Pipeline & Platform Observability (foundational)
- **Execution visibility** for Spark/Databricks, Snowflake, Airflow, dbt, Azure Data Factory — job status, duration, failures, retries, resource utilization
- **Pipeline topology** in Smartscape — DAG visualization, dependency mapping, impact analysis from data source → transformation → storage → application
- **Cost & performance** — credit consumption, cluster utilization, cost attribution by team/pipeline, optimization recommendations
- **Why now:** Highest customer pain point; 831 existing DT customers already use target data platforms; direct competitive response to Datadog DJM/DSM

### 2) Data Quality & Freshness (trust layer)
- **Anomaly detection** — freshness delays, volume spikes/drops, unexpected null rates, schema drift
- **Data profiling** — distributions, completeness, accuracy baselines
- **Lineage context** — trace quality issues to source transformations via OpenLineage + Smartscape
- **Why now:** 35% of AI projects stall on data quality issues; regulatory pressure (GDPR, HIPAA, AI ethics); Datadog/Monte Carlo already positioning here

### 3) AI Observability Foundation (strategic narrative)
- Data pipelines as the **supply chain for AI** — pipeline failures cause model drift, stale training data, hallucination risk
- **Data Observability is the prerequisite for AI Observability** — you can't trust AI if you can't trust the data feeding it
- Cross-link with AI Observability Solution for joint GTM, shared personas, and unified customer narrative
- **Why now:** Datadog has pitched data obs as part of their AI narrative for 18+ months; FY27 MCGs will elevate AI Observability further; our AI story needs the data layer

### 4) definity.ai Partnership & Integration (acceleration path)
- **Phase 0 (now):** Joint GTM — co-sell to ~70-80 overlapping customers, validate demand, 10 deals target
- **Phase 1:** Extension-based integration — definity.ai Databricks telemetry → Grail ingestion, Hub listing, dashboards/alerts
- **Phase 2:** Smartscape + Davis correlation — data pipelines as first-class entities with causal RCA
- **Phase 3:** Data Observability App — native Dynatrace experience, estate-wide monitoring
- **Build vs. Partner matrix:** definity.ai for Databricks depth; Dynatrace builds Snowflake, Kafka, dbt, Airflow, schema/quality detection, Davis AI, and Smartscape integration (see `datadog-gap-assessment.md`)

---

## MCG Alignment

Every piece of work must map to at least one FY26 Mission Critical Goal:

| MCG | How Data Observability Serves It |
|-----|--------------------------------|
| **MCG 1 — 3rd Gen Completeness & Adoption** | Pipeline telemetry in Grail = new 3rd gen data surface; pipeline entities in Smartscape = new topology; Davis correlation with pipeline anomalies = new AI surface area |
| **MCG 2 — Cloud-Native Workload Expansion** | Databricks/Spark/Snowflake on hyperscalers; data pipelines as AI supply chain; developer-adjacent entry points for data engineers |
| **MCG 3 — Log Monitoring & Analytics** | (Indirect) Pipeline logs and events flow into Grail, supporting consolidation narrative and OpenPipeline adoption |
| **MCG 4 — Drive Consumption** | New use case = new Grail ingestion = incremental DPS; new buyer personas (Raj, Maria); partnership-influenced pipeline |

---

## Target Personas

| Persona | Role | We Reach Them Today? | Buying Role |
|---------|------|---------------------|-------------|
| **Jennifer** | Platform Engineering Lead | Yes — existing DT buyer | Expansion sponsor |
| **Raj** | Data (Reliability) Engineer — IC/Manager | **No** — new persona | Evaluator, POC champion, technical influencer |
| **Maria** | Head of Data Platform — Director/VP | **No** — new decision-maker | Budget holder, decision maker |

**Key insight:** Raj and Maria are **not variants of existing personas** — they are a genuinely new buyer we don't reach today. GTM, sales enablement, and CAB composition must account for this.

---

## Operating Principles

- **Consumption-first** prioritization — bias toward outcomes that drive DPS ingestion, WAU/DAU, and time-to-first-value
- **Partner-aware** execution — every decision checks the build-vs-partner matrix; definity.ai integration milestones are first-class commitments
- **Phase-gated** delivery — green/amber/red criteria at each phase gate; kill criteria exist and are respected (see `PRODUCT-16280-action-plan.md` Appendix B)
- **Evidence over speculation** — ground metrics in field validation, not spreadsheet models; ground competitive claims in actual product docs
- **AI Observability narrative** — always frame data observability as foundational to AI workload reliability, not just "pipeline monitoring"

---

## Competitive Positioning

### vs. Datadog (primary threat)
- **Their move:** Acquired Metaplane (2025); shipping DJM, DSM, warehouse visibility, data quality
- **Their gap:** Data in isolation — no causal RCA across data + apps + infra; no automatic topology; cost surprises at scale
- **Our play:** Unified platform (Smartscape + Davis) → "Datadog shows you the data. Dynatrace tells you the answer."

### vs. Monte Carlo / Point Solutions
- **Their strength:** Established in data quality; strong mindshare with data teams
- **Their gap:** Data pipelines only — no app/infra context; no causal AI; separate from SRE workflows
- **Our play:** Breadth + full-stack context → "Point solutions see pipelines. Dynatrace sees the business."

### vs. Build-in-house
- **Customer reality:** Many teams run homegrown monitoring (custom Slack alerts, notebooks, Airflow UI)
- **Their gap:** Brittle, manual, no cross-domain correlation, no standardization
- **Our play:** Out-of-the-box value with zero-config deployment → "Stop building observability. Start using it."

---

## Financial Targets (directional)

| Year | ARR Target | Key Driver |
|------|-----------|------------|
| **FY27** | ~$0.4M | Design partners, early POCs, internal validation |
| **FY28** | ~$3-4M | Snowflake + Databricks monitoring GA; first enterprise deals |
| **FY29** | ~$17M | Orchestration (dbt, Airflow) + data quality + upsell |
| **FY30** | ~$49M | Mainstream adoption; replaces standalone tools in large deals |

---

## Risks & Mitigations

| Risk | Mitigation |
|------|-----------|
| **definity.ai viability** (8-person startup, Series A) | Cross-phase kill switch; maintain lightweight "build alternative" assessment at each gate |
| **New persona GTM** (Raj/Maria not in current sales motion) | Joint enablement with AI Observability team; careful CAB vetting for data personas; sales playbook before Phase 0 calls |
| **Cross-team dependencies** (Smartscape, Davis, Grail, Hub) | Dependency map (PRODUCT-16280 Action 3 — in progress); named owners + capacity confirmation before Phase 1 |
| **Competitive timing** — Datadog ships faster | Phase 0 validates with customers now; definity.ai partnership accelerates Databricks coverage; Snowflake built in parallel |
| **Pricing model unclear** | Initiate pricing/packaging discussions with Growth team in Q1 (meeting notes: 2026-02-23 alignment call) |

---

## What This Strategy Does NOT Cover

- **Detailed roadmap with milestones** → see `DATA-OBS-ROADMAP.md` (coming)
- **Team structure and RACI** → see `DATA-OBS-TEAM.md` (coming)
- **Implementable requirements** → see Value Increments (to be created under `issues/`)
- **Full business case with market sizing** → see `FY27_Data_Observability_Business_Plan.md`
