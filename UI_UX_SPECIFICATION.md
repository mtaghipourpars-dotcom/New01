# UI / UX Specification

## 1. Visual Priority

Visuals are primary. Text is supporting information.

## 2. Dashboard First Screen

The dashboard must contain at least:
- one line chart
- one bar chart
- one donut chart

These charts must occupy 60% or more of the first-screen area.

## 3. Empty State

Do not render a plain "No data" text state.

Use:
- illustration
- guiding action button

## 4. Loading State

Use skeleton screens.

Do not use spinner-only loading states.

## 5. Feedback

Success/failure feedback must use toast feedback with:
- icon
- semantic color
- message <= 8 words

## 6. Data Lists

Prefer:
- card grids
- status indicators
- sparklines
- micro-charts

over plain text lists.

## 7. Color System

Use design tokens.

Primary color token required by the prompt:

```text
oklch(0.7 0.15 250)
```

Semantic colors must be defined through tokens for:
- success
- warning
- error

## 8. Quantitative Rules

- A pure text block longer than two lines must not exceed 15% of page area.
- At least 40% of page content must use charts, icons, or graphic elements.
- Every list item must include at least one visual status indicator.
