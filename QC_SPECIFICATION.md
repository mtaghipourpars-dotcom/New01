# QC Specification

## QC-1 — Code Cleanliness

Every feature must verify:

- no `console.log`, except temporary development debugging removed before commit
- no `any` types under TypeScript strict mode
- no unused imports
- component files under 250 lines
- every `useEffect` has cleanup or a complete dependency array

## QC-2 — Visualization Verification

Verify:

- feature contains an applicable chart/graphic element
- data is presented visually where required
- charts are responsive
- design-token colors are used

## QC-3 — Bilingual Verification

Verify:

- all user-visible strings use translation keys
- FA RTL layout works
- charts/forms/navigation mirror correctly where required
- localized number/date formatting works

## QC-4 — Interaction Completeness

Verify:

- loading uses skeletons
- errors provide visual feedback
- empty state provides guiding visuals
- keyboard navigation is available

## Execution

The prompt requires:

```bash
npm run qc
```

implemented through:

```text
/.agents/skills/qc-gate/scripts/run-qc.sh
```

## Failure Policy

If a QC gate fails:
1. stop progression
2. fix the issue
3. rerun QC
4. update evidence
5. only then continue
