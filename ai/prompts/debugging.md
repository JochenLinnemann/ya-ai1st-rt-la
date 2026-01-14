# Debugging Prompt Guidance

Use this prompt when investigating a bug or unexpected behavior.

## Context
- What is failing?
- Where was the issue observed?
- Is it reproducible?

## Constraints
- Do not change behavior without understanding the cause
- Avoid speculative fixes

## Success Criteria
- Root cause is identified
- Fix is minimal and targeted
- Regression risk is low

## Anti-Patterns
- Trial-and-error fixes
- Refactoring while debugging
- Masking errors instead of fixing causes

---

## Example Prompt

Context:
Requests intermittently return 500 errors under moderate load.

Constraints:
- No architectural changes
- No performance optimizations yet

Success Criteria:
- Identify the failure path
- Propose a minimal fix
- Suggest a regression test

Anti-Patterns:
- Rewriting request handling
- Adding retries without diagnosis
