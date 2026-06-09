---
tags: [architecture, migration, agent-framework]
---

# Microsoft Agent Framework Migration

## Why Migrate
- Need scalable agent architecture.
- Need cleaner interfaces.
- Need easier tool/data-source registration by multiple teams.
- Current Semantic Kernel codebase mixes responsibilities.

## Recommended Approach
Start a clean codebase when the current one is too entangled, then copy over valuable components selectively.

## Migration Principles
- Preserve business logic where useful.
- Do not copy unclear abstractions.
- Define interfaces first.
- Create tests around critical behavior.
- Use AI coding tools for implementation, but keep architecture constraints explicit.

## Team Concerns
Possible objections:
- Existing owners may prefer incremental changes.
- Team may distrust AI-generated code.
- People may want line-by-line review.

Response:
- Use architecture docs, tests, small PRs, and clear acceptance criteria.
- Merge useful changes sooner; refactor iteratively.
