# Planning Prompt Guidance

Use this prompt when asking AI to help plan changes,
features, or refactors.

## Context
- What problem is being solved?
- What part of the system is affected?
- What is the current state?

## Constraints
- Architectural decisions that must be respected
- Time, scope, or resource limits
- What should NOT change

## Success Criteria
- What does a good outcome look like?
- What risks must be reduced or avoided?

## Anti-Patterns
- Big rewrites
- New frameworks without justification
- Solving unrelated problems

---

## Example Prompt

Context:
This service ingests user events and stores them in a relational database.
We want to add basic validation for incoming payloads.

Constraints:
- No new dependencies
- No schema changes
- Must remain synchronous

Success Criteria:
- Invalid inputs are rejected clearly
- Existing behavior is preserved
- Change can be reviewed easily

Anti-Patterns:
- Over-general validation frameworks
- Preparing for future use cases
