# p00005_data_access_layer

**Status:** Pending
**SRS References:** `DBMS-F-01`, `DBMS-F-02`, `DBMS-F-03`, `DBMS-F-04`, `DBMS-N-01` to `DBMS-N-13`

## Goal

Provide a shared data access layer for CRUD, integrity constraints, transaction handling, and PostgreSQL persistence.

## Subtasks

- [ ] Define repository or DAO interfaces
- [ ] Implement PostgreSQL-backed persistence adapters
- [ ] Add transaction handling for multi-step operations
- [ ] Add integrity and validation rules
- [ ] Add tests for persistence and error handling

## Notes

- Keep all subsystems behind DBMS boundaries.
- Never allow direct table access from other subsystems.
