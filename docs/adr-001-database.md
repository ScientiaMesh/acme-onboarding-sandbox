# ADR-001: SQLite for the prototype

Date: 2026-11-09
Status: accepted for the fictional prototype
Decision owner: Taylor (fictional)

## Context
The first pilot will run on one application instance with a small internal team. Operational simplicity matters more than distributed writes.

## Decision
Use SQLite for the prototype. PostgreSQL is not required for the documentation exercise.

## Consequences
Keep database access behind a repository layer. Revisit this decision before multiple application instances or sustained concurrent writes are required. Backup and restore procedures must be documented before the pilot holds important data.

## Alternative
PostgreSQL offers stronger multi-instance flexibility but introduces a separate service to operate. It is a migration option, not the current prototype choice.
