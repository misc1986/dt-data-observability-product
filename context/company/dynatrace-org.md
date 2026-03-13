```markdown
# Dynatrace – Organizational & Operating Model (Solutions–Capabilities)  
**Working draft (collated from internal pages you opened).**  
**Owner:** Wolfgang Heider — Principal Product, Software Delivery

---

## 1) Executive Summary

Dynatrace organizes product development using a **Solutions–Capabilities** model:

- **Solutions** define **strategy and outcomes** for target personas and use cases (market‑facing and internal).  
- **Capabilities** are **reusable technical product components** and their people, serving multiple Solutions (m:n).  
- **Value Creation Teams (VCTs)** are **time‑bounded**, cross‑org teams with charters to achieve measurable goals.  
- A **Steering Committee** sets vision and investment focus, resolves conflicts, and governs cross‑solution alignment.  
- The **Value Creation Guide (VCG)** codifies roles, artifacts, and alignment mechanisms for scalable collaboration.

This document consolidates the **solutions, capabilities, leadership**, and the **operating model** and ends with a **clear steering section** ("who's in charge of what, who works on what, and how we plan & refine roadmap items").

---

## 2) Operating Model Primer

### 2.1 Core Model
- **Solutions**  
  - Own: vision → key themes → value packs (roadmap items) → value increments.  
  - Market‑facing (e.g., Observability) or internal‑facing (e.g., Platform).  
  - Measure: ARR/adoption (market), internal adoption/reuse (internal).
- **Capabilities**  
  - Groupings of dev teams owning technical components and quality.  
  - Serve multiple solutions; balance m:n demands with feasibility and technical excellence.
- **VCTs**  
  - Time‑scoped, chartered, measurable goals; disband upon completion.
- **Steering Committee**  
  - Sets vision and investment context; escalates/resolves cross‑solution tradeoffs.

### 2.2 Process & Governance
- **VCG**: Defines events, artifacts, RACI, and dependency management.  
- **Quarterly Capability Reviews (QCRs)**: Ops health, priorities, improvement areas.  
- **Dashboards**: Jira/time tracking/alignment dashboards for transparency.  
- **Jira**: Capability projects + issue hierarchy + link types for cross‑capability traceability.  
- **ACC support**: Coaching on capability formation, health, and improvements.

---

## 3) Solutions Overview (Leadership & Scope)

> Each Solution lists core scope and the most relevant capabilities (non‑exhaustive; see matrix in §5).

### 3.1 Platform
- **Solution Lead:** Andreas Lehofer  
- **Go‑To‑Market:** Christian Kiesewetter  
- **Growth:** Fabian Seydewitz  
- **Delivery:** Gerald Grill  
- **PM Director:** Michael Nemeth  
- **Architects:** Ernst Ambichl, Helmut Spiegl  
- **Product Leads:** Alexander Sommer, Paul Schumacher  
- **Experience Leads:** Simon Ludwig, Ursula Wieshofer  
- **Engineering Lead:** Clemens Fuchs  
**Scope:** Backbone of the platform — **Grail**, **AppEngine**, **AutomationEngine**, **OpenPipeline (PPX)**, **Platform Services** (IAM, Documents, Platform Management, Serverless), **Platform Apps (PAPA)** (Dashboards, Notebooks, Search, SmartScape), APIs.

### 3.2 Software Delivery
- **Solution Lead:** Bonifaz Kaufmann  
- **GTM:** Sharon Sharlin  
- **Growth:** Horst Pichler  
- **Delivery:** Martin Hoelbling  
- **PM Director / Product Lead:** **Wolfgang Heider**  
- **Architect:** **Stefan Eberl**  
- **Experience Lead:** Thomas Bayer  
- **APM:** Philipp Hamann  
- **Engineering Lead:** Stefan Gusenbauer  
**Scope:** **Agentic AI**, CI/CD observability, **DORA** dashboards, **quality gates**, SDLC eventing, release validation & **auto‑remediation**, **ecosystem integrations** (GitHub, GitLab, ArgoCD, Jenkins, ServiceNow, Slack/Teams, etc.).  
**Primary capability:** **Cloud Automation** (workflows, connectors, Monaco/Terraform, release intelligence, Backstage plugin).

### 3.3 Observability
- **Solution Lead:** Florian Ortner  
- **GTM:** Michael Winkler  
- **Growth:** Peter Vinh  
- **Delivery:** Stefan Perndl  
- **PM Director:** Mario Perez  
- **Architect:** Christoph Neumueller  
- **Experience Lead:** Galina Dvoretskaya  
- **Engineering Lead:** Stefan Gusenbauer  
**Scope:** Strategy/UX for metrics, logs, traces, RUM, synthetic, topology, troubleshooting ("Follow the Red").  
**Capabilities:** **Application Observability**, **Digital Experience Monitoring (DEM)**, **Infrastructure Observability**.

### 3.4 Application Security
- **Solution Lead:** Andreas Kroier  
- **Delivery:** Manfred Del Fabro  
- **GTM:** Bojan Magusic  
- **Growth:** Thomas Siegl  
- **Architect:** David Fuereder  
- **Product Lead:** Andreas Berger  
- **APM:** Camilla Bloos  
**Scope:** Runtime security, vulnerability detection, attack paths, unified security analytics, DevSecOps alignment.  
**Capabilities:** **Runtime Security Analytics**, **Security Intelligence Automation**.

### 3.5 Business Observability
- **Solution Lead:** Franz Karlsberger  
- **Growth/PM/Prod/Exp Lead:** Klaus Enzenhofer  
- **Delivery:** Filip Rafajec  
- **Architect:** Gernot Reisinger  
- **APM:** Laurentiu Maniu  
**Scope:** Exec insights, KPI↔IT mapping, process analytics, **cost & carbon**, compliance assistant.  
**Capabilities:** **Business Analytics**, **Business Data Experience**.

### 3.6 Delivery, Reliability, Security (DRS)
- **Solution Leads:** Florian Dorfbauer, Thomas Reisenbichler  
- **Product Leads:** Andreas Deuschl, Wolfgang Gottesheim  
- **GTM:** Florian Beck  
- **Growth:** Stefanie Boruta  
- **Delivery:** Damien Antipa  
- **PM Director:** Kurt Aigner  
- **Architect:** Michael Glaess  
- **APM:** Anna Poznanska  
- **Engineering Lead:** Thomas Stagl  
**Scope:** SDLC guardrails, product quality/security/privacy, ops excellence, cloud platform reliability.  
**Capabilities:** **ASDY**, **CLIN**, **QSP**, **SRE**.

### 3.7 Edge Data Platform
- **Solution Lead:** Alois Reitbauer  
- **GTM:** Lise Berda  
- **Growth:** Andreas Wurm  
- **Delivery:** Bernhard Baumgartner  
- **Product Lead:** Thorsten Roth  
- **APM:** Ulf Weihbold  
- **Engineering Lead:** Marcio Lena  
**Scope:** Edge ingest, **OpenTelemetry + OneAgent** unification, hybrid ingest, distributed/managed/SaaS.  
**Capabilities:** **Data Acquisition**, **Ingest Control Plane (ICP)**, **OneAgent**.

### 3.8 Growth & Monetization
- **Solution Lead:** Oliver Greifenstein  
- **GTM:** Christian Kiesewetter  
- **Growth:** Anvesh Goel  
- **Delivery:** Martin Stadler  
- **Architect (int.):** Michael Glaess  
- **Product Lead:** William Osteux  
- **Experience Lead:** Gernot Reiber  
- **APM:** Gerald Stanossek  
**Scope:** Pricing/packaging, DPS, adoption & experiments, growth analytics.  
**Capability:** **Licensing**.

### 3.9 Managed
- **Solution Lead:** Gregor Rechberger  
- **Delivery:** Dominik Stadler, Krystian Kowalski  
- **Product Lead:** Alexander Huetter  
- **Architect:** Stefan Moschinski  
- **Org Leads:** Aleksander Plinski, Thomas Achleitner  
- **APM/Eng Lead:** Asterios Stamatis / Thomas Achleitner  
**Scope:** On‑prem/air‑gapped regulated deployments, lifecycle, upgrade journeys.  
**Capability:** **Managed**.

*(Open Source & Research; Strategic Product Communication; X‑Solution & Operations — capture pending page ingestion.)*

---

## 4) Capabilities Catalog (selected, with leadership)

> **Note:** Full Part‑1 & Part‑2 list available; below highlights the ones most relevant so far.

- **Application Observability** — CL: Michael Kopp; DL: Andreas Grimmer; OL: Marco Mader; Arch: Andreas Gruber; Sec: Jakob Linskeseder.  
- **Digital Experience Monitoring** — CL: Bernat Trias; DL: Rainer Fernbach; OL: Anna Krzykowska; Arch: Bernhard Lackner; Sec: Florian Hofmann.  
- **Infrastructure Observability** — CL: Lucas Hocker; DL: Robert Zoralski; OL: Malgorzata Ziolkowska; Arch: Tobias Rauter; Sec: Jakob Linskeseder.  
- **Grail** — CL: Peter Zahrer; DL: Alram Lechner; OL: Thomas Grassauer; Arch: Herwig Moser; Sec: Renate Schosser.  
- **OpenPipeline (PPX)** — CL: Gerd Eberhardt; DL: Daniel Moertenschlag; OL: Peter Studener; Exec: Bernhard Kunnert; Arch: Gernot Reisinger; Sec: Renate Schosser.  
- **Platform Apps (PAPA)** — CL: Holger Weissboeck; DL: Szymon Bultrowicz; OL: Michael Leslie; Exec: Alex Estrada Gomez, Damian Skrodzki, Peter Romirer‑Maierhofer; Arch: Blai Samitier, Daniel Pieniazek, Philipp Raab; Sec: Jakob Linskeseder.  
- **Platform Services (PS)** — CL: Dirk Wallerstorfer; DL: Florian Buchegger; OL: Dietmar Steinberger; Arch: Stefan Chiettini; Sec: Renate Schosser.  
- **Quality, Security, Privacy (QSP)** — CL: Michael Plank; DL: Stefan Hagelmueller; OL: Dietmar Strasser; Exec: Johannes Feichtner; Arch: Markus Pfleger; Sec: Florian Hofmann.  
- **SRE** — CL: Gabriela Salamanca; DL: Dieter Ladenhauf; OL: Daniel Grandl; Arch: Thomas Fischl; Sec: Florian Hofmann.  
- **Cloud Automation** — **CL: Wolfgang Heider**; DL: Martin Hoelbling; OL: Rene Panzar; Arch: **Stefan Eberl**; Sec: Renate Schosser.  
- **Business Analytics** — CL: Klaus Enzenhofer; DL: Filip Rafajec; OL: Daniel Tieber; Arch: Gernot Reisinger; Sec: Johannes Preisinger.  
- **ASDY** — CL: Andreas Doblander; DL: Bernd Farka; OL: Michael Binz; Arch: Peter Feltl; Sec: Florian Hofmann, Jakob Linskeseder.  
- **CLIN** — CL: Johannes Opitz; DL: Michael Mayr; OL: Marius Ciortan; Exec: Marek Smolinski, Michael Mayr, Wojciech Stanislawski; Arch: Krzysztof Szyntar; Sec: Florian Hofmann.  
- **Security Intelligence Automation** — CL: Gerhard Byrne; DL: Stefan Achleitner; OL: Ulrich Fischer; Arch: Tamas Antal; Sec: David Fuereder / Jakob Linskeseder.  
- **Runtime Security Analytics** — CL: Ariel Shuper; DL: Florian Hoerschlaeger; OL: Ahmed Labieb; Arch: David Fuereder; Sec: Florian Hofmann.  
- **Licensing** — CL: Peter Brandl; DL: Martin Stadler; OL: Stefan Mayer; Arch: Daniel Guggi; Sec: Jakob Linskeseder.  
- **Managed** — CL: Dominik Stadler; DL: Krystian Kowalski; OL: Aleksander Plinski; Arch: Thomas Achleitner; Sec: Stefan Moschinski / Renate Schosser.

> **Important for Agentic work:** **Data Intelligence** — the page wasn't ingested yet, but cross‑references show DI owns **Davis® AI** and **Copilot backend**. This is a **critical partner** for agent reasoning, NL↔DQL, and safety guardrails. (See §8 Collaboration Map.)

---

## 5) Solutions × Capabilities Matrix (at a glance)

```
Observability:            Application Observability; DEM; Infrastructure Observability
Application Security:     Runtime Security Analytics; Security Intelligence Automation
Business Observability:   Business Analytics; Business Data Experience
DRS:                      ASDY; CLIN; QSP; SRE
Edge Data Platform:       Data Acquisition; ICP; OneAgent
Platform:                 Grail; OpenPipeline (PPX); Platform Services; Platform Apps (PAPA); (Data Intelligence*)
Software Delivery:        Cloud Automation (+ SDLC eventing, release intelligence)
Growth & Monetization:    Licensing
Managed:                  Managed
Open Source & Research:   (TBD)
SPC:                      (TBD)
X‑Solution & Operations:  (TBD)
* Data Intelligence: platform‑level, cross‑solution enabler for agentic AI.
```

---

## 6) Cross‑Capability Dependencies (selected)

- **PAPA ↔ Data Intelligence**: PAPA's UI Copilot integrates NL↔DQL; **Copilot backend owned by Data Intelligence**.  
- **Cloud Automation ↔ Platform Services**: Workflow runtime, tokens, IAM, platform lifecycle services.  
- **Cloud Automation ↔ Ecosystem**: ServiceNow, Slack/Teams, GitHub, GitLab, Jenkins, ArgoCD, PagerDuty connectors.  
- **OpenPipeline ↔ All Solutions**: Unified ingest & semantic normalization for logs/metrics/traces/events.  
- **Grail ↔ All Solutions**: Unified storage/query with DQL for analytics and Davis AI reasoning.  
- **DRS (QSP/SRE/ASDY/CLIN) ↔ All**: SDLC guardrails, reliability, developer platform & cloud infra.  
- **Business Analytics ↔ Observability**: BizEvents/flows correlated with tech signals for impact/priority.

---

## 7) Communication & Artifacts (by layer)

- **Solutions**: Vision, Key Themes, Value Packs, Value Increments; solution SharePoint; solution mailbox; Teams; VCT registry.  
- **Capabilities**: Charter, scope, Jira project, help channels, bug handling guidance, dashboards; QCRs; ACC coaching.  
- **VCTs**: Charter (goal, KPIs, timeline), resourcing (skill‑based), dependency mapping, demo cadence, exit criteria.  
- **Ops**: Slack #help‑* channels, capability aliases, Jira hierarchy/link types, time tracking (InEx) dashboards.

---

## 8) Collaboration Map for **Agentic AI** (who to engage)

- **Software Delivery / Cloud Automation** (owner of SD connectors, SDLC eventing, release intelligence, Monaco/Terraform, Backstage).  
  - **Decisioning & Actions**: quality gates, auto‑remediation, pipeline orchestration.
- **Data Intelligence** (Davis AI, Copilot backend — **reasoning core**; NL↔DQL; planning/guardrails).  
  - **Intent → Plan → Query → Action** loop and safety rails.
- **Platform Services** (IAM, tokens, serverless runtime, platform management, documents).  
  - **Execution substrate** for agent actions, identity and policy integrations.
- **Grail & OpenPipeline** (data access and ingest hooks).  
  - **Data plane** for perception; semantic dictionary alignment.
- **PAPA** (Dashboards, Notebooks, Search, conversational UI).  
  - **User interaction layer** for agent prompts, results, and actions.
- **Observability Capabilities** (AppObs, DEM, InfraObs).  
  - **Domain signals** the agent reasons over; tracing/logs/RUM/infra context.
- **DRS (QSP + SRE + ASDY + CLIN)**  
  - **Reliability, SDLC governance, platform infra, developer platform** used by the agent and by the delivery process.

---

## 9) Planning & Refinement — **Who is in Charge of What** (RACI + Flow)

> Use this to steer **roadmap items** (Value Packs / Value Increments) and to guide **agent/VCT work**.

### 9.1 Roles (simplified RACI)

- **Solution Lead (SL)** — **A/R** for **vision, key themes, value packs**, market alignment, outcome definition.  
- **Product Lead / PM Director** — **R** for **pack definition**, scope, KPIs; **A** for prioritization within solution.  
- **Delivery Lead (DL)** — **R** for **planning & execution** across teams; risk & dependency mitigation; forecast.  
- **Architect(s)** — **R** for **feasibility, architecture, cross‑capability design**, non‑functionals, standards.  
- **Capability Lead (CL)** — **R** for **component roadmap**, quality, feasibility, resourcing; **C** on solution plans.  
- **Capability Delivery Lead / Org Lead** — **R** for team execution, staffing, ops health (QCR inputs).  
- **APM / Agile CC** — **R** for orchestration, cadence, alignment events, VCT support.  
- **Steering Committee** — **A** for **investment decisions**, conflict resolution across Solutions.

> For **agentic topics**, add:  
> **Data Intelligence (CL/Arch)** — **R/C** for **intent models, tool schemas, guardrails, evaluation**.  
> **Platform Services (IAM/Policies)** — **R/C** for **identity, authorization, audit** on agent actions.

### 9.2 Roadmap Flow (Value Packs → Value Increments)

1) **Ideation & Framing (Solution)**
   - SL/PM define the **Value Pack** (problem, outcomes, KPIs, personas).  
   - Check **strategic fit** (vision/key themes).  
   - Early **feasibility consultation** with impacted Capabilities (CL/Arch) and DI for agentic elements.

2) **Discovery & Alignment (Solution × Capabilities)**
   - **VCT Charter** (if cross‑org): scope, KPIs, exit criteria, dependencies, staffing model, timeline.  
   - **Architectural alignment** (Capabilities' Arch + Platform/DI/PS/OP/PAPA).  
   - **Security & Privacy gating** (QSP), **Reliability** implications (SRE), **Cloud footprint** (CLIN).

3) **Planning & Breakdown**
   - **Value Pack → Value Increments → Dev Epics**; define **artifact model** in Jira (Solution & Capability projects).  
   - Linkage policy:  
     - **Solution EPIC** links **Capability EPICs** (blocks/relates/depends‑on).  
     - **VCT Board** mirrors cross‑capability timeline + risk log.  
   - **Definition of Done** includes solution outcomes, telemetry, rollout, enablement, and Ops runbooks.

4) **Execution**
   - **DL** runs cadence; **APM** coordinates cross‑solution events.  
   - **Demo cadence** (Value Increment reviews), **feature flags**, **progress dashboards**.  
   - **Agentic**: DI delivers **intent/tooling** services; Cloud Automation integrates **actions/quality gates**; PS/IAM completes **policy**.

5) **Governance & Review**
   - **QCRs (Capabilities)** — ops health, throughput, improvements.  
   - **Steering checkpoints** — investment changes, inter‑solution conflicts.  
   - **Business results** review (adoption/ARR or internal reuse), DORA, SLO/SLA.

6) **Release & Rollout**
   - **SRE** for release planning/readiness; **QSP** for security/privacy verifications.  
   - **Enablement:** SPC / Product Comms; **Growth** for packaging & monetization impacts.  
   - **Post‑release**: telemetry validation, incident playbooks, **self‑healing patterns** via Cloud Automation.

---

## 10) "Who Works on What" — Assignment Rules for Roadmap Items

When creating or refining items, route ownership as follows:

- **Agentic AI features (reasoning, NL↔DQL, action planning)**  
  - **R:** **Data Intelligence** (models, semantics, Copilot backend)  
  - **C:** **Cloud Automation** (actions/quality gates), **Platform Services** (IAM/policy), **PAPA** (UI Copilot), **Grail/OpenPipeline** (data plane)

- **CI/CD observability, DORA dashboards, pipeline insights**  
  - **R:** **Software Delivery (Solution)**  
  - **C:** **Cloud Automation**, **Observability Capabilities** (AppObs, InfraObs), **PAPA** (Dashboards/Notebooks)

- **Workflow integrations (Slack/Teams, ServiceNow, GitHub/GitLab/Jenkins/ArgoCD, PagerDuty)**  
  - **R:** **Cloud Automation**  
  - **C:** **Platform Services** (API Gateway, Tokens), **Software Delivery (Solution)**

- **Release validation, change risk scoring, auto‑remediation**  
  - **R:** **Cloud Automation**  
  - **C:** **Data Intelligence** (risk models), **SRE/QSP** (guardrails), **Observability** (signals)

- **Platform data & ingest**  
  - **R:** **OpenPipeline (PPX)**, **Grail**  
  - **C:** **Data Acquisition/ICP**, **all signal owners** (AppObs/DEM/InfraObs/Business Analytics)

- **Identity, access, policies, serverless runtime for apps/agents**  
  - **R:** **Platform Services**  
  - **C:** **Cloud Automation** (action execution), **Solutions** consuming IAM/Policies

- **UI analytics, search, conversational interface**  
  - **R:** **PAPA**  
  - **C:** **Data Intelligence** (Copilot backend), **Solutions** providing domain content

- **Developer platform / golden paths (internal)**  
  - **R:** **ASDY**  
  - **C:** **QSP/SRE/CLIN/PS** for guardrails, reliability, infra, and platform services

- **Cloud infrastructure & governance**  
  - **R:** **CLIN**  
  - **C:** **SRE/QSP/PS** for reliability, security, platform alignment

---

## 11) Practical Steering Guide (Checklists)

### 11.1 Intake checklist (before planning)
- Does the item map to a **Solution** key theme? If not, reshape or reject.  
- Which **Capabilities** are impacted? Validate **feasibility** & **capacity** with CL/DL.  
- Any **agentic** parts? Loop in **Data Intelligence** + **Platform Services** (policies).  
- Security/Privacy/Compliance relevant? Involve **QSP** early.  
- Reliability/SLA? Involve **SRE** and **CLIN** if infra‑heavy.  
- UX/UI? Involve **PAPA** for platform UI patterns and Copilot surface.  
- Data plane changes? **PPX/Grail** engagement and semantic alignment.

### 11.2 Planning artifacts
- **Solution Value Pack** (problem, hypotheses, outcomes, KPIs, guardrails).  
- **VCT Charter** (scope, KPIs, resourcing, timeline, dependencies).  
- **Jira linking**: Solution EPIC ↔ Capability EPICs (+ link types).  
- **Architecture doc**: cross‑capability design, security & reliability controls.  
- **Runbooks & rollout**: release plan, feature flags, enablement assets.

### 11.3 Execution cadence
- Weekly **delivery sync** (DL/APM/CLs).  
- Fortnightly **VCT review** (demo + risk board).  
- Monthly **Steering** (if cross‑solution investments or conflicts).  
- **QCR** per capability per quarter.

---

## 12) Next Actions & Owner Map (near‑term, agentic focus)

1) **Confirm Data Intelligence page & contacts**  
   - **Owner:** Wolfgang → open page for ingestion  
   - **Why:** Establish formal engagement for **Copilot backend**, **intent/tool** schemas, **guardrails**.

2) **Define Software Delivery Agent patterns** (release decisioning, remediation)  
   - **R:** Cloud Automation (Wolfgang + Stefan E.)  
   - **C:** Data Intelligence, PS (IAM), PAPA, Observability

3) **ServiceNow first‑class integration plan**  
   - **R:** Cloud Automation  
   - **C:** Software Delivery Solution, PS (API/Tokens), QSP (data & privacy), SRE (ops workflow)

4) **IDE/Dev persona enablement** (Backstage + IDE extensions alignment)  
   - **R:** Software Delivery (Cloud Automation + Backstage)  
   - **C:** ASDY (developer platform), Observability (AppObs), PAPA (UX)

5) **Working‑Backwards PRFAQ + C‑level slide** (Agent Command Center)  
   - **R:** Wolfgang  
   - **C:** Data Intelligence, PAPA, PS, Observability, DRS leadership

---

## 13) Contact Pointers (selected)

- **Software Delivery** — `SoftwareDeliveryLeadership@dynatrace.com`  
- **Cloud Automation** — `Cap-Cloud-Automation-All@dynatrace.com`  
- **Platform Services (IAM/Policies/Runtime)** — `#help-platform-services`, `#help-oauth`, `#help-iam`  
- **PAPA** — `cap-papa-all@dynatrace.com` / #help‑dashboards‑app / #help‑notebooks‑app  
- **OpenPipeline (PPX)** — `cap-ppx-all@dynatrace.com`, #help‑openpipeline‑ppx  
- **Observability (Infra/App/DEM)** — solution & capability channels (#team‑infraobs‑all, #help‑rum‑web, #help‑rum‑mobile, etc.)  
- **DRS** — solution space & channels; QSP/SRE/ASDY/CLIN respective aliases

---

## 14) Appendix — Notes on VCTs

- Use VCTs when delivery requires **cross‑solution/capability alignment** with measurable outcomes.  
- Members should be **(mostly) dedicated** and assigned by skill & motivation, not title.  
- Charter must include: **problem & success metrics**, **timeline**, **dependencies**, **resourcing model**, **exit criteria**.  
- VCT dissolves upon completion; learnings move into **capability roadmaps**.

---

# Steering Section (TL;DR)

**When we plan & refine roadmap items:**

- **Solutions** are in charge of **what & why** (vision, key themes, Value Packs, outcomes).  
- **Capabilities** are in charge of **how** (technical feasibility, component ownership, quality, performance).  
- **Delivery Leads & APMs** orchestrate **execution** across orgs; **Steering** arbitrates investments & conflicts.  
- For **agentic features**, engage **Data Intelligence** (reasoning, Copilot backend) and **Platform Services** (IAM/policies) **early**; **Cloud Automation** owns **actions/quality gates/workflows**; **PAPA** provides **UI Copilot** surfaces; **Grail/PPX** provide **data plane**.

**Default ownership routing:**
- **Agentic reasoning/NL↔DQL** → **Data Intelligence (R)**; Cloud Automation/PAPA/PS/Observability (C).  
- **Workflow actions & connectors** → **Cloud Automation (R)**; PS (IAM), Service owners (C).  
- **CI/CD & DORA dashboards** → **Software Delivery (R)**; Observability/PAPA (C).  
- **Identity/tokens/policies/serverless runtime** → **Platform Services (R)**.  
- **Ingest & data store** → **OpenPipeline/Grail (R)**.  
- **Reliability/security/privacy** → **SRE/QSP (R)** across SDLC.  
- **Developer platform/golden paths** → **ASDY (R)**.  
- **Cloud infra/governance** → **CLIN (R)**.

**Mandated governance touchpoints:**
- **VCT Charter** for cross‑org packs; **Architecture review**; **QSP/SRE gates**; **QCR**; **Steering** as needed.

---

*End of document — ready to export to Confluence/SharePoint or extend with the remaining Solution pages (Open Source & Research, SPC, X‑Solution).*

```
