# Data Visualization Specification

## 1. Activation Rule

Any feature requiring:
- charts
- graphs
- dashboards
- data visualization
- visual data presentation

must activate `data-viz-engine`.

## 2. Chart Stack

Primary:

```text
Recharts
```

Use D3 only when the visualization requires capabilities beyond the standard chart layer.

## 3. Dashboard Minimum

The first screen must have:
- line chart
- bar chart
- donut chart

## 4. Visual Data Rules

Charts must:
- be responsive
- use design tokens
- use translated labels
- avoid hardcoded visible strings
- remain usable in EN and FA

## 5. Data Cards

Data cards should use visual indicators such as:
- progress bar
- sparkline
- status color block
- micro-chart

## 6. SSR / Rendering Constraint

Chart implementations must provide the required fallback behavior described in the AI prompt and must not rely on uncontrolled browser-only rendering for the main layout.

## 7. Evidence

For each accepted visualization requirement, store visual proof under:

```text
evidence/
```
