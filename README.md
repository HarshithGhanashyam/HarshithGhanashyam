# Harshith Ghanashyam

**Software engineer building systems at the intersection of clean architecture and intelligent behavior — backend infrastructure, ML pipelines, agents, and computer vision.**

[Email](mailto:harshithghanashyam@gmail.com) · [GitHub](https://github.com/HarshithGhanashyam)

---

### 01 / FLAGSHIP

## MemOps
**Operational memory infrastructure for AI and production systems.**

**The problem** — Operational knowledge (incident resolutions, root causes, config decisions) scatters across disconnected tools, decays over time, contradicts itself, and can't be retrieved reliably when it's needed most.

**The system** — A multi-tenant REST API + CLI for storing, versioning, retrieving, and diagnosing operational memories, with evidence and provenance attached to every entry.

**Engineering signals**
- **Hybrid ranking pipeline** — 5 weighted signals: vector similarity, lexical match, confidence decay, environment fingerprint, lifecycle state
- **Memory lifecycle** — PROPOSED → CONFIRMED → SUPERSEDED → CONTRADICTED → ARCHIVED, with contradiction detection between conflicting memories
- **Deterministic diagnosis engine** — no LLM dependency, fully auditable reasoning
- **Clean Architecture** — Domain → Application → Infrastructure → Interface → Agents
- **Access control & reliability** — scoped API-key RBAC, sliding-window rate limiting, request telemetry via OpenTelemetry
- **Verified with CI** — unit, integration, and e2e test suites

**Stack:** FastAPI · PostgreSQL · pgvector · SQLAlchemy · OpenTelemetry · Poetry · Docker

**[→ View Repository](https://github.com/HarshithGhanashyam/aioops)**

---

### 02 / FEATURED WORK

**[Autonomous Research Agent](https://github.com/HarshithGhanashyam/05-agentic-research-agent)**
A ReAct-style agent (Thought → Action → Observation) coordinating five tools — calculator, Wikipedia, web search, URL fetch, notepad. Core planning logic is deterministic and requires zero API keys, with a real LLM swappable in as a single function change.
`FastAPI · Python · ReAct architecture`

**[Q-Learning Agent from Scratch](https://github.com/HarshithGhanashyam/08-rl-learning-agent)**
Tabular Q-learning implemented without an RL library — pure NumPy and dictionaries — trained on GridWorld and Tic-Tac-Toe with ε-greedy exploration. GridWorld episode reward improved from ≈−125 (untrained) to near-optimal.
`Python · NumPy · Streamlit`

**[Real-Time Visual Intelligence System](https://github.com/HarshithGhanashyam/surveillance-project)**
A live-video pipeline combining face recognition, YOLO object detection, and person tracking, with a searchable incident log built on top.
`Python · YOLO · InsightFace · OpenCV · FastAPI · SQLite`

**[PDF Document Chatbot](https://github.com/HarshithGhanashyam/06-rag-pdf-chatbot)**
A fully local retrieval pipeline: PDF extraction → chunking → LSA embeddings → FAISS indexing → sentence re-ranking → extractive answers with page-level citations. No API keys required.
`Python · FAISS · TF-IDF/SVD (LSA) · pypdf · Streamlit`

**[Customer Churn Dashboard](https://github.com/HarshithGhanashyam/01-churn-dashboard)**
A synthetic telecom dataset generator paired with three classifiers (LR / RF / GBM, auto-selected by ROC-AUC) and a Streamlit dashboard for single predictions, batch CSV upload, and model comparison.
`Python · scikit-learn · pandas · Streamlit`

---

### 03 / AI ENGINEERING PROGRESSION

A sequence of projects moving through the ML/AI stack, each one built to demonstrate a different layer of the field:

```
01  Classical ML         → Churn Prediction Dashboard
02  CNN                  → Image Classifier
03  GAN                  → Digit Generator
04  LLM Integration      → Summarizer & QA
05  Agents               → Agentic Research Agent
06  RAG                  → PDF Chatbot
07  Computer Vision       → OpenCV Detection Suite
08  Reinforcement Learning → Q-Learning Agent
```

[01](https://github.com/HarshithGhanashyam/01-churn-dashboard) · [02](https://github.com/HarshithGhanashyam/02-cnn-image-classifier) · [03](https://github.com/HarshithGhanashyam/03-gan-digit-generator) · [04](https://github.com/HarshithGhanashyam/04-llm-summarizer-qa) · [05](https://github.com/HarshithGhanashyam/05-agentic-research-agent) · [06](https://github.com/HarshithGhanashyam/06-rag-pdf-chatbot) · [07](https://github.com/HarshithGhanashyam/07-opencv-detection-suite) · [08](https://github.com/HarshithGhanashyam/08-rl-learning-agent)

---

### 04 / ENGINEERING PROOF

**System design** — Clean Architecture with strict domain separation, multi-tenancy, event sourcing (MemOps)

**Intelligent systems** — Retrieval-augmented generation, agent orchestration with tool use, hybrid semantic+lexical retrieval, reinforcement learning from scratch

**Software engineering practice** — API design, RBAC and rate limiting, OpenTelemetry instrumentation, Docker-based deployment, CI pipelines with unit/integration/e2e coverage

---

### 05 / STACK

```
Python · TypeScript
FastAPI · Streamlit · Flask
PostgreSQL · SQLite · pgvector
PyTorch · scikit-learn · OpenCV · FAISS · NumPy
Docker · Docker Compose · Alembic · Poetry
```

---

### Contact

**[harshithghanashyam@gmail.com](mailto:harshithghanashyam@gmail.com)** · **[github.com/HarshithGhanashyam](https://github.com/HarshithGhanashyam)**
