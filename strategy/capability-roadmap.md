```markdown
# Data Observability — Roadmap (2026)

> **Owner:** Hermann Hans — Product Lead, Data Observability  
> **Last updated:** 2026-02-24  
> **Sources:** Reconciled from `FY27_Data_Observability_Business_Plan.md`, `datadog-gap-assessment.md`, `PRODUCT-16280-action-plan.md`, and `DATA-OBS-STRATEGY.md`.

---

## Start Here (agent index)

Use these files as the grounding set when working on roadmap items:

- Solution strategy: [DATA-OBS-STRATEGY.md](DATA-OBS-STRATEGY.md)
- Company strategy context: `software-delivery/DYNATRACE-STRATEGY.md`
- Business case (full): [FY27_Data_Observability_Business_Plan.md](FY27_Data_Observability_Business_Plan.md)
- Competitive gaps & build plan: [datadog-gap-assessment.md](datadog-gap-assessment.md)
- Primary Value Pack action plan: [valuepack/PRODUCT-16280-action-plan.md](valuepack/PRODUCT-16280-action-plan.md)
- Master folder guide: [AGENTS.md](AGENTS.md)

---

## Roadmap Overview

The roadmap has **two parallel tracks** that converge:

1. **Partnership Track** (PRODUCT-16280) — phased definity.ai integration for Databricks/Spark, follows the 4-phase model with kill criteria at each gate
2. **Build Track** — Dynatrace-built capabilities for Snowflake, data quality, orchestration, and platform integration (Smartscape, Davis)

Both tracks deliver into a single customer experience: **Data Observability as a first-class surface in Dynatrace**.

```
FY27 (Now)                    FY28                         FY29
├─── Phase 0: Joint GTM ──┤
├─── Snowflake repackage ──┤
│                          ├── Phase 1: Integration ──┤
│                          ├── Snowflake App GA ──────┤
│                          │                          ├── Phase 2: Smartscape ──┤
│                          │                          ├── Orchestration (dbt/Airflow) ──┤
│                          │                          ├── Data Quality v1 ──┤
│                          │                          │                     ├── Phase 3: DO App ──┤
│                          │                          │                     ├── DQ v2 + Lineage ──┤
```

---

## Partnership Track — definity.ai Integration (PRODUCT-16280)

### Phase 0 — Joint GTM (Months 1–3, NOW → May 2026)

**Objective:** Validate demand, enable the field, close first co-sell deals.

| Workstream | What | Owner | Status |
|-----------|------|-------|--------|
| Customer outreach | Call ~70-80 overlapping target customers (Spark-intensive DT accounts) | CSMs + AEs + definity | In progress |
| Sales enablement | Playbook, competitive battle cards, demo environment | PM (Michael) + GTM | Playbook drafted (Appendix E) |
| Target account list | Tiered list of Spark-intensive accounts by density | Product Lead (Hermann) | ✅ Done — see `analysis/spark-target-accounts.md` |
| Contracting | Partnership terms, deal structure, revenue share model | Alliances (Conor) + Legal | In progress |
| CAB formation | ≥4 design partners committed for feedback and co-design | PM + Product Lead | In progress — vetting participants |
| Pricing direction | At minimum a directional model for Phase 0 deals | Product Lead + Growth | Not started — must open with Growth team |

**Phase Gate (Month 3):**

| Signal | Green | Amber | Red |
|--------|-------|-------|-----|
| Customer demand | ≥20 discovery calls | 10–19 calls | <10 calls |
| POC conversion | ≥5 POCs started | 3–4 POCs | <3 POCs |
| Deal pipeline | ≥3 deals with committed next steps | 1–2 deals | 0 deals |
| Partner readiness | Enablement complete, contracting done | Delayed but recoverable | Structural blocker |
| Design partners | ≥4 committed | 2–3 | <2 |

_If 2+ Red at Month 3 → stop and reassess partnership thesis._

---

### Phase 1 — Initial Integration (Months 4–6, ~Jun–Aug 2026)

**Objective:** definity.ai capabilities accessible via Dynatrace — extension on Hub, pipeline telemetry in Grail, dashboards and alerts.

| Workstream | What | Owner |
|-----------|------|-------|
| Hub extension | definity.ai listed on Dynatrace Hub, installable by customers | PM + definity Eng |
| Grail ingestion | Pipeline telemetry (Spark jobs, stages, tasks, metrics) flowing into Grail | definity + Platform Eng |
| Dashboards & alerts | Out-of-the-box Databricks pipeline health dashboards, pre-configured alert rules | PM (Michael) + PX |
| Customer Zero | Internal DT teams running definity against our own Databricks environment | PM (Michael) — see Appendix D |
| POC support | Active POC management for ≥10 customers | SE team + definity |

**Phase Gate (Month 6):**

| Signal | Green | Amber | Red |
|--------|-------|-------|-----|
| Technical delivery | Extension on Hub, dashboards working by Month 5 | 4-week delay, recovery path | >6-week delay or integration blocker |
| Customer traction | ≥10 active POCs | 5–9 POCs | <5 POCs |
| DPS consumption | Measurable Grail ingestion from ≥3 customers | 1–2 customers | Zero consumption |
| Design partner feedback | Confirm value, willing to go production | Mixed but addressable | "Doesn't solve our problem" from ≥50% |
| Deal conversion | ≥5 closed deals | 2–4 deals | <2 deals |

_If Technical Delivery is Red → stop. If Traction + Deals both Red → pause Phase 2, run deep discovery sprint._

---

### Phase 2 — Smartscape + Correlation (Months 7–10, ~Sep–Dec 2026)

**Objective:** Data pipelines as first-class Smartscape entities; Davis AI correlation across data → app → user.

| Workstream | What | Owner |
|-----------|------|-------|
| Smartscape integration | Pipeline entities with dependency edges (data source → pipeline → app → user) | PA (Sebastian) + Smartscape team |
| Davis correlation | Pipeline anomalies as causal candidates in Dynatrace Problems | PA + Davis team |
| Cross-domain RCA | When app fails due to pipeline issue, root cause visible from app side | PM + PX |
| Customer expansion | Phase 1 customers upgrading to correlation capabilities | AEs + SE |

**Phase Gate (Month 10):**

| Signal | Green | Amber | Red |
|--------|-------|-------|-----|
| Smartscape integration | Pipeline entities rendering by Month 8 | Delayed to Month 10 | Smartscape team can't prioritize |
| Davis correlation | Pipeline anomalies in Problems | Partial, manual | Infeasible in current architecture |
| Customer expansion | ≥3 Phase 1 customers upgrading | 1–2 | None — Phase 1 is "good enough" |
| Competitive wins | Winning in accounts where Datadog pitches data obs | Losing some | Losing consistently |

_If Smartscape or Davis Red → cross-team dependency failure, escalate immediately. If Customer Expansion Red → reconsider Phase 3 scope._

---

### Phase 3 — Data Observability App (Months 11–15, ~Jan–May 2027)

**Objective:** Full native Dynatrace experience for data observability — estate-wide monitoring, dedicated app, new persona reach.

| Workstream | What | Owner |
|-----------|------|-------|
| DO App | Dedicated Data Observability app in Dynatrace | PM + PX + Eng |
| Estate-wide monitoring | Fleet-level views across all data pipelines, not just individual | PM + PA |
| Persona expansion | CDO/VP Data personas using the app (Maria) | GTM + PM |
| Consumption features | Cost attribution, SLA dashboards, optimization recommendations | PM + Growth |

**Phase Gate (Month 15):**

| Signal | Green | Amber | Red |
|--------|-------|-------|-----|
| App adoption | DAU/MAU >15% among data-obs customers within 8 weeks | 5–15% | <5% |
| New persona reach | CDO/VP Data in usage | Only existing DevOps/SRE | Zero new persona adoption |
| ARR contribution | Measurable ARR attributed to data obs | Pipeline exists, not closed | No attributable revenue |
| Consumption uplift | Data-obs customers show ≥20% DPS uplift | 10–20% | <10% |

_If App Adoption + ARR both Red → standalone app model is wrong; fold into existing apps instead._

---

## Build Track — Dynatrace-Built Capabilities

### Snowflake Monitoring (FY27, parallel to Phase 0–1)

| Milestone | What | Timeline | Owner |
|-----------|------|----------|-------|
| DSOA repackage | Repackage open-source Snowflake Observability Agent into supported solution with better UX | Q2–Q3 FY27 | Extensions PM (Maciej) |
| Dashboards & alerts | Out-of-the-box Snowflake health dashboards (query performance, credit consumption, failures) | Q3 FY27 | PM + PX |
| Snowflake App GA | Full Snowflake Monitoring App — warehouse visibility, cost attribution, table freshness | Q1–Q2 FY28 | PM + Eng |

**KPIs:** Snowflake tables monitored; customers with active Snowflake dashboards; DPS consumption from Snowflake telemetry.

### Databricks Extension Improvements (FY27, parallel)

| Milestone | What | Timeline | Owner |
|-----------|------|----------|-------|
| Gap analysis | Investigate gaps in current extension (system tables, data learning, competitor parity) | Q2 FY27 | Extensions PM (Maciej) |
| Extension refresh | Improved Databricks extension with broader metric coverage | Q3–Q4 FY27 | Extensions Eng |

### Data Quality & Anomaly Detection (FY28–FY29)

| Milestone | What | Timeline | Owner |
|-----------|------|----------|-------|
| Schema drift detection | Detect DDL changes, missing columns, type changes, partition shifts | Q3 FY28 | Eng (TBD) |
| Volume/freshness anomalies | Baseline + ML-driven detection of volume spikes/drops, stale data, unexpected null rates | Q3 FY28 | Eng + Davis team |
| Data profiling | Distribution, completeness, accuracy baselines | Q1 FY29 | Eng (TBD) |
| Custom DQ rules | User-defined quality rules (null thresholds, value ranges, cross-table consistency) | Q2 FY29 | Eng (TBD) |

**KPIs:** Anomalies detected/month; false positive rate; schema drift alerts; customer accounts with active DQ monitors.

### Orchestration Monitoring (FY28–FY29)

| Milestone | What | Timeline | Owner |
|-----------|------|----------|-------|
| dbt integration | Run results, test outcomes, model lineage, timing | Q2 FY28 | Eng (TBD) |
| Airflow integration | DAG state, task duration, backfill status, dependency monitoring | Q3 FY28 | Eng (TBD) + definity |
| Azure Data Factory | Pipeline monitoring, trigger tracking, activity metrics | Q4 FY28 | Eng (TBD) |

**KPIs:** Orchestration workflows monitored; active integrations per customer; pipeline incident MTTR.

### Pipeline Topology & Lineage (FY28–FY29)

| Milestone | What | Timeline | Owner |
|-----------|------|----------|-------|
| OpenLineage ingestion | Ingest lineage events from Airflow, dbt, Spark via OpenLineage standard | Q4 FY28 | PA + Eng |
| Smartscape data lineage | DAG visualization in Smartscape — source → transform → storage → app | Q1 FY29 | PA + Smartscape team |
| Impact analysis | Upstream/downstream impact analysis from any pipeline node | Q2 FY29 | PM + Eng |

**KPIs:** Pipelines with lineage; end-to-end DAGs visualized; cross-domain incidents resolved via lineage.

### Davis AI for Data (FY28–FY29)

| Milestone | What | Timeline | Owner |
|-----------|------|----------|-------|
| Pipeline anomalies in Problems | Pipeline failures/anomalies surface as Dynatrace Problems | Q2 FY28 | Davis team + PM |
| Cross-domain causal RCA | Davis reasons across pipeline → app → infra for root cause | Q4 FY28 | Davis team + PA |
| Proactive recommendations | AI-driven optimization recommendations for pipelines and clusters | FY29 | Davis team |

**KPIs:** Pipeline problems auto-detected; cross-domain RCA accuracy; time-to-root-cause improvement.

---

## Build vs. Partner Matrix (Quick Reference)

| Capability | Build (DT) | Partner (definity.ai) | Rationale |
|-----------|-----------|----------------------|-----------|
| Spark/Databricks deep monitoring | | ✓ | Specialized depth; faster via partner |
| Snowflake monitoring | ✓ | | Competitive necessity; standard APIs |
| Schema/quality detection | ✓ | | Proprietary advantage |
| Kafka/streaming (light) | ✓ | | API-based extensions |
| dbt integration | ✓ | | Standard API; quick ROI |
| Airflow integration | ✓ | ✓ | Standardize on OpenLineage; partner coverage |
| Smartscape integration | ✓ | | Core platform capability |
| Davis AI for data | ✓ | | Core differentiator |
| Pipeline lineage | ✓ | | OpenLineage + Smartscape |

---

## Financial Targets by Year

| Year | ARR | Key Driver |
|------|-----|-----------|
| **FY27** | ~$0.4M | Design partners, early POCs, DSOA repackage |
| **FY28** | ~$3–4M | Snowflake + Databricks apps GA; first enterprise deals; ~10% attach rate |
| **FY29** | ~$17M | Orchestration + data quality; upsell; ~30% attach rate |
| **FY30** | ~$49M | Mainstream adoption; replaces standalone tools in large deals |

---

## Pricing Direction (In Progress)

| Capability | Pricing Approach | Status |
|-----------|-----------------|--------|
| **Data Pipeline Monitoring** | Integrated into DPS via existing IRQ model (logs, events, traces) | Directional — needs Growth team review |
| **Data Orchestration** | New rate card — per workflow/task | Not started |
| **Data Quality Monitoring** | New rate card — per data asset or monitor executions | Not started |

**Next step:** Open pricing/packaging discussion with Growth team (flagged in 2026-02-23 alignment meeting).

---

## Key Dependencies (Cross-Team)

| Dependency | Team | What We Need | Status |
|-----------|------|-------------|--------|
| **Smartscape** | Platform / PAPA | Pipeline entities as first-class topology nodes; dependency edges | Not yet confirmed — Action 3 in PRODUCT-16280 |
| **Davis AI** | Data Intelligence | Pipeline anomalies as causal candidates in Problems | Not yet confirmed |
| **Grail** | Platform | Pipeline telemetry ingestion at scale; data contract for pipeline events | Directionally aligned |
| **Hub** | Platform Services | definity.ai extension listing and distribution | In progress |
| **OpenPipeline** | Platform / PPX | Mapping/enrichment/routing for pipeline telemetry | Not yet engaged |
| **IAM** | Platform Services | RBAC for data observability surfaces (data team ≠ app team) | Not yet engaged |

**⚠️ Action 3 (cross-team dependency map with named owners and capacity confirmation) is not yet complete. This is a blocker for Phase 1 planning.**

---

## Success Metrics (End FY27 → FY28)

| Category | Metric | FY27 Target | FY28 Target |
|----------|--------|------------|------------|
| **Adoption** | Customers with active data obs | 10 (design partners) | 50+ |
| **Consumption** | DPS from pipeline telemetry | Baseline established | Measurable uplift |
| **Revenue** | Data Observability ARR | ~$0.4M | ~$3–4M |
| **Pipeline** | Deal pipeline value (co-sell) | $2M+ pipeline | $10M+ pipeline |
| **Platform** | Monitored jobs/tasks (Databricks) | 500+ | 5,000+ |
| **Platform** | Snowflake tables monitored | 100+ | 1,000+ |
| **Quality** | POC-to-deal conversion rate | ≥50% | ≥60% |
| **Persona** | New data persona accounts reached | 15+ | 50+ |

---

## Common Labels (for artifact tagging)

- Fiscal year: `FY27`, `FY28`
- Personas: `data_engineer`, `data_platform_lead`, `platform_engineer`
- Platforms: `Snowflake`, `Databricks`, `Airflow`, `dbt`, `ADF`, `Kafka`
- Capabilities: `pipeline_monitoring`, `data_quality`, `orchestration`, `lineage`, `cost_optimization`
- Initiatives: `definity_partnership`, `smartscape_integration`, `davis_data`
- Phases: `phase_0_gtm`, `phase_1_integration`, `phase_2_smartscape`, `phase_3_app`
```
