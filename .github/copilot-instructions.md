# GitHub Copilot – Repository Instructions

This repository is a governance framework for AI-assisted development.
Prefer minimal, incremental changes. Keep solutions simple and explicit.

## Sources of truth (read first)
- README.md
- ARCHITECTURE.md
- DECISIONS.md
- ai/README.md
- ai/rules.md
- ai/context.md
- ai/checklists/

## Working style
- Ask clarifying questions when context is missing.
- Prefer existing patterns in this repo over “best practice” rewrites.
- Minimize dependencies and operational complexity.
- Surface uncertainty explicitly and propose verification steps.

## Guardrails
- Do not introduce new frameworks without explicit request.
- Do not make large refactors without an agreed plan.
- Do not generate or request secrets. Never include credentials in code or logs.
- Treat security/auth/permissions changes as high risk: require human review.

## Quality gates
Before proposing a PR-ready change, use relevant checklists:
- ai/checklists/security.md
- ai/checklists/reliability.md
- ai/checklists/performance.md
- ai/checklists/pr_review.md

If any checklist item is intentionally not met, document reason, risk, mitigation.
