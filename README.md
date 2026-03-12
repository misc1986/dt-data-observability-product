# Data Observability Product Documentation

This repository contains structured product documentation for Data Observability Value Packs and Value Increments.

## Folder Structure

```
dt-data-observability-product/
├── templates/
│   └── VALUE_INCREMENT_TEMPLATE.md    # Template for creating new VIs
├── value-increments/                   # Individual deliverable features
│   ├── PRODUCT-XXXXX-feature-name.md
│   └── feature-name.md                 # Without Jira ID initially
├── value-packs/                        # Collections of related VIs
│   └── PRODUCT-XXXXX-pack-name.md
└── README.md                           # This file
```

## Naming Conventions

### Value Increments (VIs)

Value Increment files should follow these naming patterns:

**With Jira ID:**
```
PRODUCT-XXXXX-short-kebab-case-description.md
```

**Without Jira ID (initially):**
```
short-kebab-case-description.md
```

**Guidelines:**
- Use lowercase kebab-case for readability
- Keep names under 50 characters
- Use descriptive but concise names
- Rename file when Jira ID is assigned

**Examples:**
- `PRODUCT-16280-pipeline-observability.md`
- `PRODUCT-16281-data-quality-checks.md`
- `anomaly-detection-integration.md` → rename to `PRODUCT-16282-anomaly-detection-integration.md`

### Value Packs (VPs)

Value Pack files follow the same convention:
```
PRODUCT-XXXXX-pack-name.md
```

**Examples:**
- `PRODUCT-16000-data-observability-mvp.md`
- `PRODUCT-16100-advanced-monitoring.md`

## Creating New Value Increments

1. Copy `templates/VALUE_INCREMENT_TEMPLATE.md` to `value-increments/`
2. Name it following the convention above
3. Update the YAML frontmatter:
   - `key`: Add PRODUCT-XXXXX when Jira issue is created (leave as placeholder initially)
   - `summary`: Write a feature-focused title describing the capability
   - `status`: Set the current stage (default: `Open`)
4. Fill in the VI details progressively (Idea → Why → What → How)
5. Link to parent Value Pack in the "Parent" section
6. Rename the file if needed to include the Jira ID when assigned

## Document Structure

Each Value Increment document includes:

**YAML Frontmatter:**
```yaml
---
key: PRODUCT-XXXXX  # Jira issue key (assigned on creation)
summary: <Feature-focused title>
status: Open  # Current workflow stage
---
```

**Content Sections:**
- **Parent** — Link to parent Value Pack
- **Idea (Open)** — Short abstract and experience statement
- **Why (Problem stated)** — Human challenge, pain points, personas, competitive context
- **What (Use case defined)** — Scenarios, surfaces, scope
- **How (Ready for implementation)** — Deliverables, requirements, acceptance criteria

## Workflow

Value Increments progress through these stages (update the `status` field in the YAML frontmatter):

- **Open** — Accepted for consideration
- **Problem stated** — Why/pain points clarified
- **Use case defined** — What/scenarios documented
- **Ready for implementation** — How/requirements complete
- **In progress** — Being developed
- **Done** — Shipped and validated
