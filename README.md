# Project Name

This repository is a **thinking framework**, not a runtime scaffold.

It exists to help teams use generative AI **deliberately, responsibly, and with clear intent** — minimizing accidental complexity while making tradeoffs explicit.

Empty files in this repository are intentional.  
They create space for decisions *as they are made*, not pressure to document everything up front.

---

## What This Repository Is

This repository is a **governance framework for AI-assisted software development**.

It provides:
- Shared norms for how AI is used (and where it should not be used)
- Lightweight structures for documenting decisions and tradeoffs
- Checklists that act as practical quality gates
- Prompt guidance that teaches teams how to think, not just what to ask

Think of it as a **constitution**, not a construction manual.

---

## What This Repository Is Not

This repository does **not**:
- Scaffold a working application
- Assume a programming language, framework, or cloud provider
- Provide a runnable example service
- Replace your existing repository structure

It is intentionally **language-agnostic, stack-agnostic, and tool-agnostic**.

---

## How to Use This Repository

You do not “fill this out” all at once.  
You adopt it **incrementally**, as the system and team evolve.

### Option 1: Overlay on an Existing Repository (Recommended)

1. Copy the `ai/` directory into your existing repo
2. Reference the checklists during PR reviews
3. Use the prompt templates to structure AI interactions
4. Add entries to `DECISIONS.md` as real decisions are made

This works especially well for brownfield systems.

---

### Option 2: Start a New Repository with It

1. Create a new repo from this template
2. Add code under `src/` and `tests/`
3. Keep documentation lightweight until it provides value
4. Let `DECISIONS.md` and `ROADMAP.md` grow organically over time

Avoid filling files “just to fill them.”

---

### Option 3: Partial Adoption

You can adopt only what you need:
- Just the AI checklists
- Just the prompt structure
- Just the decision log

Partial adoption is expected and supported.

---

## Project Overview

Use this section to describe *your* project:

- What problem it solves
- Who it is for
- What success looks like

This repository is structured to support **human + AI collaboration** while prioritizing simplicity, maintainability, and responsible use of infrastructure resources.

---

## Goals

- Make intent and tradeoffs explicit
- Encourage small, incremental changes
- Keep operational impact visible
- Enable safe, transparent AI assistance

---

## Non-Goals

- Premature optimization
- Over-engineering
- Undocumented “magic”
- AI-driven decision-making without human accountability

---

## Getting Started

Document how to:
- Run the project locally
- Execute tests
- Deploy (if applicable)

Keep this practical and minimal.

---

## Key Documentation

- Architecture overview: `ARCHITECTURE.md`
- Architectural decisions: `DECISIONS.md`
- AI usage guidance: `ai/README.md`

---

## Quick Reference
- 📋 [Checklists](ai/checklists/) — Review and quality gates
- 💬 [Prompt Templates](ai/prompts/) — Structure AI interactions
- ⚙️ [Operations Guides](ops/) — Alerts, monitoring, and runbooks
