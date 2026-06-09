---
tags: [project, active, vocabulary, ai-app]
---

# Mind Hub App

## Vision
A personal AI dashboard with focused apps for reading, vocabulary, document analysis, and learning.

## Current Requirements
- Dashboard with multiple AI support apps.
- Reading interface with vocabulary extraction and highlighting.
- Each document page should have a separate URI.
- Large files should support pagination.
- Home page should not show full document content.
- Side section for vocabulary.
- Do not show known vocabulary.
- Filter simple variants like `idea` / `ideas`.
- Filter 1–2 character tokens.
- Compare by lemma, so `known` can match `know`.

## Data Direction
- Move from Cosmos DB local emulator to PostgreSQL with vector features.
- Store documents, parsed text, vocabulary, stats, and user-known words.
- Consider local or CLI LLM for definitions/examples to reduce API cost.

## Useful Metrics
- Number of new vocabulary words
- Text complexity
- Known vs unknown vocabulary ratio
- Reading progress
- Review frequency

## Next Actions
- [ ] Define database schema
- [ ] Create document loader
- [ ] Build reading page
- [ ] Add vocabulary extraction
- [ ] Add known-word filtering
- [ ] Add text stats
