# AI Usage Guide

This directory defines how AI agents should assist with this repository.

AI is expected to:
- Ask clarifying questions when context is missing
- Respect existing architecture and decisions
- Propose minimal, incremental changes
- Explain tradeoffs clearly

AI must NOT:
- Introduce unnecessary abstractions
- Add dependencies without justification
- Assume unlimited infrastructure resources

This directory provides default AI usage guidance.
Teams are expected to adapt, tighten, or extend these rules
based on domain, risk profile, and regulatory requirements.

## Asynchronous AI Usage

AI output may be generated asynchronously.
When reviewing AI-generated changes:
- Treat output as a draft, not a decision
- Reconstruct intent before modifying code
- Ask follow-up questions if context is missing
- Prefer understanding over speed
