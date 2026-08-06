# Server Repository Instructions

## Scope

This is a provisional repository. Its name does not finalize ownership or require
the final system to have a separate server repository.

## Current phase

Before implementation, read the workspace `docs/project-background.md`. Do not
choose a language, framework, database, protocol, authentication model, feature
set, or repository boundary without an explicit decision. Do not copy the legacy
reference implementation by default.

## Working rules

- Keep server implementation and server-owned contracts in this repository.
- Keep generated output, credentials, local data, and dependency directories out
  of Git.
- Document build, test, migration, and development commands when tooling is added.
- Add tests in proportion to behavior and compatibility risk.
- Preserve unrelated user changes and avoid destructive Git operations.
- Use explicit failures rather than mock success paths or silent fallbacks.

Before finalizing a change, run the repository's documented checks and inspect the
diff for secrets, generated artifacts, and unintended contract changes.
