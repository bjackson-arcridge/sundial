---
id: DR-0031
title: Configure the memory store separately from the runtime folder
status: accepted
domain: cli
created: 2026-07-09
references:
  - packages/cli/src/core/store.ts
  - packages/cli/src/main.ts
  - packages/cli/README.md
updated: 2026-10-14
author: bjackson
---
## Decision

Keep sundial/config.json at the project root as the discovery anchor. Resolve project memory under its project-relative store setting, defaulting to sundial. The folder setting independently chooses the target for managed agent assets. Configuration changes do not migrate existing files.

## Appendix

User correction on 2026-10-14: the store field was intended to select the memory root. This replaces the previous fixed-store restriction while retaining the independent runtime-folder setting.
