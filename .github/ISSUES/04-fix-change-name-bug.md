Title: Fix `change_name` logic bug in external reference / sample (optional)

Problem
- A comparison found a bug in the external sample `event-signup-python-mysql` where the `change_name` database update uses the wrong variable for `lastName`.

Proposal
- If we adapt code from the external sample, correct the update to use the correct variable and add a unit or manual test to prevent regressions.

Acceptance criteria
- Fix applied (if relevant) and a short test or validation added.

Labels: bug