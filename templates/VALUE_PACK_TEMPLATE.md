# [Value Pack Name]

> **Key:** PRODUCT-XXXXX *(optional — add when Jira issue is created)*  
> **Status:** <Open | Solution Proposed | Solution accepted | Implementation | Cancelled | Done>

---

> **Template guide:**  
> **Optimized for:** A small team (~4 people) working on a single-Solution, partnership-driven initiative.  
> **When to use:** You're proposing a new press-release-worthy capability that becomes a strategic topic. If it's smaller, use a Value Increment instead.
> 
> A **Value Pack** is a business case explaining **why** we should invest in solving a significant customer pain. It describes the problem, value, and scope — not the implementation details (those live in Value Increments).

---

## Pitch (Open)

### 2 Minute Pitch

<2-3 paragraphs. If a customer reads only this, they should understand:
- What problem this solves
- What value it delivers
- Why Dynatrace (our differentiation)>

### The Human Challenge (1-3 sentences)

<Make the stakes real in plain language. Keep it outcome-focused.>

### Target Audience

- **Primary Persona:** <Name — Role> (e.g., Raj — Senior Data Engineer)
- **Secondary Personas:** <e.g., Maria — VP Data Engineering; Jennifer — Platform Eng Lead>

**Primary Persona block:**
- Context: <environment + responsibilities>
- Pain today: <1-2 bullets>
- Success criteria: <measurable outcomes>

### Customer Zero Candidate

- <Internal team or external customer who will pilot this>
- <Specific use case or need they have>

---

## Why (Solution Proposed)

### Pain Journey

<Current pain points grouped by moments that matter. Keep it VP-level — details live in VIs.>

**During day-to-day work:**
- <Pain>

**During incidents:**
- <Pain>

**During planning & communication:**
- <Pain>

### Solution Journey

<Proposed solution:
- How will users achieve their goals?
- What does the ideal workflow look like?
- Where does definity.ai fit vs. what Dynatrace builds natively?>

### Design Principles (3-5 max)

<Experience guardrails that shape this VP. Examples:
- "Platform-native, not bolt-on"
- "Data pipelines as first-class entities in Smartscape"
- "Business language first — users shouldn't need to know Dynatrace internals">

### Where This Shows Up

- Primary surfaces: <e.g., Data Observability App, Smartscape, Notebooks>
- Secondary surfaces: <e.g., dashboards, APIs, alerts>

---

## What (Solution Accepted)

### Business Rationale

<Why is this important for Dynatrace? Connect to:
- MCG alignment
- Market opportunity (TAM, customer demand signals)
- Competitive pressure (Datadog, Monte Carlo, etc.)>

### Competitive Context

<1-3 key competitors. Keep it concise.>

| Competitor | Approach | Our differentiation |
|-----------|----------|-------------------|
| <name> | <summary> | <value/UX/cost advantage> |

### Monetization Approach

<How does this contribute to revenue?
- Pricing model (consumption, license, hybrid)
- Build vs. partner revenue split considerations>

### Success Metrics

<How will we measure success? Include at least:>

| Metric | Target | Timeframe |
|--------|--------|-----------|
| Time-to-first-value | <target> | <when> |
| Adoption / usage | <target> | <when> |
| Value proof (e.g., incidents prevented, time saved) | <target> | <when> |

### Out of Scope

<What is explicitly NOT included in this Value Pack?>

### Key Deliverables

<Bulleted list of concrete deliverables:>
- <Feature or capability 1>
- <Feature or capability 2>
- <Integration or partner deliverable>

### Value Increments

<Track VIs that deliver this Value Pack. Update status as work progresses.>

| VI | Status | Owner | Target |
|----|--------|-------|--------|
| [PRODUCT-XXXXX](../value-increments/PRODUCT-XXXXX-feature/) | Open | @owner | Q1 2026 |
| [Feature Name](../value-increments/feature-name/) | Not started | @owner | Q2 2026 |

### Data / Platform Assumptions

<Call out platform dependencies early:>
- OpenTelemetry / OpenLineage support: <expectations>
- OpenPipeline considerations: <mapping/enrichment/topology needs>
- Smartscape integration: <entity model assumptions>
- Grail storage: <schema/bucket expectations>

---

## Tips

1. **Think press release** — Could this be announced externally? If not, it might be a VI.
2. **Focus on business value** — Describe outcomes, not features.
3. **MCG mapping is mandatory** — Every VP must connect to at least one MCG.
4. **Define Customer Zero** — Who validates this first?
5. **Be explicit about build vs. partner** — What does definity.ai deliver vs. Dynatrace?