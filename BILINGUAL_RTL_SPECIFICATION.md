# Bilingual / RTL Specification

## 1. Framework

Use:

```text
next-intl
```

## 2. Language Detection

- auto-detect browser language
- provide manual language switching
- language control is positioned in the top-right according to the locale-aware layout

## 3. Routes

```text
/[locale]/dashboard
/[locale]/reports
```

## 4. Locale Direction

### English
```text
dir="ltr"
```

### Persian
```text
dir="rtl"
```

Under FA:
- layout is mirrored
- navigation is mirrored
- forms are mirrored
- chart axes are mirrored where applicable

## 5. Translation Files

```text
messages/en.json
messages/fa.json
```

No missing translation keys are allowed.

## 6. Number and Date Formatting

Use:

```text
Intl.NumberFormat
Intl.DateTimeFormat
```

Formatting must follow the active locale.

## 7. Charts

Chart labels must be translated through i18n hooks.

Do not hardcode chart labels inside chart components.

## 8. Verification

The following must be tested:
- EN visual smoke test
- FA visual smoke test
- RTL screenshot comparison
- translated labels on every chart
- localized number/date rendering
