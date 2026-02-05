# AGENTS.md

This repository is a governance framework for AI-assisted development.

## First: establish context
Before making changes, read:
- README.md
- ARCHITECTURE.md
- DECISIONS.md
- ai/README.md
- ai/rules.md
- ai/context.md
- ai/workflow.md
- ai/checklists/

## How to work in this repo
- Keep changes small, safe, and easy to review.
- Prefer existing patterns; avoid introducing new dependencies.
- Be explicit about tradeoffs, risk, and operational impact.
- If context is missing, ask questions or propose assumptions clearly.

## Safety / boundaries
- Never generate, request, or print secrets (tokens, API keys, credentials).
- Treat authz/authn, crypto, and compliance logic as high risk.
- Do not auto-run destructive commands. If needed, explain and request confirmation.

## Quality gates
Use these before finalizing a change:
- ai/checklists/security.md
- ai/checklists/reliability.md
- ai/checklists/performance.md
- ai/checklists/pr_review.md

Exceptions are allowed only if reason, risk, and mitigation are documented.

## Operational workflow (important)
All AI agents MUST follow the collaboration and PR workflow defined in:
- **ai/workflow.md**

This includes:
- PR size guardrails
- single-branch iteration rules
- Fix Pack handling for review feedback
- Definition of Done for agent PRs

## Common commands (fill in per project)
- Install deps: `<command>`
- Run tests: `<command>`
- Lint/format: `<command>`

## Notes
RETRO.md is a shared space for reflective notes.
Only add entries to RETRO.md when explicitly invited by a human.
Do not treat notes as tasks, decisions, or recommendations.
