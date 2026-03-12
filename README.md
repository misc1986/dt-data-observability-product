# Data Observability Product Documentation

This repository contains structured product documentation for Data Observability Value Packs and Value Increments.

## Folder Structure

```
dt-data-observability-product/
├── templates/
│   └── VALUE_INCREMENT_TEMPLATE.md    # Template for creating new VIs
├── value-increments/                   # Individual deliverable features
│   ├── PRODUCT-XXXXX-feature-name/     # VI folder (with or without Jira ID)
│   │   ├── increment.md                # Main VI document
│   │   └── artifacts/                  # Supporting materials
│   │       ├── architecture-draft.md
│   │       ├── discovery-notes.md
│   │       └── demos/
│   └── another-feature/                # Without Jira ID initially
│       ├── increment.md
│       └── artifacts/
├── value-packs/                        # Collections of related VIs
│   └── PRODUCT-XXXXX-pack-name.md
└── README.md                           # This file
```

## Naming Conventions

### Value Increments (VIs)

Each VI is a folder containing the main document (`increment.md`) and supporting artifacts:

**Folder naming patterns:**

**With Jira ID:**
```
value-increments/PRODUCT-XXXXX-short-kebab-case-description/
```

**Without Jira ID (initially):**
```
value-increments/short-kebab-case-description/
```

**Guidelines:**
- Use lowercase kebab-case for folder names
- Keep folder names under 50 characters
- Main VI document is always named `increment.md`
- Store supporting materials in `artifacts/` subdirectory
- Rename folder when Jira ID is assigned

**Examples:**
- `value-increments/PRODUCT-16280-pipeline-observability/increment.md`
- `value-increments/PRODUCT-16281-data-quality-checks/increment.md`
- `value-increments/anomaly-detection/` → rename to `value-increments/PRODUCT-16282-anomaly-detection/`

### Value Packs (VPs)

Value Pack files follow the same convention:
```
PRODUCT-XXXXX-pack-name.md
```

**Examples:**
- `PRODUCT-16000-data-observability-mvp.md`
- `PRODUCT-16100-advanced-monitoring.md`

## Creating New Value Increments

1. Create a new folder in `value-increments/` with kebab-case name:
   - Without Jira: `value-increments/feature-name/`
   - With Jira: `value-increments/PRODUCT-XXXXX-feature-name/`
2. Copy `templates/VALUE_INCREMENT_TEMPLATE.md` to `feature-name/increment.md`
3. Create `feature-name/artifacts/` folder for supporting materials
4. Update the metadata in `increment.md`:
   - **Key**: Add PRODUCT-XXXXX when Jira issue is created (leave as placeholder initially)
   - **Status**: Set the current stage (default: `Open`)
   - **Value Pack**: Link to parent Value Pack with PRODUCT-XXXXX — [Name]
5. Fill in the VI details progressively (Idea → Why → What → How)
6. Rename the folder if needed to include the Jira ID when assigned

**Artifacts folder:** Store discovery notes, architecture drafts, diagrams, demos, or other supporting materials in the `artifacts/` subdirectory to keep the main `increment.md` focused on the VI specification.

## Document Structure

Each Value Increment document includes:

**Metadata (blockquote at top):**
```markdown
> **Key:** PRODUCT-XXXXX *(optional — add when Jira issue is created)*  
> **Status:** <Open | Problem stated | Use case defined | Ready for implementation | In progress | Done>  
> **Value Pack:** PRODUCT-XXXXX — [Value Pack Name]
```

**Content Sections:**
- **Idea (Open)** — Short abstract and experience statement
- **Why (Problem stated)** — Human challenge, pain points, personas, competitive context
- **What (Use case defined)** — Scenarios, surfaces, scope
- **How (Ready for implementation)** — Deliverables, requirements, acceptance criteria

## Workflow

Value Increments progress through these stages (update the `Status` field in the metadata blockquote):

- **Open** — Accepted for consideration
- **Problem stated** — Why/pain points clarified
- **Use case defined** — What/scenarios documented
- **Ready for implementation** — How/requirements complete
- **In progress** — Being developed
- **Done** — Shipped and validated
