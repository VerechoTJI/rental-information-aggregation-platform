# PBI Workspace

Use this folder to track work one feature at a time.

## Layout

- `pbi/*.md`: pending PBIs that have not started or been finished yet.
- `pbi/active/*.md`: PBIs currently in progress.
- `pbi/done/*.md`: PBIs that are complete.
- `backend/`: backend repository for executable Java work.
- `frontend/`: frontend repository for UI work.

## Workflow

- Create a PBI file for each feature.
- Track subtasks inside that file with a checklist.
- Move the file to `pbi/active/` when work starts.
- Move the file to `pbi/done/` when work finishes.
- Any PBI not in `active` or `done` is considered pending.

## Naming

- Use filenames like `p00001_login.md` with a five-digit numeric prefix and a concise lowercase name.
- Keep the same file in `pbi/`, `pbi/active/`, or `pbi/done/` depending on status.
