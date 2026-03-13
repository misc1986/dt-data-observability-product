# [Value Increment Name]

> **Key:** PRODUCT-XXXXX *(optional — add when Jira issue is created)*  
> **Status:** <Open | Problem stated | Use case defined | Ready for implementation | In progress | Done>  
> **Value Pack:** PRODUCT-XXXXX — [Value Pack Name]

---

> **Template guide:**  
> **Optimized for:** A small team where most VIs are lean. Full specification sections are marked optional — use them for cross-team or security-critical VIs.  
> **When to use:** You're defining a concrete, implementable deliverable that enables a specific use case or feature. A VI is the actual work item that engineering commits to.
> 
> **Folder structure:**  
> - Create folder: `../value-increments/feature-name/` (or `PRODUCT-XXXXX-feature-name/`)
> - Save this template as: `increment.md` in that folder
> - Create subfolder: `artifacts/` for supporting materials
> - Keep folder names under 50 characters, use lowercase kebab-case
> - Rename folder when Jira ID is assigned

---

## Idea (Open)

### Short Abstract

<1-2 paragraphs:>

I, as a **<PERSONA>**, can **<DO SOMETHING>** in order to **<ACHIEVE THIS>**.

As Dynatrace, this is important for **<MCG / Solution Strategy alignment>**.

### Experience Statement

<What users will say after using this:>
- "I can easily..."
- "I don't have to..."
- "This saves me time by..."

---

## Why (Problem stated)

### The Human Challenge

<1-3 sentences making the stakes real. Put the user under realistic pressure.>

### Current User Pain Points

**During day-to-day work:**
- <Pain>

**During incidents:**
- <Pain>

### Users We're Serving

<Define 1-3 personas this VI targets. Start with the primary persona. Add secondary personas if they have significantly different needs or workflows.>

**Primary Persona: <Name> — <Role>**
- Context: <environment + responsibilities>
- Goals: <top 3>
- Pain: <what hurts today>
- Success criteria: <measurable outcomes>

**Secondary Persona: <Name> — <Role>** *(optional)*
- Context: <environment + responsibilities>
- Goals: <top 3>
- Pain: <what hurts today>
- Success criteria: <measurable outcomes>

### Why Now / Competitive Context

<Primary problem this VI solves and why now. 1-3 competitors and our differentiation.>

| Competitor | Approach | Our differentiation |
|-----------|----------|-------------------|
| <name> | <summary> | <where we win> |

### Customer Zero

- <Internal team or customer who will validate this>
- <Specific use case>

### Success Metrics

| Metric | Target | How measured |
|--------|--------|-------------|
| <adoption, usage, time saved, etc.> | <number> | <method> |

### Assumptions / Open Questions

<Keep short; update as you learn.>

| Type | Statement | Owner | Validation plan |
|------|-----------|-------|----------------|
| Assumption | <what we assume> | <who> | <how/when to validate> |
| Open question | <what we don't know> | <who to ask> | <by when> |

---

## What (Use case defined)

### Scenarios

<Define 1-3 concrete scenarios. Start with the primary scenario. Add additional scenarios if serving multiple personas or significant workflow variations.>

#### Scenario 1: [Primary Scenario Name]

- **Persona:** <e.g., Data Engineer>
- **Pre-requisites:** <What must be in place?>
- **Context:** <When/where does this happen?>
- **Steps (from user's perspective):**
  1. <step>
  2. <step>
  3. <step>

#### Scenario 2: [Alternative Scenario] *(optional)*

- **Persona:** <e.g., Data Analyst>
- **Pre-requisites:** <What must be in place?>
- **Context:** <When/where does this happen?>
- **Steps:**
  1. <step>
  2. <step>
  3. <step>

### Where This Shows Up

- Primary surfaces: <e.g., Data Obs App, pipeline detail view, Notebooks>
- Secondary surfaces: <e.g., dashboards, alerts, APIs>
- Notifications: <where + what>

### Out of Scope

- <What is explicitly NOT included>

---

## How (Ready for implementation) — *expand for complex VIs*

### Key Deliverables (Tiered)

- **Tier 1 — Core (MVP):** <end-to-end core use case, shippable + demoable>
- **Tier 2 — Depth:** <common variants/personas>
- **Tier 3 — Polish:** <edge cases, advanced>

### Functional Requirements

- <Requirement 1>
- <Requirement 2>

### Acceptance Criteria

- Given <context>, when <action>, then <expected result>
- Given <context>, when <action>, then <expected result>


### Non-Functional Requirements *(optional for lean VIs)*

- Performance: <targets>
- Security: <considerations>

### Enablement Requirements *(optional for lean VIs)*

- Docs: <what must be updated>
- Release notes: <category + title>
- Support readiness: <runbooks, known limitations>

---

## Tips

1. **Start lean** — Fill Idea + Why first. Add What + How as you refine.
2. **Link to parent VP** — Every VI must have a Value Pack parent.
3. **Define Customer Zero** — Who validates this works?
4. **Multiple personas/scenarios** — If your VI serves multiple personas with different workflows, define separate scenarios. Keep the primary scenario focused on the most critical use case.
5. **Be concrete** — VIs should be deliverable by a team in a quarter or less.
