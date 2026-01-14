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

## Common commands (fill in per project)
- Install deps: `<command>`
- Run tests: `<command>`
- Lint/format: `<command>`
