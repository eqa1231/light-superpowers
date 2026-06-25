---
name: light-superpowers
description: Use when the user explicitly asks for light-superpowers, a lighter Superpowers workflow, task-scaled execution, or to avoid full brainstorming/planning/TDD/subagent ceremony while still keeping engineering discipline.
---

# Light Superpowers

## Core Rule

Use the smallest workflow that protects the work.

Do not turn routine tasks into full ceremonies. Keep project-specific rules, user instructions, and safety constraints above this skill. This skill controls pace and verification only; it does not override repository architecture, security, legal, product, or style rules.

## Task Tiers

| Tier | Use For | Workflow |
| --- | --- | --- |
| XS | Questions, command output, file lookup, explanation | Answer or run the direct check |
| S | Single-file edits, typo fixes, small config changes | Inspect context, edit, run the nearest useful verification |
| M | Multi-file feature or bugfix with clear requirements | State a short plan, implement, verify changed behavior |
| L | Cross-module, architecture, data migration, production-risk work | Ask only blocking questions, write a real plan, broaden tests and review |
| Debug | Broken behavior, failing tests, unclear cause | Reproduce, isolate, fix root cause, verify regression coverage when practical |

Default to the lighter tier when risk is low and requirements are clear. Escalate one tier when the task touches shared abstractions, persistence, auth, money, irreversible data changes, or public APIs.

## Operating Rules

- Follow direct user instructions first.
- Follow project `AGENTS.md`, `CLAUDE.md`, rules, and local conventions next.
- Do not use full brainstorming, design documents, subagents, worktrees, or branch-finishing flows unless the tier is L or the user asks.
- Do not spawn subagents unless the user explicitly asks for delegation or parallel agents.
- Do not force TDD for every edit. Use test-first for bug fixes, core business logic, high-risk behavior, or when the project requires it.
- Keep progress updates short. Explain what is being checked, changed, or verified.
- Ask questions only when a reasonable assumption would be risky or business logic is genuinely unclear.
- Prefer local, targeted verification over broad test suites for XS/S tasks.
- Use broader verification for M/L tasks or when targeted tests reveal suspicious failures.

## Lightweight Workflow

1. Classify the task tier silently unless the tier affects the user's choice.
2. Read the minimum context needed to avoid guessing.
3. For M/L tasks, give a short plan before edits.
4. Make focused changes that match existing patterns.
5. Verify with the closest meaningful command or manual check.
6. Before final response, report what changed, what passed, and any verification that could not be run.

## Escalation Triggers

Move to a heavier process when any of these are true:

- Requirements conflict or are incomplete in a way that affects behavior.
- Multiple valid designs have meaningfully different tradeoffs.
- The change crosses service, aggregate, schema, authentication, payment, or permission boundaries.
- A failed verification points to a broader regression.
- The user asks for a plan, spec, code review, branch workflow, or formal TDD.

## Output Style

For XS/S tasks, final responses should usually be one short paragraph plus the verification result.

For M tasks, use a compact list of changed files and tests.

For L tasks, include the plan, risk notes, verification summary, and follow-up options.

Never end in a known-bad state. If verification fails, either fix the cause or clearly report the blocker and the exact failing check.

## Common Mistakes

| Mistake | Correction |
| --- | --- |
| Loading every workflow because a skill exists | Use only the tier needed for the current risk |
| Writing a long plan for a tiny change | Inspect, edit, verify, summarize |
| Skipping verification to stay light | Keep verification small, not absent |
| Asking broad questions before reading code | Read local context first, then ask only blocking questions |
| Replacing project rules with this skill | Project rules remain authoritative |
