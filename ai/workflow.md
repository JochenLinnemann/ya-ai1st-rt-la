# ai/workflow.md

This document defines how AI agents collaborate with humans
when implementing and reviewing changes in this repository.

GitHub is the system of record.
AI agents are workers, not owners.

---

## PR Size Guardrail

Target:
- **10–15 changed files per PR**

If a change exceeds this:
- split into:
  - PR A: mechanical / preparatory changes
  - PR B: behavioral / semantic changes
- OR stop and ask for guidance in the PR description.

---

## Two-Agent Handshake (Default)

To avoid “review finds issues that could have been prevented”:

1) **Builder pass**
   - Implement the requested change
   - Stay strictly within scope

2) **Reviewer pass**
   - Perform a fresh review (checklists, security, edge cases)
   - Apply obvious fixes before human review

If GitHub Copilot Review is available, treat it as the reviewer pass.

---

## Definition of Done for Agent PRs

A PR is ready for human review only when it includes:
- **Summary**: what changed and why
- **Risk**: what could break
- **How to verify**: tests or manual steps

Additionally:
- No unrelated refactors
- No noisy diffs
- Sensitive logging avoided
- Config changes documented

---

## Handling Review Feedback (Avoid Merge Hell)

### Golden Rule
**Prefer one PR branch for multiple fixes.**

Do NOT trigger per-thread automated fixes when more than one issue exists.

---

## Fix Pack Workflow (Required for multiple fixes)

When a PR has more than one requested change:

1) A human aggregates feedback into ONE top-level comment
2) The agent applies all fixes **in the same PR branch**
3) Multiple commits are allowed; multiple branches are not

### Fix Pack Template

```md
## Fix Pack v1 (single-branch)

@codex, please fix the following in THIS PR BRANCH.

Constraints:
- Do not open new PRs
- Do not create new branches
- Multiple commits are allowed

### Changes
1. …
2. …
3. …

### Acceptance
- Build passes
- Manual test: …
- No unrelated refactors
```
