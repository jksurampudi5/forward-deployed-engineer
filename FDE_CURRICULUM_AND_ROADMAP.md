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
        Orchestration["Multi-Agent Frameworks\n(LangGraph, CrewAI, AutoGen, Swarm)"]
        Protocols["Protocols & Sandboxes\n(Model Context Protocol - MCP, Code Execution)"]
        Safety["Guardrails & Human-in-the-Loop\n(Llama Guard, NeMo, Approval Gates)"]
    end

    subgraph RealTime ["4. Real-Time & Systems Engineering"]
        Stream["Streaming & Protocols\n(SSE, WebSockets, Bidirectional Audio/Video)"]
        Cache["Latency & Cost Optimization\n(Prompt Caching, Semantic Cache, Prefetching)"]
        Evals["Evals & Observability\n(Ragas, TruLens, DeepEval, Langfuse, Tracing)"]
    end

    Core --> RAG
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
  * 📺 [Andrej Karpathy: Let's build the GPT Tokenizer](https://www.youtube.com/watch?v=zduSFxRajkE) (YouTube)
  * 📄 [Lost in the Middle: How Language Models Use Long Contexts](https://arxiv.org/abs/2307.03172)

#### 3. Structured Outputs & Schema Enforcement
* **What to Learn:**
  * Forcing LLMs to output valid JSON conforming to strict schemas.
  * Constrained decoding: Finite State Machines (FSMs), CFG Grammars (Context-Free Grammars).
  * Libraries: `instructor`, `outlines`, native OpenAI/Gemini/Anthropic JSON schema response formats.
* **Where to Study:**
  * 📖 [Instructor Library Documentation (Python/TypeScript)](https://python.useinstructor.com/)
  * 📖 [Outlines: Structured Generation Documentation](https://dottxt-ai.github.io/outlines/)
  * 🌐 [OpenAI Structured Outputs Guide](https://platform.openai.com/docs/guides/structured-outputs)

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
  * Semantic chunking (embedding similarity splits) and Hierarchical chunking (parent-child documents).
* **Where to Study:**
  * 🎓 [DeepLearning.AI: Preprocessing Unstructured Data for LLM Applications](https://www.deeplearning.ai/short-courses/preprocessing-unstructured-data-for-llm-applications/)
  * 📖 [LlamaIndex Chunking Strategies Guide](https://docs.llamaindex.ai/)

#### 2. Embeddings & Representation Models
* **What to Learn:**
  * Dense embeddings (OpenAI text-embedding-3, BAAI/bge, voyage-ai).
  * Sparse representations (BM25 keyword search, SPLADE learned sparse vectors).
  * Multi-vector late interaction: **ColBERT** (Token-level contextual embeddings).
* **Where to Study:**
  * 📖 [MTEB (Massive Text Embedding Benchmark) Leaderboard](https://huggingface.co/spaces/mteb/leaderboard)
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
  * 📖 [Neo4j GenAI Ecosystem & GraphRAG](https://neo4j.com/developer/genai-ecosystem/)

---

### Domain 3: Agentic AI & Autonomous Multi-Agent Systems

#### 1. Core Agent Control Loops & Tool Use
* **What to Learn:**
  * Patterns: **ReAct** (Reason + Act), **Plan-and-Solve**, **Reflexion** (verbal reinforcement learning).
  * Native Function / Tool Calling (schema registration, argument validation, error recovery loops).
  * Model Context Protocol (**MCP**): Anthropic's open standard for secure server-agent tool communication.
* **Where to Study:**
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
  * 📖 [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
  * 📖 [NVIDIA NeMo Guardrails Documentation](https://docs.nvidia.com/nemo/guardrails/)

---

### Domain 4: AI Systems Engineering, Real-Time & Evals

#### 1. Real-Time Streaming & Protocols
* **What to Learn:**
  * Server-Sent Events (SSE) for token streaming in web apps.
  * Bi-directional WebSockets for low-latency voice, audio, and multimodal interactions.
  * Modern streaming APIs: Gemini Live API, OpenAI Realtime API.
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

1. **[DataTalks.Club: LLM Zoomcamp](https://github.com/DataTalksClub/llm-zoomcamp)** (Free, open-source, hands-on RAG, search, and deployment)
2. **[Andrej Karpathy: Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html)** (The deepest theoretical understanding of Transformers and GPT)
3. **[DeepLearning.AI Short Courses](https://www.deeplearning.ai/short-courses/)** (1-2 hour focused hands-on labs with Andrew Ng and industry leaders)
4. **[LangChain: LangGraph Academy](https://academy.langchain.com/)** (Comprehensive course on cyclical, stateful AI agents)
5. **[Full Stack LLM Bootcamp](https://fullstackdeeplearning.com/llm-bootcamp/)** (End-to-end engineering from models to product)
6. **[Hugging Face: Natural Language Processing Course](https://huggingface.co/learn/nlp-course)** (Transformers, fine-tuning, tokenizers)
7. **[CMU CS 11-711: Advanced NLP](http://phontron.com/class/anlp2024/)** (Carnegie Mellon's graduate-level AI course on YouTube)
8. **[Microsoft: Generative AI for Beginners](https://github.com/microsoft/generative-ai-for-beginners)** (21-lesson open-source curriculum)
9. **[LlamaIndex: Building Production RAG](https://docs.llamaindex.ai/)** (Full architectural guides and code tutorials)
10. **[Eugene Yan's Patterns for Building LLM Systems](https://eugeneyan.com/writing/llm-patterns/)** (Industry-standard architectural blueprints)
