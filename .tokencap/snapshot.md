<!-- TokenCap v1.6 Savings: baseline 14,282 tok → actual 7,883 tok (44.8% saved) -->
# AI ENTRY POINT

This repository has been indexed by TokenCap.

Before analyzing files, read:

.tokencap/agent/START_HERE.md

Use:

- .tokencap/agent/agent-pack.md
- .tokencap/agent/allowed-context.json
- .tokencap/agent/context-manifest.json

Do not rediscover the repository from scratch.

---

# TokenCap Snapshot

| Field | Value |
| --- | --- |
| Generated | 2026-11-13T12:29:35.306Z |
| Workspace | /Users/jayakrishna/Desktop/rev_eng |
| Profile | balanced |
| Selected files | 10 |
| Source bytes | 57378 |
| Estimated source tokens | 14282 |

## Read First

This file is a compressed coding-session handoff. Read it before editing, then inspect the referenced files directly. Prefer the live repository over this snapshot when there is a conflict.

## TokenCap Intelligence Files

- TOKENCAP_GRAPH.md — Project dependency and architecture graph *(JS/TS projects only)*
- TOKENCAP_MEMORY.md — Developer notes, current task, constraints, and context memory

## Handoff Summary

| Field | Value |
| --- | --- |
| Read order | README.md > .github/workflows/deploy.yml > .gsd/PREFERENCES.md > .gsd/ROADMAP.md > .gsd/SPEC.md |
| Primary anchors | README.md, .github/workflows/deploy.yml, .gsd/PREFERENCES.md |
| Changed files | 0 |
| TODO notes | 0 |
| File budget used | 11% |
| Source budget used | 26% |
| Token estimate | 14282 |
| Contents mode | enabled |

## Handoff Guidelines

- Preserve user changes; avoid reverting unrelated work.
- Start with changed files and files marked `high-signal` in the manifest.
- Treat the Git diff as intent and verify changes in source files.
- Update this snapshot after meaningful edits or before handing off.

## Git Snapshot

| Field | Value |
| --- | --- |
| Branch | project/hello-world |
| Git root | /Users/jayakrishna |

Recent commits:
```text
1315279 Deploy built files
```

Status:
```text
clean or unavailable
```

## Project Map

```text
.github/
.github/workflows/
.gsd/
.github/workflows/deploy.yml
.gsd/PREFERENCES.md
.gsd/ROADMAP.md
.gsd/SPEC.md
.gsd/STATE.md
AGENTS.md
FDE_CURRICULUM_AND_ROADMAP.md
PROJECT_RULES.md
README.md
index.html
```

## File Manifest

| File | Bytes | Score | Why |
| --- | ---: | ---: | --- |
| README.md | 4401 | 105 | project-metadata, high-signal-doc |
| .github/workflows/deploy.yml | 912 | 0 | context |
| .gsd/PREFERENCES.md | 115 | 0 | context |
| .gsd/ROADMAP.md | 1777 | 0 | context |
| .gsd/SPEC.md | 1403 | 0 | context |
| .gsd/STATE.md | 1323 | 0 | context |
| AGENTS.md | 381 | 0 | context |
| PROJECT_RULES.md | 545 | 0 | context |
| FDE_CURRICULUM_AND_ROADMAP.md | 12971 | -1 | context |
| index.html | 33550 | -2 | context |

## Changed Files

No Git changes found, or this is not a Git repository.

## Git Diff Snippets

No diff available, or Git is unavailable.

## TODO / FIXME / HACK Notes

No TODO/FIXME/HACK notes found in selected files.

## Selected File Context

### README.md

| Field | Value |
| --- | --- |
| Bytes | 4401 |
| Score | 105 |
| Why | project-metadata, high-signal-doc |
| Status | Full content |


```markdown
# 🎯 Forward Deployed Engineer (FDE) — Roadmap & Live Progress Tracker

> A live interactive dashboard, master curriculum, and portfolio tracker for aspiring Forward Deployed Engineers (FDEs). Powered by GitHub Pages and automated GitHub Actions CI/CD.

![FDE Roadmap Banner](https://img.shields.io/badge/Role-Forward%20Deployed%20Engineer-indigo?style=for-the-badge)
![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-green?style=for-the-badge)
![Deployment](https://img.shields.io/badge/Hosting-GitHub%20Pages-blue?style=for-the-badge)

---

## 🌟 What This Repository Includes

1. **Live Interactive Dashboard (`index.html`)**:
   - Categorized by the **5 FDE Pillars**: Core Backend, Data & Ontologies, DevOps & Cloud, Applied AI / LLM, and Enterprise Security.
   - **4 Capstone Portfolio Projects** ready to build and publish.
   - Interactive progress bars, checkboxes with persistent `localStorage` progress saving, and Export/Import JSON capability.
   - Direct links to world-class free learning resources (MIT, CMU, DataTalks.Club, DeepLearning.AI, freeCodeCamp, etc.).
2. **Automated CI/CD Deployment (`.github/workflows/deploy.yml`)**:
   - Zero-configuration deployment straight to **GitHub Pages** on every `git push`.
3. **Master Syllabus & Curriculum Document (`FDE_CURRICULUM_AND_ROADMAP.md`)**:
   - 12-week study schedule, reading materials, and project specifications.

---

## 🚀 How to Make It Live on GitHub Pages (Step-by-Step)

Follow these quick steps to push this code to your GitHub account and activate the live site:

### Step 1: Create a new repository on GitHub
1. Go to [github.com/new](https://github.com/new).
2. Name your repository (e.g. `fde-roadmap-tracker` or `forward-deployed-engineer`).
3. Set visibility to **Public** and leave "Initialize with a README" unchecked.
4. Click **Create repository**.

### Step 2: Push your code from your terminal
Run the following commands in this directory:

```bash
# 1. Initialize git (if not already initialized)
git init

# 2. Stage and commit all files
git add .
git commit -m "feat: initial FDE curriculum and live tracking dashboard"

# 3. Rename branch to main
git branch -M main

# 4. Link your GitHub remote (replace with your GitHub username & repo name)
git remote add origin https://github.com/<YOUR-USERNAME>/<YOUR-REPO-NAME>.git

# 5. Push to GitHub
git push -u origin main
```

### Step 3: Enable GitHub Pages in your Repository Settings
1. On your GitHub repository page, click **Settings** (top navigation tab).
2. On the left sidebar, click **Pages** (under "Code and automation").
3. Under **Build and deployment** > **Source**, select:
   * **GitHub Actions** (Recommended — uses the automated workflow in `.github/workflows/deploy.yml`).
4. Once selected, go to the **Actions** tab in your repository. You will see the **Deploy FDE Tracker to GitHub Pages** workflow run automatically.
5. In ~1 minute, your live site URL will be displayed:
   `https://<YOUR-USERNAME>.github.io/<YOUR-REPO-NAME>/`

---

## 📚 The 5 Core Pillars & Project Capstones

| Pillar | Focus Areas | Key Free Resource |
| :--- | :--- | :--- |
| **1. Backend & Architecture** | Python AsyncIO, Typing, FastAPI, System Design | MIT Missing Semester, ArjanCodes, freeCodeCamp |
| **2. Data Engineering & Ontologies** | SQL, PostgreSQL, DuckDB, Polars, PySpark | CMU 15-445, Data Engineering Zoomcamp |
| **3. DevOps & Cloud** | Linux, Docker multi-stage, Kubernetes, Helm, Terraform | TechWorld with Nana, Kunal Kushwaha |
| **4. Applied AI & LLMs** | Hybrid RAG (pgvector + BM25), Agents, Ragas Evals | DeepLearning.AI, Andrej Karpathy, Full Stack LLM |
| **5. Enterprise & Security** | OAuth2/OIDC, Webhooks, Idempotency, OpenTelemetry | Stripe Webhook Guides, Prometheus/Grafana |

### Portfolio Projects to Build:
* **Project 1**: Enterprise Data Pipeline & Ontology Graph Engine
* **Project 2**: Production-Ready Enterprise RAG & Semantic Search with RBAC
* **Project 3**: High-Throughput Webhook Ingestion & Observability Gateway
* **Project 4**: Full-Stack FDE Operations Dashboard & K8s Deployment

---

## 🛠 Local Preview

To preview the dashboard locally in your browser before pushing:
* Double click `index.html` to open it in Chrome, Safari, or your preferred browser.
* Or run a simple local web server:
  ```bash
  python3 -m http.server 8000
  ```
  and visit `http://localhost:8000`.
```

### .github/workflows/deploy.yml

| Field | Value |
| --- | --- |
| Bytes | 912 |
| Score | 0 |
| Why | context |
| Status | Full content |


```yaml
name: Deploy FDE Tracker to GitHub Pages

on:
  push:
    branches: [ main, master ]
  workflow_dispatch:

# Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
permissions:
  contents: read
  pages: write
  id-token: write

# Allow one concurrent deployment
concurrency:
  group: "pages"
  cancel-in-progress: false

jobs:
  deploy:
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Repository
        uses: actions/checkout@v4

      - name: Setup GitHub Pages
        uses: actions/configure-pages@v4

      - name: Upload Pages Artifact
        uses: actions/upload-pages-artifact@v3
        with:
          # Upload entire repository root (includes index.html)
          path: '.'

      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v4
```

### .gsd/PREFERENCES.md

| Field | Value |
| --- | --- |
| Bytes | 115 |
| Score | 0 |
| Why | context |
| Status | Full content |


```markdown
---
version: 1
workflow:
  mode: spec-driven
  skip_discuss: false
  code_review: true
  atomic_commits: true
---
```

### .gsd/ROADMAP.md

| Field | Value |
| --- | --- |
| Bytes | 1777 |
| Score | 0 |
| Why | context |
| Status | Full content |


```markdown
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
```

### .gsd/SPEC.md

| Field | Value |
| --- | --- |
| Bytes | 1403 |
| Score | 0 |
| Why | context |
| Status | Full content |


```markdown
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
```

### .gsd/STATE.md

| Field | Value |
| --- | --- |
| Bytes | 1323 |
| Score | 0 |
| Why | context |
| Status | Full content |


```markdown
# GSD Project State: Forward Deployed Engineer (FDE) Track

**Objective:** FDE Zero-to-Hire Implementation Portfolio & Live GitHub Pages Tracker
**Status:** 🟢 Live Tracker Built & Ready to Deploy
**Current Focus:** Pushing to GitHub and launching GitHub Pages live tracking
**Updated:** 2026-11-13

---

## 📋 Active Tasks & Next Steps
1. [x] Built interactive tracking dashboard with local storage persistence ([index.html](file:///Users/jayakrishna/Desktop/rev_eng/index.html))
2. [x] Created automated GitHub Pages CI/CD workflow ([.github/workflows/deploy.yml](file:///Users/jayakrishna/Desktop/rev_eng/.github/workflows/deploy.yml))
3. [x] Generated GitHub setup guide & repository documentation ([README.md](file:///Users/jayakrishna/Desktop/rev_eng/README.md))
4. [ ] Push to GitHub repository and activate GitHub Pages (Instructions in README.md)
5. [ ] Begin **Pillar 1 / Milestone 1** implementation: Core Backend & Data Ingestion Engine

## 📌 Milestone Progress
- [x] **Milestone 0: Live Tracker Dashboard & CI/CD Setup** (Completed)
- [ ] **Milestone 1: Backend & Data Pipeline (Ontology Engine)**
- [ ] **Milestone 2: Applied AI & Enterprise RAG System**
- [ ] **Milestone 3: High-Throughput Webhook & Observability Gateway**
- [ ] **Milestone 4: Full-Stack FDE Operations Dashboard & K8s Deployment**
```

### AGENTS.md

| Field | Value |
| --- | --- |
| Bytes | 381 |
| Score | 0 |
| Why | context |
| Status | Full content |


```markdown
# TokenCap Start Here

Project intelligence is generated locally in `.tokencap/`.

1. Read `.tokencap/agent/START_HERE.md`.
2. Use `.tokencap/agent/allowed-context.json` to find task-relevant files.
3. Use the connected TokenCap MCP server for overview, search, impact, memory, and debug context.
4. Do not scan the repository broadly unless the generated context is insufficient.
```

### PROJECT_RULES.md

| Field | Value |
| --- | --- |
| Bytes | 545 |
| Score | 0 |
| Why | context |
| Status | Full content |


```markdown
# Project Rules & Guidelines (GSD Mode)

1. **Spec-Driven**: Never write speculative production code without referencing `.gsd/SPEC.md` and `.gsd/ROADMAP.md`.
2. **Context-Preserving**: Break large tasks into atomic phases to prevent context degradation and maintain high verification standards.
3. **Continuous State Updates**: Keep `.gsd/STATE.md` updated as phases and tasks are planned, executed, and completed.
4. **Verification Gates**: Every phase must pass explicit verification tests/audits before transitioning to the next milestone.
```

### FDE_CURRICULUM_AND_ROADMAP.md

| Field | Value |
| --- | --- |
| Bytes | 12971 |
| Score | -1 |
| Why | context |
| Status | Full content |


```markdown
# Forward Deployed Engineer (FDE) — Master Curriculum & Implementation Roadmap

> A complete zero-to-hire syllabus, free learning catalog, and hands-on portfolio plan for aspiring Forward Deployed Engineers (FDEs).

---

## 1. What is a Forward Deployed Engineer?

A **Forward Deployed Engineer (FDE)** (pioneered by Palantir and now essential at AI/data leaders like OpenAI, Scale AI, Databricks, and Anthropic) operates at the high-impact intersection of **Software Engineering**, **Data Engineering**, **Cloud/DevOps**, and **Client Architecture**.

```
            ┌─────────────────────────────────────────┐
            │       Forward Deployed Engineer         │
            └────────────────────┬────────────────────┘
                                 │
     ┌───────────────────┬───────┴───────────┬────────────────────┐
     ▼                   ▼                   ▼                    ▼
┌───────────────┐ ┌───────────────┐ ┌─────────────────┐ ┌──────────────────┐
│  Core Backend │ │     Data      │ │ Cloud, DevOps & │ │   Applied AI /   │
│  Engineering  │ │  Engineering  │ │   Deployment    │ │   LLM Systems    │
│ (Python/TS/Go)│ │(SQL/ETL/Spark)│ │ (Docker/K8s/IaC)│ │ (RAG/Agents/Evals│
└───────────────┘ └───────────────┘ └─────────────────┘ └──────────────────┘
```

FDEs embed directly with customers or product deployments to:
1. Ingest, sanitize, and model messy real-world customer data into clean schemas and business ontologies.
2. Build custom microservices, pipelines, dashboards, and integrations connecting enterprise systems to the core platform.
3. Deploy models and applications securely into complex environments (AWS, GCP, Azure, hybrid cloud, or air-gapped on-prem).
4. Act as technical advisors translating ambiguous business requirements into robust, production-grade code.

---

## 2. Complete 5-Pillar Syllabus

```
flowchart TD
    P1["Pillar 1: Core Backend & Architecture\nPython, FastAPI, System Design, REST/gRPC"] --> P2["Pillar 2: Data Engineering & Ontologies\nAdvanced SQL, Postgres, DuckDB, Spark, Data Modeling"]
    P2 --> P3["Pillar 3: DevOps, Containers & Cloud\nDocker, Kubernetes, AWS/GCP, Terraform, CI/CD"]
    P3 --> P4["Pillar 4: Applied AI & Modern Stack\nRAG, Vector DBs, LangChain/LlamaIndex, Evaluations"]
    P4 --> P5["Pillar 5: Enterprise Integration & Security\nOAuth2, OIDC, RBAC, Webhooks, API Reverse-Eng"]
    P5 --> Port["GitHub Portfolio Capstones\n4 Production-Grade Projects"]
```

---

### Pillar 1: Core Backend Engineering & Software Architecture

FDEs must write production-ready, clean, well-tested code fast.

* **Core Language (Python - Deep Dive)**:
  * Typing (`typing`, `Pydantic v2`), AsyncIO (`async`/`await`, event loops, concurrency vs parallelism).
  * Generators, context managers, decorators, object-oriented design & design patterns (Factory, Strategy, Adapter).
  * Packaging and dependency management: `uv` (modern), `Poetry`, virtual environments.
* **Secondary Language (Pick one)**:
  * **TypeScript/JavaScript**: Essential for building frontend dashboards or full-stack wrappers.
  * **Go**: Highly valued for low-latency microservices and cloud tooling.
* **API Development**:
  * **REST APIs**: FastAPI (request validation, dependency injection, middleware, background tasks).
  * **RPC/Streaming**: gRPC and Protocol Buffers, WebSockets for real-time telemetry.
* **System Design & Architecture**:
  * Microservices vs Modular Monolith, caching patterns (Redis: write-through, cache-aside), message queues (RabbitMQ, Redis Pub/Sub).
  * Rate limiting, circuit breakers, idempotency keys, retries with exponential backoff.

---

### Pillar 2: Data Engineering, Modeling & Ontologies

At least 40% of an FDE's time is spent wrestling customer data.

* **SQL Mastery**:
  * Window functions (`ROW_NUMBER()`, `RANK()`, `LEAD()`, `LAG()`, cumulative aggregations).
  * Common Table Expressions (CTEs), recursive CTEs.
  * Query optimization, execution plans (`EXPLAIN ANALYZE`), indexing strategies (B-Tree, GIN, Hash).
* **Database Systems**:
  * Relational: **PostgreSQL** (connection pooling with PgBouncer, JSONB querying, partitioning).
  * Analytical / Embedded OLAP: **DuckDB**, **ClickHouse**, or **Snowflake/BigQuery**.
* **Data Processing & Pipelines**:
  * Local/Fast: **Polars** and **Pandas** for rapid data transformations.
  * Distributed: **PySpark** basics (DataFrame API, transformations, actions, partitions, shuffling).
  * Orchestration: **Prefect** or **Apache Airflow** / **dbt** (data build tool) for transformation workflows.
* **Ontology & Schema Design**:
  * Entity-Relationship (ER) modeling, 3NF vs Star Schema / Snowflake Schema.
  * Palantir-style Ontology concepts: mapping raw rows into real-world Objects, Properties, Links, and Actions.

---

### Pillar 3: DevOps, Containers & Deployment

FDEs deploy code into customer infrastructure. You cannot rely on a dedicated DevOps team.

* **Linux Fundamentals & Shell Scripting**:
  * Process management, permissions, systemd, environment variables, networking commands (`curl`, `netstat`, `nslookup`, `ss`).
* **Containerization**:
  * **Docker**: Multi-stage builds, rootless containers, volume management, networking, optimizing image sizes (<100MB).
  * **Docker Compose**: Multi-container local environments (App + Postgres + Redis + MinIO).
* **Container Orchestration**:
  * **Kubernetes (K8s)**: Pods, Deployments, Services, ConfigMaps, Secrets, Ingress, Persistent Volumes.
  * Package management: **Helm** charts basics.
* **Cloud & Infrastructure as Code (IaC)**:
  * Core AWS or GCP services: IAM, VPCs, S3/Cloud Storage, ECS/EKS or Cloud Run.
  * **Terraform**: Declarative infrastructure provisioning (state management, variables, modules).
* **CI/CD & Observability**:
  * **GitHub Actions**: Linting, automated testing, container build & push to registries.
  * Observability: Structured logging (`structlog`), OpenTelemetry, Prometheus & Grafana dashboard metrics.

---

### Pillar 4: Applied AI & Enterprise LLM Systems (Modern FDE)

FDEs at modern startups bridge foundation models with messy corporate databases.

* **Retrieval-Augmented Generation (RAG)**:
  * Chunking strategies (semantic, recursive, hierarchical).
  * Embeddings models, Vector Databases (**pgvector**, **Qdrant**, or **Chroma**).
  * Hybrid search (dense vector + sparse BM25 keyword search), Cross-encoder Re-ranking.
* **LLM Orchestration & Structured Output**:
  * Function Calling / Tool Calling (OpenAI / Anthropic / Gemini SDKs).
  * Structured Outputs with Pydantic (`instructor` or native JSON schemas).
  * Frameworks: **LangChain**, **LlamaIndex**, or minimal custom pipelines with the official SDKs.
* **AI Agents & Enterprise Workflows**:
  * ReAct pattern, planning loops, error recovery, human-in-the-loop approvals.
* **Evaluation & Guardrails**:
  * LLM evaluation frameworks: **Ragas**, **TruLens**, or custom assertion suites.
  * Hallucination detection, latency monitoring, cost tracking (token counting).

---

### Pillar 5: Enterprise Integration, Security & Field Engineering

What distinguishes an FDE from a standard backend engineer:

* **Enterprise Authentication & Access Control**:
  * OAuth2.0 flows, OpenID Connect (OIDC), JWT tokens, SAML 2.0 overview.
  * Role-Based Access Control (RBAC) and Attribute-Based Access Control (ABAC).
* **API Integration & Data Extraction**:
  * Dealing with rate limits, pagination, webhooks, error formats, unmaintained third-party APIs.
  * Secure credential management (HashiCorp Vault, AWS Secrets Manager, `.env` hygiene).
* **Customer Interfacing Skills**:
  * Running technical discovery calls, writing Technical Design Documents (TDD), Scope of Work (SOW), and Architecture Diagrams.

---

## 3. High-Quality Free Courses & Open-Source Catalog

Every single topic above can be mastered through top-tier free courses:

| Topic | Course / Resource | Platform | Link / Provider |
| :--- | :--- | :--- | :--- |
| **Linux & Tools** | The Missing Semester of Your CS Education | YouTube / Web | MIT (`missing.csail.mit.edu`) |
| **Python & Architecture** | ArjanCodes / Corey Schafer | YouTube | Software Design Patterns in Python |
| **FastAPI & Microservices** | FastAPI Tutorial - Building Modern Backends | YouTube | freeCodeCamp / Amigoscode |
| **Backend & System Design** | Hussein Nasser / ByteByteGo / NeetCode | YouTube | Database internals, networking, System Design |
| **Data Engineering** | **Data Engineering Zoomcamp** (Gold Standard) | YouTube / GitHub | DataTalks.Club (`github.com/DataTalksClub/data-engineering-zoomcamp`) |
| **SQL & PostgreSQL** | CMU 15-445: Database Systems | YouTube / Web | Carnegie Mellon University (Andy Pavlo) |
| **Docker & Kubernetes** | DevOps Bootcamp / TechWorld with Nana | YouTube | TechWorld with Nana |
| **Kubernetes Deep-Dive** | Complete Kubernetes Course | YouTube | Kunal Kushwaha |
| **Terraform & Cloud** | Terraform Associate / AWS Cloud Practitioner | YouTube | freeCodeCamp (Andrew Brown) |
| **Applied AI & LLMs** | DeepLearning.AI Short Courses | Web | `deeplearning.ai` (Free interactive courses) |
| **LLMs from Scratch** | Neural Networks: Zero to Hero | YouTube | Andrej Karpathy |
| **Modern AI Systems** | Full Stack LLM Bootcamp | Web / YouTube | `fullstackdeeplearning.com` |

---

## 4. The 4 Portfolio Capstones (Ready to Build for GitHub)

To get hired as an FDE, your GitHub should prove you can integrate systems, process messy data, and deploy to real infrastructure.

### Project 1: Enterprise Data Pipeline & Ontology Graph Engine
* **Goal**: Ingest heterogeneous data (CSV/JSON/REST API), clean and normalize with Polars/DuckDB, load into PostgreSQL with a unified business ontology (Nodes, Links, Actions).
* **Stack**: Python, FastAPI, DuckDB, PostgreSQL, Docker, dbt.
* **Highlights**: Data validation with Great Expectations or Pydantic, automated schema migration, interactive API docs.

### Project 2: Production-Ready Enterprise RAG & Semantic Search
* **Goal**: Secure document search system for enterprise policies/documents with Role-Based Access Control (RBAC).
* **Stack**: Python/FastAPI, pgvector or Qdrant, hybrid search (BM25 + vector), re-ranking, token cost tracking.
* **Highlights**: Ragas evaluation suite proving precision/recall, automated ingestion pipeline for PDFs.

### Project 3: Client Data Ingestion Microservice & Webhook Gateway
* **Goal**: High-throughput webhook and batch ingestion service that handles unreliable customer data feeds, validates payloads, retries failed deliveries, and logs to OpenTelemetry.
* **Stack**: FastAPI / Go, Redis queue, PostgreSQL, Prometheus, Grafana.
* **Highlights**: Idempotency keys, rate limiter, dead-letter queue, live Grafana metrics dashboard.

### Project 4: Full-Stack FDE Operations Dashboard with K8s Deployment
* **Goal**: End-to-end deployed application featuring a Next.js / React management dashboard, backend API, multi-container Docker setup, and Helm charts for Kubernetes.
* **Stack**: Next.js (TypeScript), FastAPI, Docker, Kubernetes (Minikube / Kind), GitHub Actions CI/CD.
* **Highlights**: Complete 1-command deployment (`helm install` / `docker compose up`), comprehensive README with architecture diagram.

---

## 5. 12-Week Execution Roadmap

| Week | Focus | Hands-on Deliverable |
| :--- | :--- | :--- |
| **Week 1–2** | Python Mastery, FastAPI, AsyncIO, Pytest | REST API with Pydantic validation and full test suite |
| **Week 3–4** | SQL Mastery, PostgreSQL, Data Modeling & DuckDB | Complex SQL analytical queries + data ingestion script |
| **Week 5–6** | Docker, Docker Compose, Linux, GitHub Actions CI | Multi-container stack (API + DB + Redis) with automated CI |
| **Week 7** | Kubernetes basics & Cloud Deployment (AWS/GCP) | Deploy containerized service to local K8s / Cloud Run |
| **Week 8–9** | Vector Databases, Hybrid RAG, Function Calling | **Project 2 (Enterprise RAG with RBAC)** published on GitHub |
| **Week 10** | Data Pipelines, Ontologies & dbt / Spark | **Project 1 (Ontology Data Engine)** published on GitHub |
| **Week 11** | High-throughput Gateway & Observability | **Project 3 (Webhook Gateway + Grafana)** published on GitHub |
| **Week 12** | Full-Stack Dashboard, System Design Mock Interviews | **Project 4 (Full-Stack Deployment)** + Resume & Outreach |
```

### index.html

| Field | Value |
| --- | --- |
| Bytes | 33550 |
| Score | -2 |
| Why | context |
| Status | Truncated (budget limit) |

**Structural Outline:**
  - `fn loadState` (line 498)
  - `fn saveState` (line 514)
  - `fn updateDashboard` (line 524)
  - `fn renderCards` (line 543)


```html
// … lines 1–46
<!DOCTYPE html>
<html lang="en" class="dark">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Forward Deployed Engineer (FDE) — Roadmap & Live Tracker</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          colors: {
            brand: {
              50: '#eef2ff',
              100: '#e0e7ff',
              500: '#6366f1',
              600: '#4f46e5',
              700: '#4338ca',
              900: '#1e1b4b',
            }
          }
        }
      }
    }
  </script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
  <style>
    /* Custom scrollbar */
    ::-webkit-scrollbar { width: 8px; height: 8px; }
    ::-webkit-scrollbar-track { background: #0f172a; }
    ::-webkit-scrollbar-thumb { background: #334155; border-radius: 4px; }
    ::-webkit-scrollbar-thumb:hover { background: #475569; }
  </style>
</head>
<body class="bg-slate-950 text-slate-100 min-h-screen flex flex-col font-sans selection:bg-indigo-500 selection:text-white">

  <!-- Header -->
  <header class="border-b border-slate-800 bg-slate-900/80 backdrop-blur sticky top-0 z-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex flex-wrap items-center justify-between gap-4">
      <div class="flex items-center gap-3">
        <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-indigo-600 to-violet-500 flex items-center justify-center shadow-lg shadow-indigo-500/20 text-white font-bold text-xl">
          <i class="fa-solid fa-compass"></i>
        </div>
        <div>
          <h1 class="text-xl font-bold tracking-tight bg-gradient-to-r from-white via-slate-200 to-indigo-300 bg-clip-text text-transparent">
// … lines 497–502

    function loadState() {
      try {
        const raw = localStorage.getItem(STORAGE_KEY);
        if (raw) return JSON.parse(raw);
      } catch (e) {
// … lines 513–518

    function saveState() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(appState));
      updateDashboard();
    }

// … lines 523–528

    function updateDashboard() {
      const total = CURRICULUM.length;
      const completedCount = Object.values(appState.completed).filter(Boolean).length;
      const percentage = Math.round((completedCount / total) * 100) || 0;

// … lines 542–547

    function renderCards() {
      const container = document.getElementById("cardsContainer");
      const emptyState = document.getElementById("emptyState");

      const filtered = CURRICULUM.filter(item => {
```