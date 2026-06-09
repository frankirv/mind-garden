---
tags: [ai, codex, claude-code, workflow]
---

# Codex and Claude Code Workflow

## Use Cases
- Implement GitHub issues
- Refactor existing code
- Generate tests
- Create documentation
- Review PRs
- Enforce architecture constraints

## Recommended Flow
1. Write or refine GitHub issue.
2. Add acceptance criteria.
3. Add architecture constraints.
4. Ask Codex/Claude Code to implement.
5. Run tests and lint.
6. Review only high-risk logic and architecture boundaries.
7. Merge smaller PRs faster; leave non-blocking refactors for follow-up.

## Prompt Pattern
```text
Implement this GitHub issue.

Context:
- Repo:
- Architecture constraints:
- Existing related files:
- Acceptance criteria:

Rules:
- Keep changes minimal.
- Add or update tests.
- Do not introduce new framework dependencies without explaining why.
- Summarize changed files and risks.
```

## Review Checklist
- [ ] Does it satisfy the issue?
- [ ] Are tests added or updated?
- [ ] Is the architecture still clean?
- [ ] Is the change small enough to merge?
- [ ] Are follow-up refactors captured separately?
