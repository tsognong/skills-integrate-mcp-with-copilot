Title: Add persistent storage (SQLite) and migrations

Problem
- The app currently uses an in-memory activities store; data is lost on restart.

Proposal
- Add SQLite-based persistence (using SQLAlchemy or the standard `sqlite3`), add lightweight migration or bootstrap scripts, and include an updated `requirements.txt` for local development. Keep the current JSON API and frontend unchanged where possible.

Acceptance criteria
- Activities and participant sign-ups persist across restarts.
- Provide a migration / bootstrap step and update the README with setup instructions.
- Add a minimal smoke test or manual verification steps to confirm persistence.

Labels: enhancement