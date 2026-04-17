# RIAP Super Repo

This repository is the top-level workspace for RIAP and manages separate backend and frontend repositories alongside shared documentation.

## Layout

- `backend/`: standalone backend repository with the Java service.
- `frontend/`: standalone frontend repository for the UI.
- `docs/`: source-of-truth requirements and documentation.
- `pbi/`: per-feature PBIs and backlog tracking.

## Backend Build

From `backend/`:

```powershell
mvn test
```

To create a packaged JAR:

```powershell
mvn package
```

## Workflow

- Keep backend and frontend work in their own repositories.
- Use the root repo to coordinate shared docs, PBIs, and cross-repo planning.