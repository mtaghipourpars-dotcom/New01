# Execution Protocol

## Required Sequence

### Step 1 — Read and register skills

Read the full prompt and confirm:

```text
/.agents/skills/app-scaffold/SKILL.md
/.agents/skills/data-viz-engine/SKILL.md
/.agents/skills/qc-gate/SKILL.md
```

Expose only metadata during discovery.

### Step 2 — Initialize the project

Initialize Next.js 15 with App Router and configure the specified stack.

### Step 3 — Implement core layout + Dashboard

The Dashboard/Home screen is implemented first.

Required first-screen visual content:
- minimum 3 real-time chart components
- chart-heavy layout
- data cards / micro-visuals
- responsive behavior

### Step 4 — Run QC

Run QC-1 through QC-4.

```bash
npm run qc
```

Do not continue if a gate fails.

### Step 5 — Update Comparison Map

Update every dashboard requirement line-by-line and attach evidence.

### Step 6 — Implement next module

The prompt identifies:
- Reports
- Data management
- Settings

Continue with the same QC → evidence → comparison-map loop.

### Step 7 — Final delivery

Run:

```bash
npm run qc
```

Also execute:
- bilingual smoke tests
- RTL screenshot comparison
- evidence review
- final comparison-map review

## Prohibitions

- Do not mark `✅` without evidence.
- Do not skip QC.
- Do not hardcode user-visible strings.
- Do not create chart code without activating `data-viz-engine`.
- Do not proceed after a failed QC gate.
