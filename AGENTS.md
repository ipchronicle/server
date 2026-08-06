# Server Repository Instructions

## Scope

This repository owns server-side IPChronicle product code and server-owned
contracts. Cross-repository decisions belong in the workspace architecture docs.

## Current phase

This is a scaffold. Do not choose a language, framework, database, protocol,
authentication model, or feature set without an explicit architecture decision.
Do not copy the legacy reference implementation by default.

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
