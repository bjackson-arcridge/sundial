---
id: DR-0033
title: Shared Sundial guidance lives in the canonical store file
status: accepted
domain: cli
created: 2026-07-19
references:
  - packages/cli/src/core/store.ts
  - packages/cli/src/core/harnesses.ts
  - packages/cli/src/core/templates/skills
updated: 2026-10-14
author: bjackson
---
## Decision

Install and refresh shared agent workflow guidance at SUNDIAL-INSTRUCTIONS.md in the configured store; decision-aware skills reference that file instead of embedding Sundial-managed blocks in AGENTS.md or CLAUDE.md.
