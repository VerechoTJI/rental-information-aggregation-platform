---
name: pbi-construction
description: Create and update RIAP product backlog items in the `pbi/` workflow. Use when asked to construct a new PBI, update PBI status, or organize subtasks for a feature.
---

# PBI Construction Skill

Use this skill to create or update product backlog items (PBIs) for the RIAP workspace.

## When To Use

- When a user asks to create a new feature PBI.
- When a user asks to update PBI status, subtasks, or naming.
- When a user wants backlog work organized for the `pbi/` workflow.

## Copilot Discovery Convention

- This skill is auto-discovered by GitHub Copilot because it lives under `.github/skills/<skill-name>/SKILL.md`.
- The skill directory name and the `name` frontmatter field should stay lowercase and hyphenated.
- Keep any supporting scripts or notes inside the same skill directory if needed later.

## PBI Structure

- Create one file per feature.
- Use the filename pattern `p00001_short_name.md`.
- Keep the file title aligned with the filename and feature name.
- Put the PBI at the top level of `pbi/` when it is pending.
- Move it to `pbi/active/` when work starts.
- Move it to `pbi/done/` when work is finished.

## Required Sections

- `Status`: one of `Pending`, `Active`, or `Done`.
- `SRS References`: list the relevant requirement IDs from `docs/SRS.pdf`.
- `Goal`: describe the feature outcome in one short paragraph.
- `Subtasks`: track implementation work with a checklist.
- `Notes`: capture constraints, dependencies, or traceability reminders.

## Writing Rules

- Keep each subtask actionable and small enough to complete independently.
- Prefer clear feature names like `login`, `listing_management`, or `search_and_filtering`.
- Reference SRS requirement IDs whenever possible.
- Keep the wording concise and implementation-focused.
- Do not invent requirements that are not in the SRS.

## Example Template

```markdown
# p00001_login

**Status:** Pending
**SRS References:** `RIAP-F-01`, `RIAP-F-02`

## Goal

Describe the feature briefly.

## Subtasks

- [ ] Subtask one
- [ ] Subtask two

## Notes

- Any constraints or traceability reminders.
```

## Output Expectation

When asked to construct a PBI, produce a ready-to-use markdown file that matches this structure and naming convention.
