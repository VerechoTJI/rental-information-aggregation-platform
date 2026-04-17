# p00001_login

**Status:** Pending
**SRS References:** `RIAP-F-01`, `RIAP-F-02`, `UAS-N-01` to `UAS-N-15`

## Goal

Provide registration, login, logout, session handling, and role-based access control for tenants, landlords, and admins.

## Subtasks

- [ ] Define user and session domain model
- [ ] Implement registration and login flow
- [ ] Implement logout and session invalidation
- [ ] Enforce tenant, landlord, and admin authorization
- [ ] Add unit tests for happy-path and denial cases

## Notes

- Hash credentials before persistence.
- Keep API payloads JSON-based and transport secure over HTTPS.
