# AI Prompting Guide

## 1. Structured Prompt Embedding

Use XML blocks:

```xml
<role>Senior Full-Stack Engineer</role>
<constraints>
1. No external UI libraries beyond Shadcn/Tailwind/Recharts.
2. All text must go through next-intl.
3. Charts must render with SSR fallback.
</constraints>
<context>
[Insert component code or specification here]
</context>
<task>
Implement the required feature.
</task>
```

## 2. Long-Context Anchoring

Order:
1. all context
2. transition phrase
3. task

Use:

> Based on the above information, perform the following task:

## 3. Reasoning Enhancement

For complex logic, request:

> Before starting to code, explain your implementation approach and potential pitfalls in 3 sentences.

## 4. Strictly Grounded Mode

For bug fixes:

```text
You are a strictly grounded assistant limited to the information provided in the User Context.
Rely only on the facts directly mentioned.
Do not use your own knowledge or common sense.
If the exact fix is not explicitly derivable from the provided code and error log,
state that the information is not available.
```

## 5. Service Configuration Requests

When implementation depends on external services, require explicit console configuration steps in the AI output.

The output must state where to navigate, what to enable, and what value/configuration to apply.
