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
