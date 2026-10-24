# Anna-Martina
Backend and AI engineering projects with measured results

# Hi, I'm Anna Martina 👋

Backend and AI engineering projects, built to practice production-style patterns, with measured results.

## Projects

### [E-commerce Distributed Platform](https://github.com/AnnaMartina31/ecommerce-platform)
Spring Boot microservices with Kafka, Redis, PostgreSQL, Prometheus/Grafana and Jaeger.
- CI on GitHub Actions for all services (Testcontainers integration tests)
- Transactional outbox, tested with Kafka down and up
- Timeouts + circuit breaker, k6 before/after: 240 uncontrolled failures → 0
- Idempotent consumer (a test caught a `merge`-instead-of-`insert` bug)
- Distributed tracing across 4 services
- JWT authentication validated at the gateway

### [Research Assistant (RAG)](https://github.com/AnnaMartina31/research-assistant)
Ask questions about PDFs and get answers with file and page citations.
- Retrieval evaluation (hit rate, MRR): hybrid search raised MRR from 0.683 to 0.835 on a 20-question set
- SSE streaming, pgvector + Postgres full-text, local LLM via Ollama

## Stack
Java 21, Spring Boot, Kafka, PostgreSQL, Redis, Docker, k6 · Python, FastAPI, pgvector, React + TypeScript
