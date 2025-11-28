Title: Improve frontend UX — success messages and activity limits

Problem
- Frontend works but could show clearer confirmations and enforce activity capacity server-side.

Proposal
- Add clearer success/error messages, disable signup when an activity is full, and return `spots_left` from server API. Ensure server enforces `max_participants`.

Acceptance criteria
- Frontend shows clear success/error messages for signup/unregister.
- Server returns spots-left and enforces `max_participants`.

Labels: enhancement
