Title: Fix security issues — hash passwords & use parameterized queries

Problem
- Storing plaintext passwords and building SQL via string interpolation is insecure and vulnerable to SQL injection.

Proposal
- Add password hashing (Werkzeug or bcrypt) and update the database layer to use parameterized queries or an ORM (SQLAlchemy). Audit existing DB calls and replace unsafe patterns.

Acceptance criteria
- Passwords are stored hashed; login verifies with hash checks.
- No raw string interpolation in SQL statements; queries use parameters.
- README updated with security notes and migration steps if needed.

Labels: security
