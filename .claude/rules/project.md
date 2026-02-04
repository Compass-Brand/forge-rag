# Forge RAG Project Rules

## Project-Specific Guidelines

This project implements a custom RAG (Retrieval-Augmented Generation) system using the Ant Colony V2 architecture.

### Architecture Principles

- Follow the Ant Colony V2 distributed retrieval pattern
- Maintain separation between ingestion, storage, and retrieval layers
- Use swarm intelligence for query routing and result ranking

### Code Organization

- `api/` - FastAPI endpoints for ingestion, query, and management
- `core/` - Core RAG logic and algorithms
- `embeddings/` - Embedding generation and management
- `storage/` - PostgreSQL with pgvector and Memgraph integration
- `chunking/` - Document chunking strategies

### Testing Requirements

- All RAG operations must have integration tests
- Mock external embedding services in unit tests
- Test both BM25 and vector search paths
- Validate chunk boundary handling edge cases

### Performance Considerations

- Batch embedding requests where possible
- Use connection pooling for database operations
- Implement caching for frequently accessed embeddings
- Monitor and log query latency metrics

## Inherited Rules

This project inherits all rules from:
- `compass-brand/.claude/rules/` (coding style, security, testing, git workflow, performance, agents)
- `compass-forge/CLAUDE.md` (parent project guidelines)
