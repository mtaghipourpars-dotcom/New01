# Skill Registry

## Discovery Metadata

The discovery layer exposes only:

```xml
<available_skills>
  <skill>
    <name>app-scaffold</name>
    <description>Use this skill when the user wants to initialize the application's core structure, routing, and design tokens.</description>
    <location>/.agents/skills/app-scaffold/SKILL.md</location>
  </skill>
  <skill>
    <name>data-viz-engine</name>
    <description>Use this skill when the user needs charts, graphs, dashboards, or any data visualization. Even if they say "show data" or "make it visual."</description>
    <location>/.agents/skills/data-viz-engine/SKILL.md</location>
  </skill>
  <skill>
    <name>qc-gate</name>
    <description>Use this skill after every feature implementation to run quality control checkpoints. Also use when user says "check quality" or "validate this."</description>
    <location>/.agents/skills/qc-gate/SKILL.md</location>
  </skill>
</available_skills>
```

## Activation Rules

| Skill | Activate when |
|---|---|
| app-scaffold | application initialization, core structure, routing, design tokens |
| data-viz-engine | charts, dashboards, graphs, visual data presentation |
| qc-gate | after every feature, or explicit validation request |

## Multi-Skill Workflows

For a dashboard task:
- activate `app-scaffold` where project structure is involved
- activate `data-viz-engine` for chart work
- activate `qc-gate` after implementation
