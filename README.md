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

