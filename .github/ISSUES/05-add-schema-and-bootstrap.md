Title: Add database schema & sample data + bootstrap script

Problem
- There are no local DB bootstrap scripts or sample data to speed development and testing.

Proposal
- Provide a `schema.sql` or lightweight migration, and a sample data loader or script that inserts example activities and participants for local development.

Acceptance criteria
- `schema.sql` or migrations included and documented.
- A `scripts/bootstrap_db.sh` or Python script provided to load sample data.

Labels: enhancement