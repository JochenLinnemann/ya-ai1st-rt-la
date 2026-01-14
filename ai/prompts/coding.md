# Coding Prompt Guidance

A good coding prompt should include:

## Context
- What the system does
- Where this code fits

## Constraints
- Performance, cost, security, or compliance limits
- What must NOT change

## Success Criteria
- What does "done" look like?
- How will correctness be verified?

## Anti-Patterns
- What should explicitly be avoided?

---

## Example Prompt

Context:
This service processes user-submitted events and stores them in a database.

Constraints:
- Do not introduce new dependencies
- Keep the function synchronous
- No schema changes

Success Criteria:
- Input validation is explicit
- Errors are handled clearly
- Existing behavior is preserved

Anti-Patterns:
- No abstractions for future use
- No background jobs
