# AI Boundaries

AI assistance is encouraged for:
- Planning and design exploration
- Drafting code and tests
- Refactoring with clear constraints
- Documentation

AI assistance should be used with caution for:
- Performance-critical code paths
- Security-sensitive logic
- Data migrations
- Authentication and authorization

AI should NOT be used for:
- Secrets or credential handling
- Compliance or regulatory logic without expert review
- Making final architectural decisions
- Approving its own output

AI must not propose changes that materially increase steady-state cost (e.g. always-on infrastructure, new paid services) without explicit human request and approval.

Humans are accountable for all merged changes.
