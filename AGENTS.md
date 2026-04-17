# AGENTS.md

## Project Overview

- This workspace is for the **Rental Information Aggregation Platform (RIAP)**.
- The SRS defines five subsystems: `LMS` (Listing Management), `UAS` (User Authentication), `RCS` (Real-time Communication), `LSS` (Listing Search), and `DBMS` (Database Management).
- Treat `docs/SRS.pdf` as the source of truth for functional scope, interfaces, and requirement IDs.

## Core Constraints

- Use `PostgreSQL 16` for persistence.
- Prefer `Java 17+` for backend work if implementation files are added.
- Keep external traffic on `HTTPS`; use `WSS` or an equivalent secure channel for real-time messaging.
- Use `JSON` for API payloads and keep APIs `RESTful` unless the SRS explicitly requires otherwise.
- Never bypass `DBMS` for direct table access from other subsystems.

## Architecture Notes

- `UAS` owns authentication, sessions, roles, and access control.
- `LMS` owns listing creation, editing, moderation flow, and mandatory fee disclosure.
- `RCS` owns asynchronous tenant/landlord messaging and message history.
- `LSS` owns listing search, filtering, sorting, and search result formatting.
- `DBMS` owns CRUD, integrity constraints, transactions, connection management, and database access abstraction.

## Security Rules

- Hash passwords; never store plain-text credentials.
- Validate and sanitize all user input to prevent `SQL Injection` and `XSS`.
- Use least-privilege access for database connections and internal service calls.
- Preserve role-based access control for tenant, landlord, and admin actions.

## Implementation Conventions

- Keep changes small, modular, and aligned with the subsystem boundaries above.
- Prefer explicit interfaces or repositories/DAO layers for data access.
- Preserve requirement traceability when practical by referencing SRS requirement IDs in code, tests, commits, or PR notes.
- For UI work, keep layouts responsive and compatible with common desktop and mobile browsers.

## Testing Expectations

- Add or update tests for every behavioral change.
- Cover authentication, authorization, search filtering, message flow, and data persistence where relevant.
- Validate performance-sensitive search paths and any requirement that depends on timing or throughput.
- If a project build/test command exists, run it before finishing; otherwise, document the missing command path in the handoff.

## Working Habits

- Read the relevant SRS section before changing related code.
- Do not invent new product requirements without checking the SRS first.
- Update documentation when public behavior, APIs, or deployment steps change.
- Prefer existing workspace conventions over introducing new frameworks or folder structures.
- Follow the incremental workflow in `.github/skills/incremental-solver/SKILL.md`: work on one PBI at a time, move it to `pbi/active/`, review it together, update the PBI with new knowledge, plan small tasks, commit after each completed task, run TDD at the end, then do a final review and move it to `pbi/done/`.
- Track each feature as its own PBI file under `pbi/` using names like `p00001_login.md`.
- Keep pending PBIs at the top level of `pbi/`, move active work to `pbi/active/`, and move finished PBIs to `pbi/done/`.
- Track subtasks inside the relevant PBI file with a checklist.
- Keep executable Java work inside `backend/` unless a different structure is explicitly requested.

## Conventions

- Branch naming
	- `main`: protected release branch.
	- `feature/<ticket-id>-short-desc`: new features.
	- `fix/<ticket-id>-short-desc`: bug fixes.
	- `hotfix/<short-desc>`: urgent fixes to `main`.

- Commit messages (Conventional Commits)
	- Use Conventional Commits. Examples:
		- `feat: add new search endpoint`
		- `fix: correct null pointer in listing parser`
		- `docs: update API section in README`

- Submodules
	- Clone with `--recurse-submodules` or run `git submodule update --init --recursive` after clone.
	- When changing a submodule's files: cd into the submodule, commit and push there, then update the super-repo's submodule pointer and commit in the super-repo.

## Build & Test

- Run `mvn test` from `backend/` to validate the backend Maven project.
- Run `mvn package` from `backend/` when you need a distributable JAR.

## Current Workspace State

- The repository now contains documentation plus a `pbi/` workspace and separate `backend/` and `frontend/` repositories.
- Keep `docs/` intact and keep executable Java work inside `backend/`.
