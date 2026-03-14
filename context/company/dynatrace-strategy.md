# Dynatrace Company Strategy Context (2026)

> **Last updated:** 2026-01-19  
> **Note:** Company-level strategy context relevant for Data Observability product work.

---

This document summarizes the 2026 company-level strategy context, grounded in the Application Observability + Log Analytics vision and the FY26 Mission Critical Goals (MCGs).

## Strategic Context (grounded)

Dynatrace's 2026 direction is to complete and drive adoption of the latest Dynatrace platform (3rd gen), expand cloud‑native + AI‑native workloads (with developers as key decision influencers), and accelerate log monitoring and analytics. Execution is organized around June/December rallies and parallel strategic goals.

Key product strategy tenets (company-wide):

- **3rd gen first, with a low-friction path for existing customers**; classic (2nd gen) remains supported where required.
- **Cloud‑native + AI‑native workloads** are the growth focus; developer experiences must be first-class.
- **Value must be collection‑agnostic**: OpenTelemetry and API-ingested data must achieve the same Dynatrace outcomes as native collection when the data contract is satisfied.
- **OpenPipeline + an explicit observability data contract** are the "unification layer" for mapping, enrichment, routing, permissions, cost allocation, and consistent AI/analytics behavior.
- **Unified tagging (primary Grail fields + primary tags)** is the scalable replacement for legacy auto-tagging/mgmt-zones in Grail contexts.
- **AI value must scale on mass data** (patterns, bubble-up correlation, causal and agentic AI), not only on single traces or single log lines.

## FY26 Mission Critical Goals (MCGs): Must‑Win Priorities

The FY26 MCGs provide the top-level execution frame:

### MCG 1 — Latest Dynatrace Completeness & Adoption (3rd gen)

**Key principle:** Prioritize 3rd-gen-first workflows; ensure new capabilities are 3rd-gen-native and use platform-consistent contracts (permissions, routing, tags).

### MCG 2 — Cloud‑Native Workload Expansion

**Key principle:** Support cloud-native and AI-native workloads; treat OpenTelemetry as first-class; enable easy onboarding and mapping.

### MCG 3 — Log Monitoring and Analytics Acceleration

**Key principle:** Logs as first-class troubleshooting surface; reduce time-to-answer using logs + traces + topology context; compatible with OpenPipeline governance and cost control.

---

## Consumption Lens (cross-cutting)

Across all MCGs, we should bias toward product outcomes that drive:

- Faster time-to-first-value
- Higher adoption of 3rd gen workflows
- Increased usage of analytics (logs, traces, workflows) via daily user touchpoints

## Platform Alignment Principles

All capabilities should align to platform direction by:

1. **Building collection-agnostic value**: requirements must specify needed data in terms of fields/semantics, not collection method.
2. **Leaning on platform contracts**: primary fields/tags, OpenPipeline governance, and consistent permissions/cost context.
3. **Low-friction onboarding**: reduce time-to-first-value with context-rich guidance.
4. **Supervised autonomy by default**: auditable actions, approvals, and clear ownership boundaries for automated workflows.

---

## Product & Platform Roadmap Themes (Execution Lens)

**3rd‑Gen Experience**: unified navigation, context‑aware insights, role‑based workspaces, and AI copilots with explainability.

**AI Observability & Agentic Governance**: policy‑bounded actioning, change‑impact simulation, lineage across systems, and audit‑ready decision trails.

**Logs @ Scale**: PB‑scale ingestion, adaptive retention tiers, OpenPipeline policies, and Davis AI narratives; queries‑included pricing to simplify procurement.

**Grail as the Contextual Lakehouse**: cross‑domain joins, entity graphs, fine‑grained RBAC, data residency controls for regulated industries.

---

## Go‑to‑Market Motions & Plays
**Hyperscaler Co‑Sell**: packaged solutions (e.g., EKS/GKE/AKS blueprints, serverless packs, AI stack packs) with marketplace transactability; joint ROI cases. citeturn7search1turn7search2

**Competitive Logs Takeout**: TCO head‑to‑head with assisted migration, OpenPipeline tuning, and AI narratives; win themes: cost, speed, simplicity.

**AI Reliability for the C‑Suite**: board‑level resilience dashboards linking AI reliability to revenue risk; supervised autonomy readiness assessments.

**Developer Adoption Flywheel**: free trials with opinionated templates, IDE quickstarts, golden paths for K8s/serverless; usage‑based expansion.

---

## Operating Model, Governance & Metrics
**Whole Product Lifecycle (WPL)** with **semiannual rallies** align R&D, PM, Design, Docs, Marketing, Sales, and Services to MCGs; success measured by consumption and customer outcomes.

**Cadence & Reviews**
- **Monthly**: MCG scorecards (leading/lagging consumption metrics, NRR, workload penetration).
- **Quarterly**: Rally readouts; GTM pipeline & partner influence; competitive win/loss (esp. logs).
- **Biannual**: Strategy refresh vs. CTO outlook (agentic AI trends, autonomy maturity).

**Core Metrics**
- **Consumption** per account (+XX%), **DPS attach** (+XX%), **feature adoption** (+XX pp), **time‑to‑first value** (−XX%), **partner‑influenced bookings** (≥80%), **AI workload coverage** (+XX%). citeturn7search1turn7search2

---

## Risks, Assumptions & Mitigations (RAM)
- **AI safety & governance gaps** → require **supervised autonomy** guardrails, explainability, and auditability as out‑of‑the‑box capabilities.
- **Toolchain fragmentation in cloud‑native** → hyperscaler patterns + curated integrations reduce deployment friction.
- **Data gravity & ingestion costs (logs)** → OpenPipeline policies, tiered retention, and queries‑included pricing to control TCO.
- **Adoption inertia for 3rd‑gen UX** → phased migration, in‑product guidance, Dynatrace ONE enablement.

---

## Timeline & Milestones (FY26)
- **Q3 FY26**: 3rd‑gen default for core workflows; 3–5 hyperscaler blueprints GA; logs strike‑team playbooks in market.
- **Q4 FY26**: AI/LLM observability packs v2; OpenPipeline policy library GA; DPS attach +XX pp; partner influence ≥80% sustained. citeturn7search1turn7search2
- **Perform & Mid‑Year**: showcase agentic governance and resilience outcomes; publish autonomy readiness framework. citeturn7search2turn3search1

## 2026 Target Outcomes
- Consumption-led ARR growth
- Hyperscaler workload gains and AI/LLM observability adoption
- Logs growth with strong competitive performance
- Customer outcomes: faster MTTR, improved reliability, stronger AI trust

## Executive Summary Line
Dynatrace's 2026 strategy is to become the essential AI-powered observability control plane for autonomous, cloud-native enterprises by completing & driving adoption of the 3rd-gen platform, winning hyperscaler workloads, accelerating Logs + Grail, and aligning the entire company around consumption-led growth.

---

## Narrative Anchors (CEO / CTO / MCGs)
- CEO direction: "AI Winner" and autonomous operations; ship AI‑first, cloud/AI‑native, consumption‑driving capabilities.
- CTO outlook: autonomy maturity curve (preventive → recommendations → supervised autonomy → autonomy) and resilience as the north star.
- MCGs: focused company execution framework to drive adoption and consumption.

---

## Sources
- Our 2026 Mission Critical Goals (SharePoint): https://dynatrace.sharepoint.com/sites/DLTCOMMS/SitePages/Our-2026-Mission-Critical-Goals.aspx
- Welcome to 2026! (CEO Letter, SharePoint): https://dynatrace.sharepoint.com/sites/DLTCOMMS/SitePages/Welcome-to-2026!.aspx
- Six observability predictions for 2026 (CTO Blog, dynatrace.com): https://www.dynatrace.com/news/blog/six-observability-predictions-for-2026/
