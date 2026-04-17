# p00004_real_time_messaging

**Status:** Pending
**SRS References:** `RIAP-F-08`, `RIAP-F-09`, `RCS-N-01` to `RCS-N-14`

## Goal

Support asynchronous tenant-landlord messaging with persisted message history.

## Subtasks

- [ ] Define conversation and message domain model
- [ ] Implement message send and receive flow
- [ ] Persist conversation history
- [ ] Enforce access control for participants
- [ ] Add tests for history retrieval and unauthorized access

## Notes

- Use a secure real-time transport such as `WSS`.
- Keep message history available for later review.
