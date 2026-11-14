# Roadmap: FDE Portfolio Implementation (ROADMAP.md)

## Milestone 1: Enterprise Data Pipeline & Ontology Graph Engine
- [ ] Task 1.1: Project scaffolding with `uv` / `poetry` & Docker Compose (PostgreSQL + PgAdmin)
- [ ] Task 1.2: Raw data ingestion service (CSV/JSON/REST) with DuckDB & Polars
- [ ] Task 1.3: Data modeling & Palantir-style Ontology layer (Entities, Relationships, Action hooks)
- [ ] Task 1.4: FastAPI REST interface with Pydantic validation & documentation
- [ ] Task 1.5: Automated pytest suite, GitHub Actions CI workflow, and architecture README

## Milestone 2: Production-Ready Enterprise RAG & Semantic Search
- [ ] Task 2.1: Document processing & chunking pipeline with metadata extraction
- [ ] Task 2.2: pgvector / Qdrant vector store integration with hybrid search (dense + BM25)
- [ ] Task 2.3: Re-ranking with cross-encoders & RBAC filtering
- [ ] Task 2.4: Evaluation framework with Ragas / TruLens (Context Recall, Faithfulness)
- [ ] Task 2.5: Containerization & GitHub publication

## Milestone 3: High-Throughput Client Webhook & Observability Gateway
- [ ] Task 3.1: Async webhook ingestion endpoint with idempotency checks
- [ ] Task 3.2: Redis background worker with exponential backoff & dead-letter queue
- [ ] Task 3.3: OpenTelemetry instrumentation, Prometheus metrics, and Grafana dashboard
- [ ] Task 3.4: Load testing with Locust and resilience validation

## Milestone 4: Full-Stack FDE Operations Dashboard & K8s Deployment
- [ ] Task 4.1: Next.js (TypeScript) dashboard for data pipelines & pipeline health
- [ ] Task 4.2: End-to-end integration with backend APIs
- [ ] Task 4.3: Helm chart authoring & local Kubernetes (Minikube/Kind) validation
- [ ] Task 4.4: Final documentation, live demo recording, and resume alignment
