# Project Charter

## Product Identity

**Application:** [Application Name]

**Working model:** Professional-Grade Agent Skill-Driven Application

**Primary delivery environment:** Google AI ecosystem / Firebase-oriented workflow

## Core Objective

Build the application using a progressive-disclosure Agent Skills structure and a strict feature-by-feature QC process.

## Primary Principles

1. Visual-first presentation.
2. Progressive disclosure of development knowledge.
3. No un-QC'd code in the deliverable.
4. Bilingual EN/FA support.
5. Correct RTL behavior under FA.
6. Requirement-to-implementation traceability.
7. Evidence-backed completion status.
8. Continuous comparison-map maintenance.

## Non-Negotiable Technology Baseline

| Layer | Required technology |
|---|---|
| Framework | Next.js 15, App Router |
| UI | Shadcn/ui + Tailwind CSS |
| Charts | Recharts + D3 on demand |
| Client state | Zustand + React Query |
| Backend / DB | Firebase Firestore + Auth |
| Forms / validation | React Hook Form + Zod |
| Motion | Framer Motion |
| i18n | next-intl |

## Primary Quality Rule

A feature is not complete because implementation exists. It is complete only when the feature passes the applicable QC gates and the evidence is recorded.
