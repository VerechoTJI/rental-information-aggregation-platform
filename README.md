# RIAP Super Repo

This repository is the top-level workspace for RIAP and manages separate backend and frontend repositories alongside shared documentation.

## Layout

- `backend/`: standalone backend repository with the Java service.
- `frontend/`: standalone frontend repository for the UI.
- `docs/`: source-of-truth requirements and documentation.
- `pbi/`: per-feature PBIs and backlog tracking.

## Quick setup (clone + submodules)

Clone and fetch submodules in one step:

```powershell
git clone --recurse-submodules https://github.com/VerechoTJI/rental-information-aggregation-platform.git
```

If you already cloned without submodules, run:

```powershell
git submodule sync --recursive
git submodule update --init --recursive
```

## Prerequisites

- Java 17 (JDK) installed and `java`/`javac` available on PATH.
- Apache Maven 3.8+ (`mvn` on PATH) to build the backend.
- (Frontend) Node.js and a package manager (npm or pnpm) when frontend code is added.

On Windows you can install with winget (example):

```powershell
winget install --id=Microsoft.OpenJDK.17 -e --source winget
winget install --id=Apache.Maven -e --source winget
```

## Backend build (quick)

From the repository root you can run:

```powershell
mvn -f backend test
# or to build the artifact
mvn -f backend package
```

If `mvn` is not available you'll see an error like "mvn: The term 'mvn' is not recognized" — install Maven and ensure it's on your PATH.

## Frontend

The `frontend/` submodule is currently a placeholder. When frontend sources are added the typical workflow will be:

```powershell
# from repo root
cd frontend
# install deps (example)
npm install
# start dev server
npm run dev
# build for production
npm run build
```

## Workflow

- Keep backend and frontend work in their own repositories.
- Use the root repo to coordinate shared docs, PBIs, and cross-repo planning.

## Conventions

Branch naming
- main: protected release branch.
- feature/<ticket-id>-short-desc: new features.
- fix/<ticket-id>-short-desc: bug fixes.
- hotfix/<short-desc>: urgent fixes to `main`.

Commit messages (Conventional Commits)
- Use Conventional Commits for all commits. Examples:
	- feat: add new search endpoint
	- fix: correct null pointer in listing parser
	- docs: update API section in README
	- chore: bump maven plugin versions

Submodules
- Clone with `--recurse-submodules` or run `git submodule update --init --recursive` after clone.
- Do not attempt to commit changes inside a submodule from the super-repo — cd into the submodule, commit there, then update the super-repo's recorded submodule commit and commit that change in the super-repo.

Pull requests
- Open PRs from feature branches into `main` and require at least one reviewer.
- Include a short description and reference the ticket id (if any).

Formatting and linters
- Follow project-specific linters where configured. For Java use a standard formatter (Google Java Style or similar).