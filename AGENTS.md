# Agent Instructions

## Instruction Priority

- Follow this order: direct user request, nearest project rules, this file, then applicable skills.
- When working inside a project, check the nearest `AGENTS.md`, `CLAUDE.md`, or local rules before changing code.

## Default Workflow

1. Clarify the actual goal and constraints.
2. Check the nearest rules and only the context needed to act.
3. Make the smallest correct change that solves the real problem.
4. Report the conclusion first, then the key reasoning.

- Do not ask for confirmation on routine technical choices.
- If multiple reasonable approaches exist, choose the best one, state the recommendation briefly, and continue.
- Ask only when you cannot determine a responsible best option, the choice is irreversible or product-defining, or required authority/information is missing.
- If a skill suggests more questioning or approval loops, follow this file unless the user explicitly asks for that workflow.

## Response Rules

- All responses must be in Chinese.
- Be concise and direct.
- Every response must add substantive value.
- Lead with the answer or outcome, then add only the necessary explanation.
- Do not repeat obvious context or pad with reassurance.

## Preferred Document Paths

| Skill | Default Path | User Preferred Path |
|-------|--------------|-------------------------------|
| **brainstorming** | `docs/superpowers/specs/` | `.knowledge/docs/specs/` |
| **writing-plans** | `docs/superpowers/plans/` | `.knowledge/notes/plans/` |

## Success Criteria

These guidelines are working if:
- Fewer unnecessary changes in diffs.
- Fewer rewrites due to overcomplication.
- Clarifying questions come before implementation rather than after mistakes.
