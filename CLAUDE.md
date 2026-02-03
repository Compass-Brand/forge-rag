# CLAUDE.md

This file provides guidance to Claude Code when working in this repository.

## Project: Forge RAG

**Description:** Custom RAG system using Ant Colony V2 architecture for intelligent retrieval.

**Project Type:** development

---

## Tech Stack

| Layer          | Technology            |
| -------------- | --------------------- |
| Language       | Python 3.11+          |
| Embeddings     | OpenAI / Local models |
| Graph Database | Memgraph              |
| Framework      | FastAPI               |

---

## Development Methodology: TDD

All functional code MUST follow Test-Driven Development.

```
RED -> GREEN -> REFACTOR
```

---

## Git Discipline (MANDATORY)

**Commit early, commit often.**

- Commit after completing any file creation or modification
- Maximum 15-20 minutes between commits
- Use conventional commit format: `type: description`

Types: `feat`, `fix`, `refactor`, `docs`, `chore`, `test`
