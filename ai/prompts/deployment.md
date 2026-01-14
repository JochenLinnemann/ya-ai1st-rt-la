# Deployment Prompt Guidance

Use this prompt when planning or reviewing deployment-related changes.

## Context
- How is the system currently deployed?
- What is changing?

## Constraints
- Prefer reversible changes
- Avoid downtime if possible
- Respect infrastructure cost limits

## Success Criteria
- Rollback path is clear
- Failure modes are understood
- Operational risk is minimized

## Anti-Patterns
- Irreversible migrations
- Assumptions of unlimited capacity
- “We’ll monitor it later”

---

## Example Prompt

Context:
We are adding a new configuration option to the service.

Constraints:
- No downtime deployment
- Must work with existing configs

Success Criteria:
- Old configs remain valid
- Rollback is trivial

Anti-Patterns:
- Hard-coded defaults
- Manual deployment steps
