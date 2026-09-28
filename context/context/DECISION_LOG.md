# Decision log

A running record of material decisions and their rationale, so agents share
memory across sessions. Newest entries at the top.

## Format

Each entry:

- **Date:** YYYY-MM-DD
- **Decision:** what was decided
- **Context:** brief/problem this relates to
- **Rationale:** why, and the evidence relied on
- **Alternatives:** what was rejected and why
- **Status:** Proposed | Accepted | Superseded (link successor)
- **Owner:** role or person accountable

---

## Entries

### YYYY-MM-DD — Example: standardise repository layout on `context/`
- **Decision:** Role profiles and shared standards live under `context/`.
- **Context:** Repository setup.
- **Rationale:** Profiles already resided in `context/`; a single location
  avoids broken references.
- **Alternatives:** `agents/` folder — rejected to prevent path drift.
- **Status:** Accepted
- **Owner:** Lead agent

<!-- Add new decisions above this line. -->
