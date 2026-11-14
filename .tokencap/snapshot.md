<!-- TokenCap v1.6 Savings: baseline 17,340 tok → actual 8,233 tok (52.5% saved) -->
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
| Generated | 2026-11-14T11:20:11.911Z |
| Workspace | /Users/jayakrishna/Desktop/rev_eng |
| Profile | balanced |
| Selected files | 10 |
| Source bytes | 66218 |
| Estimated source tokens | 17375 |

## Read First

This file is a compressed coding-session handoff. Read it before editing, then inspect the referenced files directly. Prefer the live repository over this snapshot when there is a conflict.

## TokenCap Intelligence Files

- TOKENCAP_GRAPH.md — Project dependency and architecture graph *(JS/TS projects only)*
- TOKENCAP_MEMORY.md — Developer notes, current task, constraints, and context memory

## Handoff Summary

| Field | Value |
| --- | --- |
| Read order | .gsd/STATE.md > FDE_CURRICULUM_AND_ROADMAP.md > index.html > README.md > .github/workflows/deploy.yml |
| Primary anchors | .gsd/STATE.md, FDE_CURRICULUM_AND_ROADMAP.md, index.html |
| Changed files | 3 |
| TODO notes | 0 |
| File budget used | 11% |
| Source budget used | 30% |
| Token estimate | 17375 |
| Contents mode | enabled |

## Handoff Guidelines

- Preserve user changes; avoid reverting unrelated work.
- Start with changed files and files marked `high-signal` in the manifest.
- Treat the Git diff as intent and verify changes in source files.
- Update this snapshot after meaningful edits or before handing off.

## Git Snapshot

| Field | Value |
| --- | --- |
| Branch | main |
| Git root | /Users/jayakrishna/Desktop/rev_eng |

Recent commits:
```text
163e462 feat: initial FDE live tracker dashboard and CI/CD
```

Status:
```text
 M .gsd/STATE.md
 M FDE_CURRICULUM_AND_ROADMAP.md
 M index.html
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
| .gsd/STATE.md | 1734 | 120 | changed |
| FDE_CURRICULUM_AND_ROADMAP.md | 14696 | 119 | changed |
| index.html | 40254 | 117 | changed |
| README.md | 4401 | 105 | project-metadata, high-signal-doc |
| .github/workflows/deploy.yml | 912 | 0 | context |
| .gsd/PREFERENCES.md | 115 | 0 | context |
| .gsd/ROADMAP.md | 1777 | 0 | context |
| .gsd/SPEC.md | 1403 | 0 | context |
| AGENTS.md | 381 | 0 | context |
| PROJECT_RULES.md | 545 | 0 | context |

## Changed Files

-  M .gsd/STATE.md
-  M FDE_CURRICULUM_AND_ROADMAP.md
-  M index.html

## Git Diff Snippets

### Unstaged Changes Diff

```diff
// … lines 1171–1176
 
     function loadState() {
       try {
@@ -516,7 +625,6 @@
       updateDashboard();
     }
```

## TODO / FIXME / HACK Notes

No TODO/FIXME/HACK notes found in selected files.

## Selected File Context

### .gsd/STATE.md

| Field | Value |
| --- | --- |
| Bytes | 1734 |
| Score | 120 |
| Why | changed |
| Status | Full content |


```markdown
# GSD Project State: Forward Deployed Engineer (FDE) & Applied AI Track

**Objective:** Complete Master Curriculum (LLMs, Advanced RAG, Agentic AI, Real-Time Systems, Evals) & Live GitHub Pages Tracker
**Status:** 🟢 Live Interactive Dashboard & Master Syllabus Expanded
**Current Focus:** Ready to commit & push to GitHub Pages; Begin Milestone 1
**Updated:** 2026-11-14

---

## 📋 Active Tasks & Next Steps
1. [x] Comprehensive LLM, RAG, Agentic AI & Real-Time curriculum authored ([FDE_CURRICULUM_AND_ROADMAP.md](file:[REDACTED:ENTROPY].md))
2. [x] Interactive live dashboard updated with full AI concept cards, category filters, and study links ([index.html](file:///Users/jayakrishna/Desktop/rev_eng/index.html))
3. [x] GitHub Actions deployment workflow active ([.github/workflows/deploy.yml](file:///Users/jayakrishna/Desktop/rev_eng/.github/workflows/deploy.yml))
4. [ ] Commit and push changes to trigger automated GitHub Pages live rebuild
5. [ ] Choose first implementation milestone:
   - **Milestone 1**: Data Pipeline & Business Ontology Engine (Python, DuckDB, Postgres, FastAPI)
   - **Milestone 2**: Enterprise RAG with Hybrid Search, Cohere Re-Ranking & RBAC (pgvector, Qdrant, Ragas)
   - **Milestone 3**: Autonomous Multi-Agent System with LangGraph & Model Context Protocol (MCP)

## 📌 Milestone Progress
- [x] **Milestone 0: Interactive Live Tracker & Complete Syllabus** (Completed)
- [ ] **Milestone 1: Backend & Data Ingestion (Ontology Engine)**
- [ ] **Milestone 2: Production Enterprise RAG & Hybrid Search**
- [ ] **Milestone 3: Agentic AI, Memory & Multi-Agent Orchestration**
- [ ] **Milestone 4: Real-Time Streaming, Evals & Full-Stack Deployment**
```

### FDE_CURRICULUM_AND_ROADMAP.md

| Field | Value |
| --- | --- |
| Bytes | 14696 |
| Score | 119 |
| Why | changed |
| Status | Truncated (budget limit) |


```markdown
// … lines 1–29
# Comprehensive Master Syllabus: Modern Applied AI, LLMs, RAG & Agentic Systems

> A complete zero-to-production curriculum covering LLM internals, Advanced RAG, Multi-Agent Architectures, Real-Time Streaming, Evals, and Enterprise Deployment.

---

## 🗺️ Architectural Concept Map

```
flowchart TD
    subgraph Core ["1. LLM Core & Architecture"]
        Trans["Transformer Internals\n(Self-Attention, RoPE, KV Cache)"]
        Token["Tokenization & Context Windows\n(BPE, Tiktoken, Lost-in-the-Middle)"]
        Struct["Structured Outputs & Validation\n(Pydantic, Instructor, JSON Schema)"]
        FineTune["Fine-Tuning & Alignment\n(LoRA, QLoRA, DPO, SFT)"]
        Inference["Inference Acceleration & Local\n(vLLM, Ollama, GGUF, Quantization)"]
    end

    subgraph RAG ["2. Production & Advanced RAG"]
        Chunk["Chunking & Preprocessing\n(Recursive, Semantic, Document Layout)"]
        Embed["Embeddings & Representations\n(Dense, Sparse BM25/SPLADE, ColBERT)"]
        Vect["Vector Stores & Indexing\n(pgvector, Qdrant, HNSW, Hybrid Search)"]
        Rerank["Re-Ranking & Fusion\n(Cross-Encoders, Cohere, RRF)"]
        AdvRAG["Contextual & Graph RAG\n(HyDE, Parent-Doc, GraphRAG, Neo4j)"]
    end

    subgraph Agents ["3. Agentic AI & Autonomous Systems"]
        AgentCore["Core Agent Loops\n(ReAct, Plan-and-Solve, Tool Calling)"]
        Memory["Memory Architectures\n(Short-term, Vector Episodic, Semantic, Mem0)"]
// … lines 42–70
    RAG --> Agents
    Agents --> RealTime
```

---

## 📚 Detailed Domain Breakdown & Where to Study

---

### Domain 1: LLM Core Foundations & Architecture

#### 1. Transformer Architecture & Attention Deep Dive
* **What to Learn:**
  * Self-Attention, Multi-Head Attention, Scaled Dot-Product calculation.
  * Modern attention variants: Grouped-Query Attention (GQA), Multi-Query Attention (MQA), FlashAttention (IO-awareness).
  * Positional Encodings: Sinusoidal vs Rotary Position Embeddings (RoPE) vs ALiBi.
  * KV Cache (Key-Value Cache): how generative autoregression works and memory consumption calculation.
* **Where to Study:**
  * 📺 [Andrej Karpathy: Let's build GPT: from scratch, in code, spelled out](https://www.youtube.com/watch?v=kCc8FmEb1nY) (YouTube)
  * 📄 [Attention Is All You Need (Vaswani et al.)](https://arxiv.org/abs/1706.03762)
  * 📖 [Jay Alammar: The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/)

#### 2. Tokenization & Context Windows
* **What to Learn:**
  * Byte-Pair Encoding (BPE), WordPiece, SentencePiece, and Tiktoken.
  * Special tokens (`<|im_start|>`, `<|endoftext|>`), vocabulary size tradeoffs.
  * The "Lost in the Middle" phenomenon in long context windows (128k to 2M+ tokens).
* **Where to Study:**
// … lines 83–111

#### 4. Fine-Tuning & Parameter-Efficient Tuning (PEFT)
* **What to Learn:**
  * SFT (Supervised Fine-Tuning) data preparation and formatting.
  * LoRA (Low-Rank Adaptation) and QLoRA (Quantized LoRA) mathematical intuition.
  * Alignment algorithms: RLHF (PPO) vs DPO (Direct Preference Optimization) vs ORPO.
* **Where to Study:**
  * 🎓 [Hugging Face: Deep RL & Alignment Course](https://huggingface.co/learn)
  * 📺 [Umar Jamil: LoRA (Low-Rank Adaptation) Explained Visually](https://www.youtube.com/watch?v=PXOIvdI73bs) (YouTube)
  * 📖 [Axolotl & Unsloth Guides for Fast Fine-Tuning](https://docs.unsloth.ai/)

#### 5. Local Inference Acceleration & Quantization
* **What to Learn:**
  * Quantization algorithms: GGUF, AWQ (Activation-aware Weight Quantization), GPTQ, BitsAndBytes (4-bit/8-bit).
  * High-throughput serving engines: **vLLM** (PagedAttention), **TGI** (Text Generation Inference), **Ollama**, **llama.cpp**.
  * Continuous batching, speculative decoding, chunked prefill.
* **Where to Study:**
  * 📖 [vLLM Official Documentation & Architecture Guide](https://docs.vllm.ai/)
  * 💻 [Ollama GitHub & Setup](https://github.com/ollama/ollama)
  * 📄 [PagedAttention Paper (Woosuk Kwon et al.)](https://arxiv.org/abs/2309.06180)

---

### Domain 2: Advanced & Production RAG

#### 1. Advanced Chunking & Document Parsing
* **What to Learn:**
  * Fixed-size vs Recursive Character vs Token chunking.
  * Document-structure-aware parsing (Unstructured, LlamaParse, MinerU) for tables, headers, PDFs.
// … lines 124–152
  * 📄 [ColBERT Paper: Efficient and Effective Passage Search via Contextualized Late Interaction](https://arxiv.org/abs/2004.12832)

#### 3. Vector Storage, Indexing & Hybrid Search
* **What to Learn:**
  * Vector index algorithms: HNSW (Hierarchical Navigable Small World), IVF-FLAT, Product Quantization (PQ).
  * PostgreSQL integration: **pgvector** (`vector_cosine_ops`, HNSW indexes).
  * Dedicated engines: **Qdrant**, **Milvus**, **Chroma**.
  * Hybrid Search: combining Dense + BM25 using Reciprocal Rank Fusion (RRF).
* **Where to Study:**
  * 💻 [pgvector Official GitHub & Indexing Guide](https://github.com/pgvector/pgvector)
  * 📖 [Qdrant Hybrid Search & RRF Documentation](https://qdrant.tech/documentation/concepts/hybrid-queries/)

#### 4. Re-Ranking & Context Enrichment
* **What to Learn:**
  * Cross-Encoders vs Bi-Encoders: trade-off between latency and accuracy.
  * Re-ranking models: Cohere Rerank, BGE-Reranker-Large, FlashRank.
  * Anthropic Contextual Retrieval (pre-pending document-level context to chunks before embedding).
  * Hypothetical Document Embeddings (HyDE) and Query Expansion (Multi-Query generation).
* **Where to Study:**
  * 📖 [Anthropic: Introducing Contextual Retrieval](https://www.anthropic.com/news/contextual-retrieval)
  * 🎓 [DeepLearning.AI: Building & Evaluating Advanced RAG](https://www.deeplearning.ai/short-courses/building-evaluating-advanced-rag/)

#### 5. Graph RAG & Knowledge Graph Traversal
* **What to Learn:**
  * Extracting Entities and Relationships from unstructured text using LLMs.
  * Microsoft GraphRAG: Hierarchical community detection (Leiden algorithm) and global summaries.
  * Graph databases: **Neo4j** (Cypher queries), graph traversals combined with vector search.
* **Where to Study:**
  * 💻 [Microsoft GraphRAG Official Repository & Paper](https://github.com/microsoft/graphrag)
// … lines 165–193
  * 📄 [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629)
  * 📖 [Model Context Protocol (MCP) Official Documentation](https://modelcontextprotocol.io/)
  * 🎓 [DeepLearning.AI: Functions, Tools and Agents with LangChain](https://www.deeplearning.ai/short-courses/functions-tools-agents-langchain/)

#### 2. Agent Memory Architectures
* **What to Learn:**
  * Short-term memory: conversation buffer, summarization memory, sliding windows.
  * Long-term memory: semantic vector retrieval, user profile stores.
  * Modern memory frameworks: **Mem0**, **Letta (formerly MemGPT)** (virtual context paging like OS memory).
* **Where to Study:**
  * 💻 [Mem0: The Memory Layer for AI Applications](https://github.com/mem0ai/mem0)
  * 📄 [MemGPT: Towards LLMs as Operating Systems](https://arxiv.org/abs/2310.08560)

#### 3. Multi-Agent Orchestration Frameworks
* **What to Learn:**
  * State Graph Agents: **LangGraph** (cyclical graphs, persistence, state reducers, time-travel).
  * Role-playing multi-agent systems: **CrewAI**, **AutoGen** (Microsoft).
  * Multi-agent communication topologies: Hierarchical Supervisor, Choreography (Peer-to-Peer), Swarm.
* **Where to Study:**
  * 🎓 [LangChain: LangGraph Academy (Free Official Course)](https://academy.langchain.com/)
  * 🎓 [DeepLearning.AI: Multi AI Agent Systems with crewAI](https://www.deeplearning.ai/short-courses/multi-ai-agent-systems-with-crewai/)
  * 💻 [OpenAI Swarm GitHub (Educational Lightweight Orchestration)](https://github.com/openai/swarm)

#### 4. Guardrails, Security & Human-in-the-Loop (HITL)
* **What to Learn:**
  * Vulnerabilities: Prompt Injections, Jailbreaking, Indirect Injections, Data exfiltration via Markdown.
  * Guardrail systems: **NeMo Guardrails** (NVIDIA), **Llama Guard** (Meta), **Guardrails AI**.
  * HITL: Pause-and-resume workflows, human approval gates before executing critical tools (e.g. SQL writes, API payments).
* **Where to Study:**
// … lines 206–234
* **Where to Study:**
  * 📖 [MDN Web Docs: Server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events)
  * 📖 [OpenAI Realtime API Guide](https://platform.openai.com/docs/guides/realtime)
  * 💻 [Google GenAI SDK Python Live Streaming](https://github.com/google-gemini/cookbook)

#### 2. Evaluation Frameworks & LLM-as-a-Judge
* **What to Learn:**
  * RAG Triad: Context Relevance, Groundedness (Faithfulness), Answer Relevance.
  * Automated metrics: **Ragas**, **DeepEval**, **TruLens**.
  * Synthetic dataset generation (Testset generation from knowledge documents).
  * G-Eval and custom rubrics using frontier models as judges.
* **Where to Study:**
  * 📖 [Ragas Framework Documentation & Tutorials](https://docs.ragas.io/)
  * 💻 [DeepEval GitHub: The Evaluation Framework for LLMs](https://github.com/confident-ai/deepeval)
  * 🎓 [DeepLearning.AI: Evaluating and Debugging Generative AI Models](https://www.deeplearning.ai/short-courses/evaluating-debugging-generative-ai/)

#### 3. Observability, Tracing & Cost Optimization
* **What to Learn:**
  * Distributed tracing for LLM calls: **Langfuse** (open-source), **Arize Phoenix**, **LangSmith**.
  * OpenTelemetry for Generative AI semantic conventions.
  * Cost & Latency reduction: Prompt Caching (Anthropic / Gemini prompt caching), Semantic Caching (GPTCache / Redis).
* **Where to Study:**
  * 💻 [Langfuse: Open Source LLM Engineering Platform](https://langfuse.com/docs)
  * 💻 [Arize Phoenix: AI Observability & Tracing](https://phoenix.arize.com/)
  * 📖 [Anthropic: Prompt Caching Documentation](https://docs.anthropic.com/en/docs/build-with-claude/prompt-caching)

---

## 🏆 Top 10 Free Comprehensive Online Courses

/* …72 lines not shown — file has no detected definitions; ask for full content if needed. */
```

### index.html

| Field | Value |
| --- | --- |
| Bytes | 40254 |
| Score | 117 |
| Why | changed |
| Status | Truncated (budget limit) |

**Structural Outline:**
  - `fn loadState` (line 607)
  - `fn saveState` (line 623)
  - `fn updateDashboard` (line 632)
  - `fn renderCards` (line 650)


```html
// … lines 1–46
<!DOCTYPE html>
<html lang="en" class="dark">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Applied AI, LLMs, RAG & Agentic Systems — Master Tracker</title>
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
        <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-indigo-600 via-purple-600 to-pink-500 flex items-center justify-center shadow-lg shadow-indigo-500/20 text-white font-bold text-xl">
          <i class="fa-solid fa-brain"></i>
        </div>
        <div>
          <h1 class="text-xl font-bold tracking-tight bg-gradient-to-r from-white via-slate-200 to-indigo-300 bg-clip-text text-transparent">
// … lines 606–611

    function loadState() {
      try {
        const raw = localStorage.getItem(STORAGE_KEY);
        if (raw) return JSON.parse(raw);
      } catch (e) {
// … lines 622–627

    function saveState() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(appState));
      updateDashboard();
    }

// … lines 631–636

    function updateDashboard() {
      const total = CURRICULUM.length;
      const completedCount = Object.values(appState.completed).filter(Boolean).length;
      const percentage = Math.round((completedCount / total) * 100) || 0;

// … lines 649–654

    function renderCards() {
      const container = document.getElementById("cardsContainer");
      const emptyState = document.getElementById("emptyState");

      const filtered = CURRICULUM.filter(item => {
```

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