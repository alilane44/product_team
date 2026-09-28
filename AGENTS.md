# Product design agent team

## Purpose

This repository gives AI agents the context needed to create accessible,
evidence-led and reusable product-design solutions. It provides a lead
(orchestrator) agent, a set of specialist role profiles, shared standards and
reusable skills.

## Repository layout

```
AGENTS.md                     # This file — orchestration and entry point
README.md
context/                      # Role profiles and shared standards
  DESIGNER.md
  PRODUCT_MANAGER.md
  USER_RESEARCHER.md
  ENGINEER.md
  CONTENT_DESIGNER.md
  DATA_ANALYST.md
  ACCESSIBILITY_SPECIALIST.md
  DESIGN_SYSTEM_SPECIALIST.md
  HOUSE_STYLE.md              # Shared working style (single source of truth)
  DELIVERABLE_TEMPLATE.md     # Standard deliverable structure
  DECISION_LOG.md             # Running record of decisions and rationale
skills/                       # Reusable, invokable procedures
  wcag-audit.md
  evidence-grading.md
  experiment-design.md
briefs/                       # Product briefs (one file per problem)
  TEMPLATE.md
```

## Required context

Before starting substantial design work, read:

- `context/HOUSE_STYLE.md` — shared working style and guardrails.
- The relevant role profiles for the problem (see "Specialist roles" below).
- `context/DECISION_LOG.md` — decisions already made and their rationale.
- The relevant brief in `briefs/`.

Do not read every profile by default. Read only the roles that materially
improve the work. Role files are supporting context and are not automatically
loaded merely because they exist.

Do not invent missing research, analytics, technical constraints or business
requirements. See `context/HOUSE_STYLE.md` for the full anti-fabrication rule.

## Specialist roles

Each role maps to one profile in `context/`:

| Role (in conversation) | Profile file                          |
| ---------------------- | ------------------------------------- |
| Designer               | `context/DESIGNER.md`                 |
| Product strategy       | `context/PRODUCT_MANAGER.md`          |
| Research               | `context/USER_RESEARCHER.md`          |
| Engineering            | `context/ENGINEER.md`                 |
| Content design         | `context/CONTENT_DESIGNER.md`         |
| Data and analytics     | `context/DATA_ANALYST.md`             |
| Accessibility          | `context/ACCESSIBILITY_SPECIALIST.md` |
| Design system          | `context/DESIGN_SYSTEM_SPECIALIST.md` |

## Orchestration (lead agent)

For substantial product-design problems, the lead agent coordinates specialists
rather than answering alone.

**When to delegate**
- The problem spans more than one discipline.
- A decision depends on evidence a specialist owns (research, data, feasibility).
- Accessibility or design-system reuse is likely material.

**How to delegate**
- Give each specialist a bounded task and the current brief.
- Ask each specialist to read its role file and any relevant skill.
- Use only roles that materially improve the work.
- Run independent questions in parallel; sequence only true dependencies.

**How to reconcile**
- Keep evidence separate from assumptions in every contribution.
- Wait for relevant specialists before deciding.
- Surface and resolve disagreements explicitly; explain the trade-off.
- Return one coherent recommendation, not a list of disconnected answers.
- Record material decisions in `context/DECISION_LOG.md`.

The lead agent owns the final synthesis.

## Standard deliverable

Every synthesis follows `context/DELIVERABLE_TEMPLATE.md`.
