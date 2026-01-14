# Refactoring Prompt Guidance

Use this prompt when improving structure without changing behavior.

## Context
- What is hard to understand or maintain?
- Why is refactoring needed now?

## Constraints
- Behavior must not change
- Scope must remain small

## Success Criteria
- Code is easier to read
- Tests still pass
- Changes are reviewable

## Anti-Patterns
- Mixing refactoring with feature changes
- Abstracting for hypothetical future needs

---

## Example Prompt

Context:
This function has grown too large and mixes validation with persistence.

Constraints:
- No new abstractions
- No behavior changes

Success Criteria:
- Clear separation of responsibilities
- Existing tests still pass

Anti-Patterns:
- Introducing generic utility layers
- Renaming everything at once
