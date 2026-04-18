```markdown
# p00006_quick_prototype

**Status:** Active
**SRS References:** Prototype focuses on UI-level, user-visible flows only (LMS, UAS, RCS, LSS features surfaced via fixtures)

## Goal

Rapidly deliver a minimal, hackable frontend prototype that demonstrates user flows (registration/login UI, listing browsing/search, listing detail, messaging UI, landlord management, and admin review) using a `Vite + Vue` app with local JSON fixtures. Backend persistence and runner execution are out of scope for this prototype slice.

## Constraints & Approach

- This PBI is explicitly a frontend prototype: prioritize speed and clear UI interactions over backend implementation.
- Build a `Vite + Vue` frontend prototype under `frontend/prototype/` that consumes JSON fixtures for users, listings, and messages.
- No backend services or test DB are required for this frontend-only prototype; interactions should be simulated in-browser using Vue state and fixtures.
- Keep UI minimal and localized in Traditional Chinese for stakeholder review.

## Implementation Plan

1. Scaffold a `Vite + Vue` app under `frontend/prototype/`.
2. Create Vue views/components for login, listings, listing detail, messages, landlord dashboard, and admin review.
3. Create JSON fixtures for users, listings, and messages under `frontend/prototype/public/fixtures/`.
4. Implement client-side Vue state and routing to load fixtures, simulate login/session, filter/search listings, and simulate messaging flows.
5. Add a README showing how to run `npm install`, `npm run dev`, and `npm run build`.
6. Document known limitations and technical debt (no backend, no persistence, no file uploads).

## Acceptance Criteria

- **AC-PROT-01:** The Vite app opens in a browser and loads JSON fixtures without backend dependencies.
- **AC-PROT-02:** The listings view supports search by keyword, city filter, and rent range with pagination simulated in the client.
- **AC-PROT-03:** The listing detail view shows full listing fields (title, description, rent, deposit, fees) using fixture data.
- **AC-PROT-04:** The messages view simulates sending a message from a tenant to a landlord; the message appears in the UI (in-memory only).
- **AC-PROT-05:** The frontend README includes instructions to run Vite and lists out-of-scope items/technical debt.

## User-visible Requirements (prototype scope)

- Users can register an account in the UI (simulated) with role selection (`tenant` or `landlord`) and a login identifier (email or username).
- Users can 'login' in the UI; the session is simulated client-side and persisted in localStorage for the prototype.
- Landlords can view, create (client-side only), edit, and delete listings within the UI; these actions update the in-memory state and fixtures for the session.
- Tenants can search listings by keyword (title/description) and by basic filters: city and rent range. Search supports client-side pagination.
- From a listing detail view, a tenant can compose a message to the landlord; messages display in the UI but are not persisted to a backend.
- Listings in fixtures may be marked `pending` or `published`; the UI shows `published` listings by default and includes a developer toggle to reveal `pending` items.
- All UI text is in Traditional Chinese.
- File upload, image processing, background jobs, REST API exposure, and backend persistence are out of scope for this frontend prototype and will be documented as technical debt.

- Landlord-specific UI: landlords can access a landlord dashboard to manage their listings (create, edit, delete) within the frontend prototype; create/edit flows update in-memory state for the session.
- Admin-specific UI: admins can access an admin review page that lists `pending` listings and can `publish` or `return` listings with a required return reason; these actions update in-memory state.

## Subtasks (frontend-focused)

- [x] Create PBI and mark as `Active` (this file)
- [x] Capture user-visible requirements (added `User-visible Requirements` section)
- [x] Frontend prototype: scaffold `Vite + Vue` app under `frontend/prototype/`
- [x] Frontend pages/components: create login, listings, listing detail, messages, landlord dashboard, and admin review screens
- [x] Frontend fixtures: add JSON fixtures under `frontend/prototype/public/fixtures/` for users, listings, and messages
- [x] Frontend interactions: add client-side Vue state/routing to simulate login, search/filters, pagination, and messaging (in-memory)
- [x] Frontend README: add `frontend/prototype/README.md` with instructions to run `npm install`, `npm run dev`, and `npm run build`
- [ ] Demo & feedback capture
- [ ] Frontend: landlord UI pages (`frontend/prototype/src/views/LandlordDashboard.vue`, `frontend/prototype/src/views/LandlordEditListing.vue`) to manage own listings (client-side)

Progress summary: 9/12 frontend tasks completed. Current focus: document technical debt, implement `LandlordEditListing.vue`, and capture demo feedback.

Notes: This PBI is intentionally frontend-only for fast stakeholder feedback; backend persistence work will be tracked in follow-up PBIs.

_Created 2026-04-18 to deliver a rapid frontend prototype per stakeholder request._
```
