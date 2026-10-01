# Architecture Baseline

## 1. Progressive Disclosure Layers

### Layer 1 — Skill Discovery

The model initially exposes only skill metadata:
- name
- description
- location

### Layer 2 — Skill Activation

When a request matches a skill, read its full `SKILL.md` and execute it.

For multi-step workflows, activate multiple applicable skills.

### Layer 3 — Resource Loading

Skills may load:
- `scripts/`
- `references/`
- `assets/`
- `examples/`

References are resolved relative to the parent directory of `SKILL.md`.

## 2. Required Skill Set

```text
/.agents/skills/
├── app-scaffold/
│   └── SKILL.md
├── data-viz-engine/
│   └── SKILL.md
└── qc-gate/
    └── SKILL.md
```

## 3. Application Routing

The prompt requires locale-aware routes:

```text
/[locale]/dashboard
/[locale]/reports
```

## 4. Translation Files

```text
messages/en.json
messages/fa.json
```

All user-visible strings must use semantic translation keys.

## 5. Quality Evidence

```text
evidence/
```

Evidence can be:
- screenshots
- test references
- QC terminal output

## 6. Traceability

The project root contains:

```text
COMPARISON_MAP.md
```

It is the single source of truth for requirement implementation status.

## 7. Technology Boundary

The attached prompt specifies the technology stack and implementation constraints. This document does not replace those constraints with alternate libraries.
