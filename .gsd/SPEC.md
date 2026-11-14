# Specification: Forward Deployed Engineer (FDE) Portfolio

> Status: Locked — Phase 1 Ready

## 1. Executive Summary
- **Track Goal:** Comprehensive Forward Deployed Engineer (FDE) technical mastery and building 4 production-grade projects for GitHub.
- **Role Focus:** Applied AI, Data Engineering, Backend Microservices, Containerization & Client Deployment.

## 2. Core Technical Competencies
- **Core Languages:** Python (AsyncIO, Pydantic, Typing), TypeScript / Go.
- **Data Engineering:** SQL (Advanced Window Functions, CTEs), PostgreSQL, DuckDB, Polars, dbt.
- **DevOps & Infra:** Docker multi-stage builds, Docker Compose, Kubernetes, Helm, GitHub Actions.
- **AI & Retrieval:** Hybrid RAG (pgvector/Qdrant + BM25), Cross-encoders, Tool-calling agents, Ragas evaluation.
- **Enterprise Integrations:** OAuth2/OIDC, Webhooks, Idempotency, Rate-limiting, OpenTelemetry.

## 3. GitHub Project Deliverables
1. **`enterprise-data-ontology-engine`**: Messy data ingestion, normalization, and relational/graph ontology mapper.
2. **`secure-enterprise-rag`**: RAG system with document chunking, hybrid search, RBAC permissions, and evaluation metrics.
3. **`client-webhook-gateway`**: Resilient ingestion microservice with Redis queue, dead-letter logic, and Prometheus/Grafana metrics.
4. **`fde-ops-dashboard`**: Full-stack Next.js + FastAPI monitoring dashboard deployable via Kubernetes / Helm.
