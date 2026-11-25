# Builder Runner

This is a dedicated CI runner repository for building Android artifacts securely via GitHub Actions.

- Builds are triggered manually via **Actions -> Run workflow** (`workflow_dispatch`).
- Source code is pulled from the private repository at build time.
- Compilation logs are concealed to prevent private code leakage in public CI logs.
- Generated artifacts are published directly to private repository releases; no public artifacts are stored here.
