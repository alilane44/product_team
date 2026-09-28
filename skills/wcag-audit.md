# Skill: WCAG audit

A repeatable accessibility review procedure. Any role may invoke it. Produces a
consistent, actionable output. This is a review aid, not a compliance
certificate — see the compliance caveat in `../context/HOUSE_STYLE.md`.

## When to use

- Reviewing a flow, screen or component for accessibility barriers.
- Before recommending an interaction pattern as complete.

## Procedure

Check each area and record pass / fail / needs-testing with the user impact.

1. **Keyboard** — every action reachable and operable; no traps; logical order.
2. **Focus** — visible indicator; focus managed on route/dialog/state changes.
3. **Name, role, value** — controls expose correct semantics programmatically.
4. **Structure** — headings, landmarks and reading order are meaningful.
5. **Announcements** — dynamic updates announced when needed, without noise.
6. **Contrast** — text and essential UI meet contrast expectations.
7. **Colour independence** — meaning never conveyed by colour/shape/position alone.
8. **Zoom and reflow** — usable at 200–400% and at narrow widths, no loss of content.
9. **Motion and timing** — no essential info in motion; time limits adjustable.
10. **Errors** — identifiable, described in text, and recoverable.

## Output format

| Area | Result | User impact | Recommendation |
|------|--------|-------------|----------------|
| Keyboard | Fail | Cannot submit without a mouse | Add keyboard handler + focus order |

Follow with:
- **Highest-risk barriers** (blockers to core tasks first).
- **Manual + assistive-tech tests required** (what a review cannot confirm).
