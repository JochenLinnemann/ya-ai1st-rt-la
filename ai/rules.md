# AI Rules

1. Keep solutions simple and explicit
2. Prefer existing patterns
3. Minimize dependencies
4. Optimize for maintainability
5. Surface uncertainty
6. Avoid premature optimization
7. Respect cost and operational impact

## Examples

❌ Bad:
"Rewrite this module to be more scalable"

✅ Good:
"Extract the parsing logic into a pure function and add unit tests.
Do not change behavior."

## Cost Guardrails

AI suggestions should be rejected if they:
- Introduce always-on infrastructure without justification
- Increase steady-state cost by more than ~5–10% for marginal gains
- Add paid third-party services for convenience only

Cost tradeoffs should be documented explicitly.

## No "Down the Rabbit Hole"

Before making changes, restate the goal in one sentence.
If the proposed change does not directly advance that goal, stop and ask.

You have at most three iterations to propose the smallest viable change.
Do not explore alternatives unless asked.

Do not combine:
- Refactoring + new behavior
- Performance changes + readability changes
- Dependency changes + logic changes

After proposing a solution, include:
- Summary (3 bullets)
- Why this is sufficient
- What is intentionally left out
- A recommendation: STOP or CONTINUE

If a change introduces a new tradeoff or long-term implication,
stop and propose a DECISIONS.md entry instead of continuing.

When uncertain whether additional work adds value, stop and ask.

## Notes

RETRO.md is a shared space for reflective notes.
Only add entries to RETRO.md when explicitly invited by a human.
Do not treat notes as tasks, decisions, or recommendations.
