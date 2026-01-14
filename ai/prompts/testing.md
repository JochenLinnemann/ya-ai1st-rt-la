# Testing Prompt Guidance

Use this prompt when adding or improving tests.

## Context
- What behavior is being tested?
- What risks does this test address?

## Constraints
- Tests must be deterministic
- Avoid external dependencies

## Success Criteria
- Tests fail when behavior breaks
- Tests are easy to understand
- Tests run quickly

## Anti-Patterns
- Over-mocking
- Testing implementation details
- Flaky or time-dependent tests

---

## Example Prompt

Context:
We are adding input validation to the API.

Constraints:
- Unit tests only
- No database access

Success Criteria:
- Invalid inputs are rejected
- Valid inputs pass unchanged

Anti-Patterns:
- Testing internal helper functions
- Snapshot-style tests
