# ScientiaMesh import acceptance test

1. Create an empty Space called Acme Engineering.
2. Add this repository as a public GitHub connection. Include Markdown documentation and issues if selectable.
3. Wait for import and processing to finish.
4. Ask these questions and inspect their source citations:
   - How do I run this project locally? Expected: documentation server on port 8080, not a working taskboard.
   - Why did we choose SQLite? Expected: single-instance pilot and operational simplicity; cite ADR-001.
   - What must be decided before the pilot? Expected: authentication and timezone policy, plus backup/restore work.
   - Does the MVP include billing? Expected: no.
5. Change the documentation server port in README from 8080 to 8090 in both the command and URL, commit it, then sync. Ask the run question again and verify the updated source is used.
6. Invite a second Space member without GitHub authorization; verify they can read the imported content.
7. Create a separate Space and verify it does not automatically receive this content. Keep descendant sharing off unless explicitly testing it.

This public fixture does not test private GitHub App authorization or revocation.
