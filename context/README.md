# Product team agent profiles

This pack contains specialist role instructions for a multidisciplinary product-agent team.

## Included profiles

- `PRODUCT_MANAGER.md`
- `USER_RESEARCHER.md`
- `ENGINEER.md`
- `CONTENT_DESIGNER.md`
- `DATA_ANALYST.md`
- `ACCESSIBILITY_SPECIALIST.md`
- `DESIGN_SYSTEM_SPECIALIST.md`

Add your existing designer profile alongside these files.

## Suggested repository location

```text
agents/
├── DESIGNER.md
├── PRODUCT_MANAGER.md
├── USER_RESEARCHER.md
├── ENGINEER.md
├── CONTENT_DESIGNER.md
├── DATA_ANALYST.md
├── ACCESSIBILITY_SPECIALIST.md
└── DESIGN_SYSTEM_SPECIALIST.md
```

Your root `AGENTS.md` should tell the lead agent when to use these profiles. Role files are supporting context and are not automatically loaded merely because they exist in the repository.

## Suggested orchestration instruction

```markdown
## Specialist agents

For substantial product problems, delegate independent questions to the relevant specialists in `agents/`.

- Give each specialist a bounded task.
- Ask each specialist to read its role file and the current brief.
- Use only roles that materially improve the work.
- Keep evidence separate from assumptions.
- Wait for relevant specialists before deciding.
- Reconcile disagreements and return one coherent recommendation.
- The lead agent owns the final synthesis.
```
