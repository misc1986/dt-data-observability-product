# Value Pack Template (Data Observability)

> **Adapted from:** `software-delivery/VALUE-PACK-TEMPLATE.md`  
> **Trimmed for:** A small team (~4 people) working on a single-Solution, partnership-driven initiative.  
> **When to use:** You're proposing a new press-release-worthy capability that becomes a strategic topic. If it's smaller, use a Value Increment instead.

A **Value Pack** is a business case explaining **why** we should invest in solving a significant customer pain. It describes the problem, value, and scope — not the implementation details (those live in Value Increments).

---

## Template

```yaml
---
key: PRODUCT-XXXXX  # Assigned by Jira on creation
summary: <Business-value focused title, 8-15 words>
status: Open
priority: Undefined
labels:
  - <Capability label, e.g., data-quality, pipeline-obs, spark, snowflake>
  - <Strategic label if applicable, e.g., definity-partnership>
issueType: Value Pack
customFields:
  owning Program: Business Observability
  Labs:
    - Global
  Participants:
    - <Your Name>
  Effort: 0
---
```

### Parent

- **PRODUCT-XXXXX** (Key Theme): <Parent Key Theme title>

---

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
- "Business language first — Raj shouldn't need to know Dynatrace concepts">

### Where This Shows Up

- Primary surfaces: <e.g., Data Observability App, Smartscape, Notebooks>
- Secondary surfaces: <e.g., dashboards, APIs, alerts>

### Business Rationale

<Why is this important for Dynatrace? Connect to:
- MCG alignment (MCG 1 / 2 / 4)
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

### Value Increments (outline)

<List 3-7 candidate VIs (titles only). Details go into VI issues.>

### Data / Platform Assumptions

<Call out platform dependencies early:>
- OpenTelemetry / OpenLineage support: <expectations>
- OpenPipeline considerations: <mapping/enrichment/topology needs>
- Smartscape integration: <entity model assumptions>
- Grail storage: <schema/bucket expectations>

---

## Relationships

```
Key Theme (parent — required)
    └── Value Pack (YOU ARE HERE)
            └── Value Increment (children)
```

Link types:
- **Parent**: Required link to Key Theme
- **is improved by**: Value Increments that deliver parts of this VP
- **relates to**: Other VPs with overlapping scope
- **is blocked by**: Dependencies that must be resolved first

## Status Workflow

1. **Open** → 2. **Solution proposed** → 3. **Solution accepted** → 4. **Implementation** → 5. **Cancelled** (if deprioritized)

## Tips

1. **Think press release** — Could this be announced externally? If not, it might be a VI.
2. **Focus on business value** — Describe outcomes, not features.
3. **MCG mapping is mandatory** — Every VP must connect to at least one MCG.
4. **Define Customer Zero** — Who validates this first?
5. **Be explicit about build vs. partner** — What does definity.ai deliver vs. Dynatrace?

---

## Common Labels (Data Observability)

| Label | Purpose |
|-------|---------|
| `pipeline-obs` | Data pipeline observability |
| `data-quality` | Data quality monitoring |
| `spark` | Apache Spark / Databricks |
| `snowflake` | Snowflake integration |
| `definity-partnership` | Joint definity.ai work |
| `ai-data-supply` | AI data supply chain |
| `FY27` / `FY28` | Fiscal year targeting |
