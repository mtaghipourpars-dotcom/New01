# Requirement-Implementation Comparison Map

> Auto-generated + manually maintained. Last updated: TBD

## Status Legend

| Symbol | Meaning | Required action |
|---|---|---|
| ✅ | Fully implemented | Evidence required |
| ⚠️ | Partially implemented | Fix plan or known limitation required |
| ❌ | Not implemented | Blocking |
| 🔄 | In progress | Not deliverable |

## Evidence Rule

Every `✅` must include at least one:
- `./evidence/<module>-<id>.png`
- specific test reference
- QC terminal output

## Module: Architecture / Skills

| Req ID | Requirement | Requirement (FA) | Implementation File | Status | Evidence |
|---|---|---|---|---|---|
| A-01 | Three required skills exist | سه Skill اصلی وجود دارند | `/.agents/skills/**/SKILL.md` | 🔄 | TBD |
| A-02 | Progressive disclosure is followed | معماری Progressive Disclosure رعایت شود | `ARCHITECTURE_BASELINE.md` | 🔄 | TBD |

## Module: Dashboard

| Req ID | Requirement | Requirement (FA) | Implementation File | Status | Evidence |
|---|---|---|---|---|---|
| D-01 | Show 3 real-time charts on first screen | نمایش ۳ نمودار زنده در صفحه اول | `app/[locale]/dashboard/page.tsx` | 🔄 | TBD |
| D-02 | Charts occupy 60%+ of first-screen area | نمودارها بیش از ۶۰٪ صفحه اول را اشغال کنند | dashboard chart layout | 🔄 | TBD |
| D-03 | Charts are bilingual | نمودارها دوزبانه باشند | chart translation layer | 🔄 | TBD |
| D-04 | Data cards contain visual status indicators | کارت‌های داده شاخص بصری داشته باشند | data cards | 🔄 | TBD |

## Module: Bilingual / RTL

| Req ID | Requirement | Requirement (FA) | Implementation File | Status | Evidence |
|---|---|---|---|---|---|
| I-01 | Browser language detection | تشخیص زبان مرورگر | next-intl configuration | 🔄 | TBD |
| I-02 | Manual language switching | تغییر دستی زبان | locale switcher | 🔄 | TBD |
| I-03 | RTL under FA | RTL در فارسی | locale layout | 🔄 | TBD |
| I-04 | Locale-aware dates and numbers | تاریخ و عدد وابسته به زبان | formatting utilities | 🔄 | TBD |

## Module: QC

| Req ID | Requirement | Requirement (FA) | Implementation File | Status | Evidence |
|---|---|---|---|---|---|
| Q-01 | `npm run qc` exists | دستور QC وجود داشته باشد | package script / QC skill | 🔄 | TBD |
| Q-02 | QC-1 through QC-4 enforced | چهار دروازه QC اجرا شوند | `/.agents/skills/qc-gate/**` | 🔄 | TBD |

## Module: Reports

| Req ID | Requirement | Requirement (FA) | Implementation File | Status | Evidence |
|---|---|---|---|---|---|
| R-01 | Reports page exists | صفحه Reports وجود داشته باشد | `app/[locale]/reports/**` | 🔄 | TBD |

## Rule

Do not change a status to `✅` until verification evidence exists.
