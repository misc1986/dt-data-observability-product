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
3. Fill in the VI details progressively (Idea → Why → What → How)
4. Update the Jira ID when the issue is created
5. Rename the file if needed to include the Jira ID

## Workflow

Value Increments progress through these stages:
- **Idea** — Initial concept
- **Open** — Accepted for consideration
- **Problem stated** — Why/pain points clarified
- **Use case defined** — What/scenarios documented
- **Ready for implementation** — How/requirements complete
- **In progress** — Being developed
- **Done** — Shipped and validated

Update the `Status` field in each VI document as it progresses.
