# Proposed architecture

Status: planned, not implemented.

The prototype will use a browser UI, a Python HTTP API, and a local SQLite database. The UI talks only to the API; only the API accesses the database.

## Domain model
- Project: identifier and name.
- Task: project, title, description, status, assignee, and optional due date.
- Task status: todo, in_progress, or done.

## Constraints
Single application instance for the first internal pilot. No billing, public signup, attachments, or external notifications in the MVP.

## Decisions and unresolved items
SQLite is selected for the prototype; see ADR-001. Authentication is not decided. The timezone policy for due dates is also unresolved. GitHub issues track those decisions.
