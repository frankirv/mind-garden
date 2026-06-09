---
tags: [github, workflow, ai-development]
---

# GitHub Issue Based Development

## Goal
Use GitHub issues as the actionable task layer below higher-level planning tools.

## Issue Template
```markdown
## Goal

## Background

## Acceptance Criteria
- [ ]

## Architecture Constraints
- 

## Files likely involved
- 

## AI Prompt
Implement this issue following the acceptance criteria and architecture constraints.
Keep changes minimal, add tests, and summarize risks.
```

## Best Practices
- One issue should be small enough for one PR.
- Add clear acceptance criteria.
- Include non-goals.
- Use labels like `ai-ready`, `needs-design`, `refactor`, `test`.
- Capture follow-up cleanup as separate issues.
