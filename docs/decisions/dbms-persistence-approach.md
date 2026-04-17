# DBMS Persistence Approach Decision

**Status:** Accepted
**Date:** 2026-04-17
**Scope:** `p00005_data_access_layer`

## Decision

Use `JPA` with `Hibernate` as the persistence approach for the DBMS layer.

## Rationale

- `DBMS-N-13` explicitly recommends `Hibernate` or `JPA` for object-relational mapping.
- The first DBMS slice is expected to support standard CRUD flows, which fit a repository-based ORM approach well.
- `JPA` and `Hibernate` reduce boilerplate for the shared data access layer while keeping the implementation compatible with PostgreSQL.

## Notes

- This is a project implementation decision, not a change to the SRS requirements.
- The SRS already allows this direction through `DBMS-N-13`.
- Future DBMS work should keep the repository boundary in place and avoid direct table access from other subsystems.