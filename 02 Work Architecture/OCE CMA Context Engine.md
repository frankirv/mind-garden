---
tags: [project, active, architecture, oce, cma]
---

# OCE / CMA Context Engine

## Definitions
- **OCE**: generic context engine that handles flexible context retrieval and reasoning.
- **CMA**: application layer that calls OCE with prompts and expects structured JSON outputs.

## Current Challenge
Existing code mixes agents, context, and tools together. Interfaces are inconsistent. The team wants to move from Semantic Kernel to Microsoft Agent Framework.

## Target Direction
- Clean interfaces between agents, tools, context, and data sources.
- Other teams can register tools, agents, and data sources.
- Context ingestion should be separate from runtime context retrieval.
- The system should scale across multiple teams and use cases.

## Splitting Strategies to Spike
| Option | Description | Pros | Cons |
|---|---|---|---|
| A | Single prompt | Simple | May become too large |
| B | Split by repo at CMA | Practical | CMA owns routing |
| C | Split by category at CMA | More structured | Need category taxonomy |
| D | OCE decides split | More generic | Harder to implement |
| E | CMA passes split hints to OCE | Balanced | Needs clear contract |

## Documents Needed
- Broad team vision document
- Dev architecture document
- AI/Codex implementation guide
- Migration plan from Semantic Kernel to Microsoft Agent Framework
