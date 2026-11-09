# Acme Taskboard — onboarding sandbox

A fictional engineering project for testing ScientiaMesh GitHub imports, source-grounded answers, and synchronization. All people, requirements, and incidents are synthetic. This is a documentation fixture, not a production application.

## Product
A small task board for an internal engineering team. The planned MVP supports projects, tasks, assignees, and due dates. It does not include billing or public signup.

## Run the documentation locally
Requires Python 3.10 or newer; no packages or credentials required.

```sh
git clone https://github.com/ScientiaMesh/acme-onboarding-sandbox.git
cd acme-onboarding-sandbox
python3 -m http.server 8080 --bind 127.0.0.1
```

Open http://127.0.0.1:8080. This serves the files for inspection; it is not a running taskboard app and does not render Markdown.

## Start here
- [Onboarding](docs/onboarding.md)
- [Architecture](docs/architecture.md)
- [Decision: SQLite for the prototype](docs/adr-001-database.md)
- [Roadmap](docs/roadmap.md)
- [Import test checklist](docs/import-test.md)

GitHub issues track deliberately unresolved sample work. Nothing here contains customer data or private ScientiaMesh documentation.
