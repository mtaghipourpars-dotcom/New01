# RAIL CONTROL TOWER — Agent Skill-Driven Application Documentation Pack v1.0

## 1. Purpose

This package converts the attached build prompt into a complete documentation baseline for a professional-grade, Agent Skill-driven application.

The package defines:
- Progressive Disclosure skill architecture
- Required technology and project conventions
- Visual-first UI/UX rules
- Bilingual EN/FA and RTL requirements
- QC gates and evidence rules
- Requirement-to-implementation traceability
- Google AI execution conventions
- Delivery protocol and acceptance criteria
- Skill files for `app-scaffold`, `data-viz-engine`, and `qc-gate`

The prompt requires the same order of work: skill discovery/activation, project initialization, dashboard-first implementation, QC after every feature, continuous comparison mapping, and final bilingual/RTL verification.

## 2. Package Structure

```text
RAIL_CONTROL_TOWER_Agent_Skill_Documentation_Pack_v1/
├── README.md
├── README.dm
├── PROJECT_CHARTER.md
├── ARCHITECTURE_BASELINE.md
├── EXECUTION_PROTOCOL.md
├── UI_UX_SPECIFICATION.md
├── BILINGUAL_RTL_SPECIFICATION.md
├── DATA_VIZ_SPECIFICATION.md
├── QC_SPECIFICATION.md
├── ACCEPTANCE_CRITERIA.md
├── COMPARISON_MAP.md
├── AI_PROMPTING_GUIDE.md
├── SKILL_REGISTRY.md
├── .agents/
│   └── skills/
│       ├── app-scaffold/
│       │   └── SKILL.md
│       ├── data-viz-engine/
│       │   └── SKILL.md
│       └── qc-gate/
│           └── SKILL.md
├── messages/
│   ├── en.json
│   └── fa.json
└── evidence/
    ├── README.md
    └── .gitkeep
```

## 3. How to Execute

### Phase 0 — Load the project specification
Read the documents in this order:

1. `PROJECT_CHARTER.md`
2. `ARCHITECTURE_BASELINE.md`
3. `SKILL_REGISTRY.md`
4. `EXECUTION_PROTOCOL.md`
5. `UI_UX_SPECIFICATION.md`
6. `BILINGUAL_RTL_SPECIFICATION.md`
7. `DATA_VIZ_SPECIFICATION.md`
8. `QC_SPECIFICATION.md`
9. `ACCEPTANCE_CRITERIA.md`
10. `COMPARISON_MAP.md`

Then activate the relevant `SKILL.md` files.

### Phase 1 — Initialize the application
Create or initialize the Next.js 15 App Router project and install the specified stack:

- Next.js 15
- Shadcn/ui
- Tailwind CSS
- Recharts
- D3 on demand
- Zustand
- React Query
- Firebase Firestore/Auth
- React Hook Form
- Zod
- Framer Motion
- next-intl

No feature is considered complete merely because its files compile.

### Phase 2 — Implement the first module
The first feature is the Dashboard/Home experience.

The first screen must satisfy the prompt's visual constraints:
- at least 3 real-time chart components
- charts occupy 60%+ of the first screen area
- visual-first presentation
- responsive behavior
- no hardcoded user-visible strings
- bilingual EN/FA support
- RTL behavior under FA

### Phase 3 — Mandatory QC Gate
After every feature module:

```bash
npm run qc
```

Do not move to the next module until QC-1 through QC-4 pass.

Any failed gate requires correction before progression.

### Phase 4 — Update traceability
Immediately after each module, update:

```text
COMPARISON_MAP.md
```

Every `✅` requires evidence:
- screenshot, or
- test reference, or
- QC terminal output

No evidence = no `✅`.

### Phase 5 — Continue module by module
Follow the project execution order defined in `EXECUTION_PROTOCOL.md`.

### Phase 6 — Final verification
Run:

```bash
npm run qc
```

Then run:
- bilingual smoke tests
- RTL screenshot comparison
- final evidence review
- final Comparison Map verification

## 4. Required Delivery Condition

A deliverable is accepted only when:
- all required documentation exists
- all required skills exist
- all user-visible strings use translations
- EN and FA translations are complete
- RTL layout is verified
- charts are responsive
- QC gates pass
- comparison-map status is evidence-backed
- final evidence is stored under `evidence/`

## 5. Important Boundary

This package is the documentation and execution-control baseline. It does not claim that the application itself has been implemented or QC-passed.
