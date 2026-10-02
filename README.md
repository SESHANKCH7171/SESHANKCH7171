# Hi, I'm Seshank Chinnapotula 👋
### AI Agent Engineer | Multi-Agent Systems · Real-Time WebRTC Voice · Enterprise RAG & Security

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/seshankch)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/seshankch7171)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:seshankch7171@gmail.com)
[![YouTube Demo](https://img.shields.io/badge/Live_Voice_Demo-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/lGpPy6ma4SQ)

---

## ⚡ Engineering Philosophy
> **"Draw the line between deterministic logic and LLM reasoning."**  
> Moving beyond basic prompt wrappers and toy demos. I build production-ready multi-agent workflows, sub-second multimodal voice pipelines, and hardened enterprise RAG platforms designed for real deployment constraints: **low latency, zero hallucination on metrics, API cost control, and rigorous quantitative evaluation.**

🎓 **IIT Madras Dual Degree (B.Tech + M.Tech)** in Aerospace Engineering.

---

## 🧭 Agent Engineering Blueprint

```
System Requirements ➔ State Machine Topology (LangGraph) ➔ Deterministic Tool Contracts (Pydantic) ➔ Guardrail Policies (Colang) ➔ Retrieval & Reranking Funnel ➔ Gateway & Fallbacks ➔ Golden Evaluation Benchmarks (RAGAS) ➔ Telemetry & Distributed Tracing
```

I don't build demos that look good once and fail in the wild. I build deterministic agent state machines with explicit failure boundaries, automated fallback routes, and measurable production unit economics.

---

## 🛠️ Core Technical Stack

```
Agent Architecture    │ Python 3.11+, LangGraph, LangChain, Multi-Agent Systems, Tool Calling, Pydantic Schemas
Voice & Multimodal    │ LiveKit WebRTC, Groq LPUs (Whisper Large V3), Deepgram Aura-2, Silero VAD
Retrieval & Vectors   │ Qdrant Cloud (HNSW), ChromaDB, FlashRank (TinyBERT Cross-Encoder), Document AI
Security & Guardrails │ NeMo Guardrails (Colang 1.0/2.0), RBAC Route Interceptors, Portkey AI Gateway
Eval & Observability  │ RAGAS (LLM-as-a-Judge), Pydantic Logfire Tracing, LangSmith Telemetry
Cloud & Backend Ops   │ FastAPI, Google Cloud Run, Vertex AI, Docker, SQLModel / SQLite (WAL mode), APScheduler
```

---

## 📌 Featured Flagship Systems

### 🏨 [Hotel GM Intelligence Copilot 3.0](https://github.com/SESHANKCH7171/HOTEL_GM_SYSTEM_3.0)
*Autonomous Multi-Agent Hotel Operations Analytics & Real-Time WebRTC Voice Agent*

[![Live Voice Demo](https://img.shields.io/badge/Watch_Live_Voice_Demo-YouTube-red?style=flat-square&logo=youtube)](https://youtu.be/lGpPy6ma4SQ)
[![LangGraph](https://img.shields.io/badge/Orchestrator-LangGraph-orange.svg?style=flat-square)](https://github.com/langchain-ai/langgraph)
[![LiveKit WebRTC](https://img.shields.io/badge/Transport-LiveKit_WebRTC-purple.svg?style=flat-square)](https://livekit.io/)
[![Groq LPU](https://img.shields.io/badge/Inference-Groq_LPU-green.svg?style=flat-square)](https://groq.com/)

* **The Problem:** Hotel General Managers spend hours manually pulling operational metrics from fragmented PMS, RMS, and payroll databases. Standard LLMs hallucinate financial KPIs (RevPAR, ADR, labor variance), making them unusable for executive decisions.
* **The Solution:** Architected a deterministic multi-agent state machine in **LangGraph** separating KPI computation from LLM interpretation. Bridged browser audio to **LiveKit WebRTC** Cloud connected to **Groq LPUs** (`whisper-large-v3` + `gpt-oss-20b`) and **Deepgram Aura-2** streaming speech synthesis.
* **Conversational UX:** Integrated **Silero VAD** with turn-commit heuristics to eliminate crosstalk and handle real-time interruptions seamlessly.
* **Hybrid Data Sync:** Simultaneously streams structured operational tables to an executive **Streamlit** dashboard while delivering concise audio briefs through low-latency WebRTC data tracks.
* 📊 **Verified Metrics:** **891ms** LLM Time-to-First-Token (TTFT) | **3.0s** end-to-end voice turnaround | **0%** math hallucination.

---

### 🛡️ [Enterprise Agentic RAG & AI Security Platform for STRIPE](https://github.com/SESHANKCH7171/enterprise-rag-with-gcp)
*Production RAG Architecture with Upstream Guardrails, Intelligent Gateway, and RAGAS Evals*

[![NeMo Guardrails](https://img.shields.io/badge/Security-NeMo_Guardrails_Colang-brightgreen?style=flat-square)](https://github.com/NVIDIA/NeMo-Guardrails)
[![Qdrant](https://img.shields.io/badge/Vector_DB-Qdrant_HNSW-red?style=flat-square)](https://qdrant.tech/)
[![RAGAS](https://img.shields.io/badge/Evals-RAGAS_Framework-blue?style=flat-square)](https://github.com/explodinggradients/ragas)
[![Docker](https://img.shields.io/badge/Deployment-Cloud_Run_Docker-2496ED?style=flat-square&logo=docker)](https://cloud.google.com/run)

* **The Problem:** Deploying LLMs over 4,000+ technical documentation pages introduces major security vulnerabilities (prompt injection, secret leaks, API fraud bypass) and high token latency from bloated context windows.
* **Two-Stage Retrieval Funnel:** Parsed 4,000+ technical docs from `docs.stripe.com` via **Document AI**. Combined dense **Qdrant HNSW** vector search with a local **FlashRank (TinyBERT)** cross-encoder, boosting Context Precision to **0.93** while reducing prompt tokens by **65%**.
* **Upstream Security Gate:** Enforced **NeMo Guardrails** with custom **Colang** policies upstream of LLM inference, neutralizing prompt injections, credential leaks, and fraud jailbreak attempts across attack benchmarks with zero false positives.
* **Resilience & Evaluation:** Orchestrated intent-based planning in **LangGraph** with a **Portkey AI Gateway** and automated Groq fallbacks (**1.00 Tool Correctness**). Validated against a 15-scenario golden evaluation set with **RAGAS** and **Pydantic Logfire** distributed tracing (**0.80 Answer Relevancy**, **0.75 Answer Correctness**).
* **Containerization:** Engineered a dual-manifest Docker build for **Google Cloud Run**, slashing image size by **85% (3.5 GB → 520 MB)**.

---

### 🎯 [SmartReco.ai — Proactive Recommendation Engine](https://github.com/SESHANKCH7171/smartreco-ai-engine)
*Event-Driven Asynchronous Multi-Agent Recommendation Platform*

[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?style=flat-square&logo=fastapi)](https://fastapi.tiangolo.com/)
[![LangGraph](https://img.shields.io/badge/State_Machine-LangGraph-orange?style=flat-square)](https://github.com/langchain-ai/langgraph)
[![ChromaDB](https://img.shields.io/badge/Vector_Store-ChromaDB-lightblue?style=flat-square)](https://www.trychroma.com/)

* **The Problem:** Tracking user clickstreams and running LLMs synchronously on every interaction causes severe frontend lag, DDOSes backend servers, and burns thousands of unnecessary API tokens on administrative browsing.
* **Non-Blocking Telemetry:** Engineered a custom client-side event bus (`tracker.js`) with 5-second queue flushing and an asynchronous background evaluation engine using **APScheduler**, eliminating live-session UI latency while cutting API churn by **80%**.
* **Asynchronous LangGraph Graph:** Built a 3-node state machine (`analyze_behavior` → `retrieve_products` → `generate_copy`) deducing technical career trajectory from clickstream telemetry to query **ChromaDB**.
* **Dual-Store Synchronization:** Built an atomic dual-write transactional service layer across **SQLite** and **ChromaDB**, ensuring 100% relational-vector consistency across catalog mutations at sub-100ms sync speeds.
* **Production Guardrails:** Role-Based Access Control (RBAC) interceptors eliminate redundant token expenditure on administrative requests, combined with an automated Cold-Start discovery fallback.

---

## 🧪 Shipped Systems & Engineering Portfolio

| System | Architecture & Focus | Tech Stack | Status |
| :--- | :--- | :--- | :---: |
| **[Hotel GM Intelligence Copilot 3.0](https://github.com/SESHANKCH7171/HOTEL_GM_SYSTEM_3.0)** | Real-time WebRTC Voice Copilot + LangGraph operational anomaly engine for Hotel GMs | `LiveKit` `Groq LPUs` `Whisper V3` `LangGraph` `Deepgram` `Streamlit` | ✅ Live Demo |
| **[Enterprise Agentic RAG Platform](https://github.com/SESHANKCH7171/enterprise-rag-with-gcp)** | Enterprise RAG over 4,000+ docs with NeMo Guardrails, Portkey Gateway, and RAGAS evals | `Qdrant HNSW` `NeMo Colang` `FlashRank` `Portkey` `Logfire` `Cloud Run` | ✅ Deployed |
| **[SmartReco.ai Engine](https://github.com/SESHANKCH7171/smartreco-ai-engine)** | Event-driven proactive recommendation agent with async background workers & dual-store sync | `FastAPI` `LangGraph` `APScheduler` `ChromaDB` `SQLite` `Vanilla JS` | ✅ Shipped |
| **[Universal LLM Terminal Bridge](https://github.com/SESHANKCH7171/universal-llm-terminal-bridge)** | High-throughput transparent proxy server translating Anthropic API protocols to LiteLLM for Claude Code CLI | `Python` `LiteLLM` `Vertex AI` `Gemini 2.5` `SSE Streaming` `Docker` | ✅ Shipped |
| **[HR Analytics Intelligence](https://github.com/SESHANKCH7171/Business-Analytics-Portfolio)** | Multimodal resume screening engine automating JD gap analysis and candidate scoring across 500+ PDFs | `Gemini 2.5 Flash` `Multimodal Vision` `FastAPI` `Streamlit` `Pydantic` | ✅ Shipped |
| **[VoiceScribe](https://github.com/SESHANKCH7171/Voicescribe)** | Local, zero-latency audio dictation alternative to Wispr Flow streaming to Groq Whisper Large V3 | `Python` `Streamlit` `Groq Whisper V3` `Web Audio` `Speech-to-Text` | ✅ Open Source |

---

## 🚨 What I've Broken & What I Learned (POST-MORTEMS)

> *"The only way to build reliable agentic software is to break things under real constraints. Here are real post-mortems from my projects:"*

| Project | What Broke (The Bug) | Root Cause | The Post-Mortem (How I Fixed It) |
| :--- | :--- | :--- | :--- |
| **Universal LLM Terminal Bridge** | Anthropic CLI rejected streaming responses midway through large codebases with JSON decode errors. | SSE (Server-Sent Events) chunking protocol mismatch between Anthropic's expected event format and LiteLLM's raw stream chunks. | Rewrote the SSE event translator to buffer chunks and parse raw bytes before re-emitting standardized Anthropic event frames. Added test suites handling 500k+ token payloads. |
| **SmartReco.ai** | `APScheduler` background worker crashed with `sqlite3.OperationalError: database is locked` during concurrent browser browsing. | SQLite default rollback journal blocks concurrent writes between FastAPI request threads and async background workers. | Enabled SQLite Write-Ahead Logging (`PRAGMA journal_mode=WAL`), configured a 15-second busy timeout, and wrapped writes in an atomic transactional service layer with exponential backoff. |
| **Hotel GM Voice Copilot** | Voice interaction latency spiked to >6 seconds during multi-turn conversations, causing awkward pauses and audio lag. | The system waited for the entire LLM response to complete generation before sending text to the Text-to-Speech (TTS) engine. | Switched to streaming TTS via Deepgram Aura-2 over WebRTC data tracks. As soon as the LLM emits the first 3 tokens, audio synthesis begins immediately, cutting perceived turnaround to <1s. |
| **Enterprise Stripe RAG** | Ingestion of 4,000+ technical pages caused retrieval context dilution ("lost-in-the-middle") and high P95 prompt token costs. | Naive dense vector search retrieved top-20 chunks containing redundant boilerplate and navigation headers from parsed HTML. | Engineered a Two-Stage Retrieval Funnel: Qdrant HNSW retrieves top-25 candidate chunks, followed by a local **FlashRank (TinyBERT)** cross-encoder reranking to top-5, slashing prompt tokens by **65%** and boosting Context Precision to **0.93**. |

---

## 📈 Quantitative System Telemetry

| Engineering Metric | Measured Value | Architectural Layer |
| :--- | :---: | :--- |
| **Voice Time-to-First-Token (TTFT)** | **891 ms** | Groq LPU + Silero VAD + LiveKit WebRTC |
| **End-to-End Voice Turnaround** | **3.0 s** | Full Turn: Acoustic Ingestion ➔ LangGraph ➔ Deepgram TTS |
| **RAG Context Precision** | **0.93** | Two-Stage Funnel: Qdrant HNSW + FlashRank Cross-Encoder |
| **Prompt Token Payload Reduction** | **65%** | TinyBERT Cross-Encoder Reranking & Context Pruning |
| **Attack Interception Recall** | **100% (Test Set)** | Upstream NeMo Guardrails with Colang policies |
| **Agent Tool Correctness** | **1.00** | Autonomous LangGraph State Machine with TypedDict schema |
| **Docker Container Footprint** | **85% reduction** | Dual-manifest build for Google Cloud Run (3.5 GB → 520 MB) |
| **Frontend Telemetry Ingestion Overhead** | **0 ms** | APScheduler background worker + client-side queue flush |

---

## 📁 System Design & Architecture Artifacts

- 📐 **State Machine Graphs:** Explicit TypedDict cyclic topologies for LangGraph nodes (`analyze`, `retrieve`, `route`, `execute`, `verify`).
- 🛡️ **Colang Security Policies:** Multi-rail guardrails for jailbreak neutralization, sensitive credential masking, and topic adherence.
- 📊 **Golden Evaluation Datasets:** 15-scenario RAG and 6-scenario red-team attack benchmarks evaluated with RAGAS metrics.
- ⚡ **Telemetry Logs:** Pydantic Logfire distributed spans and LangSmith execution run trees tracking latency, token usage, and P95 overhead.

---

## 🎓 Background & Education

- 🏛️ **IIT Madras** — Dual Degree (B.Tech + M.Tech), Aerospace Engineering (2018 – 2023)
- 🎯 **Minor Degree** — Personality and Professional Development, IIT Madras
- 🔬 **Engineering Foundation:** Strong analytical background in computational mathematics, fluid dynamics, state-space systems modeling, and high-performance computing, now applied to autonomous agent architectures and latency optimization.

---

## 📬 Connect with Me

- 💼 **LinkedIn:** [linkedin.com/in/seshankch](https://linkedin.com/in/seshankch)
- 🐙 **GitHub:** [github.com/seshankch7171](https://github.com/seshankch7171)
- ✉️ **Email:** [seshankch7171@gmail.com](mailto:seshankch7171@gmail.com)
