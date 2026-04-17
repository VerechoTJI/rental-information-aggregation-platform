---
name: decision-tracking
description: Track implementation decisions for RIAP in a lightweight, traceable format. Use when a design choice needs to be recorded, justified, and linked to SRS requirements or a PBI.
---

# Decision Tracking Skill

Use this skill when the team needs to record an implementation decision that is related to the RIAP SRS, but is not itself a new requirement.

## When To Use

- When choosing between implementation options such as ORM vs. DAO, sync vs. async, or schema strategies.
- When a design choice should be tracked in `docs/` for later reference.
- When the decision needs to stay aligned with an active PBI and SRS traceability.

## Decision Flow

1. **Identify the decision**
   - State the implementation choice clearly.
   - Separate the choice from the SRS requirements it supports.

2. **Confirm SRS alignment**
   - List the SRS requirement IDs that justify or constrain the decision.
   - Note whether the decision is required by the SRS or is a permitted implementation choice.

3. **Write the decision record**
   - Create a markdown file under `docs/decisions/`.
   - Keep the record short, traceable, and specific.

4. **Update the active PBI**
   - Add a short section that records the chosen approach.
   - Mark the corresponding planning task as complete.

5. **Verify the traceability**
   - Check that the decision record, PBI, and SRS references agree.
   - Keep any later implementation work within the selected boundary.

## Current Template

Use this template for a new decision record:

```markdown
# <decision-title>

**Status:** Accepted
**Date:** YYYY-MM-DD
**Scope:** `<pbi-id-or-feature>`

## Decision

State the implementation choice in one sentence.

## Rationale

- Explain why this option was chosen.
- Reference the SRS requirement IDs that support the choice.
- Mention any relevant tradeoffs or constraints.

## Notes

- Clarify whether this is a project decision or an SRS requirement.
- Record any follow-up constraints for implementation.
```

## Writing Rules

- Keep the decision record short and actionable.
- Use the SRS requirement IDs in the rationale whenever possible.
- Do not turn the decision file into a full design document.
- Keep the PBI and decision record synchronized when the choice changes.

## Example

Use `docs/decisions/dbms-persistence-approach.md` as the current example of this pattern.
