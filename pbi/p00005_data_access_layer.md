# p00005_data_access_layer

**Status:** Active
**SRS References:** `DBMS-F-01`, `DBMS-F-02`, `DBMS-F-03`, `DBMS-F-04`, `DBMS-N-01` to `DBMS-N-13`

## Goal

Provide a shared data access layer for CRUD, integrity constraints, transaction handling, and PostgreSQL persistence.

## Implementation Plan

- Map the DBMS requirements to concrete persistence responsibilities.
- Define the first set of domain contracts and repository boundaries.
- Choose the persistence approach and transaction model for the backend.
- Scaffold the DBMS-facing interfaces and shared infrastructure.
- Implement one repository end-to-end with tests before expanding further.

## Design Breakdown

- `DBMS-F-01` and `DBMS-F-02` require a persistence layer that can store and retrieve shared entities for users, listings, messages, and logs.
- `DBMS-F-03` requires integrity rules to live close to the persistence boundary so foreign keys and checks are enforced consistently.
- `DBMS-F-04` is a later concern and should stay out of the first slice unless a backup abstraction is needed.
- `DBMS-N-02` means the first contract should look like a DAO or repository boundary, not direct table access.
- `DBMS-N-03` and `DBMS-N-08` require transaction-aware operations for multi-step writes and ACID-safe behavior.
- `DBMS-N-04` and `DBMS-N-07` imply the persistence layer should assume a controlled internal application-server connection, not public database access.
- `DBMS-N-05`, `DBMS-N-06`, and `DBMS-N-10` are performance-oriented concerns that should influence schema and query design after the core contract exists.
- `DBMS-N-11` means deletion behavior must be designed explicitly for parent-child relationships.
- `DBMS-N-12` and `DBMS-N-13` confirm PostgreSQL as the target database and allow a JPA or DAO-based approach.

## First Domain Slice

- Start with `UserAccount` as the first shared domain model because it is foundational to authentication, role checks, and ownership references across the platform.
- Define `UserAccountRepository` as the first boundary so the DBMS layer exposes only CRUD-style operations for account persistence.
- Keep session handling, listing persistence, messaging history, and backup concerns out of this first slice.
- Model fields should be limited to the account identity, role, credential hash, and account status needed by UAS and downstream ownership checks.
- Prefer repository methods that support lookup by ID and by login identifier, plus create/update/delete operations.

## Persistence Decision

- Use `JPA` with `Hibernate` for the DBMS layer.
- Track the implementation choice in `docs/decisions/dbms-persistence-approach.md`.
- Keep the repository API narrow so the ORM remains behind the DBMS boundary.

## Current Implementation Slice

- Added the initial JPA and Hibernate dependencies to `backend/pom.xml`.
- Introduced the first shared DBMS model with `UserAccount`, `UserAccountRole`, and `UserAccountStatus`.
- Added `UserAccountRepository` as the first repository boundary.
- Added a JPA entity and mapper scaffold for the user-account flow.
- Verified the backend with `mvn test` after the scaffold was added.
- Scaffolded a small DBMS infrastructure helper `JPAEntityManagerFactoryProvider` to centralize `EntityManagerFactory` creation and closing.

## Acceptance Criteria

- **AC-DBMS-01:** The persistence approach decision is documented in `docs/decisions/dbms-persistence-approach.md` and referenced from the PBI.
- **AC-DBMS-02:** The backend builds and tests successfully with `mvn test` (unit + integration using H2 in-memory `test-pu`).
- **AC-DBMS-03:** `UserAccountRepository` interface exists and a JPA-backed adapter (`UserAccountJpaAdapter`) implements CRUD: save, findById, findByLoginIdentifier, deleteById.
- **AC-DBMS-04:** A `persistence.xml` test persistence unit (`test-pu`) is present under `src/test/resources/META-INF` and is used by integration tests.
- **AC-DBMS-05:** JPQL usage in adapters is documented in `docs/decisions/jpql-explainer.md` and the PBI notes.
- **AC-DBMS-06:** No other subsystem accesses database tables directly; all access is through repository/DAO boundaries.
- **AC-DBMS-07:** The first persistence flow (UserAccount) has automated tests covering domain validation and mapping (unit) and persistence CRUD (integration).
- Scaffolded a small DBMS infrastructure helper `JPAEntityManagerFactoryProvider` to centralize `EntityManagerFactory` creation and closing.

## Subtasks

- [x] Break DBMS requirements into implementable persistence responsibilities
- [x] Define the first domain model and repository interfaces
- [x] Confirm PostgreSQL/JPA or DAO approach for the backend
- [x] Scaffold shared DBMS infrastructure and error handling
- [x] Implement one persistence flow with unit tests
- [ ] Add transaction and integrity rules for multi-step writes
- [ ] Extend the layer to cover additional subsystems
- [x] Add integration-style tests for persistence behavior

## Notes

- Keep all subsystems behind DBMS boundaries.
- Never allow direct table access from other subsystems.
- Start with a design pass before introducing database-specific code.
- Prefer the smallest vertical slice that can be verified independently.
- JPQL usage and alternatives documented in `docs/decisions/jpql-explainer.md`.
