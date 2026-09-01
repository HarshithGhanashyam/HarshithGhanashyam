<h1 align="center">Harshith Ghanashyam</h1>

<p align="center">
  <strong>Software Developer · AI/ML Engineering · Clean Architecture</strong>
</p>

<p align="center">
  <a href="mailto:harshithghanashyam@gmail.com">
    <img src="https://img.shields.io/badge/Email-harshithghanashyam@gmail.com-EA4335?style=flat&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  &nbsp;
  <a href="https://github.com/HarshithGhanashyam">
    <img src="https://img.shields.io/badge/GitHub-HarshithGhanashyam-181717?style=flat&logo=github&logoColor=white" alt="GitHub"/>
  </a>
</p>

---

## About

I build software systems — from production APIs with clean architecture to ML pipelines, computer vision, and reinforcement learning agents.

My focus is on **engineering that works**: readable code, proper separation of concerns, testable components, and systems that degrade gracefully.

---

## What I Build

| Area | What I've built |
|------|----------------|
| **Backend Systems** | Multi-tenant FastAPI services, clean architecture, event sourcing, RBAC |
| **AI/ML Systems** | RAG pipelines, ReAct agents, Q-learning from scratch, GAN training |
| **Computer Vision** | Real-time face/object detection, YOLO tracking, surveillance systems |
| **Data / ML** | Churn prediction dashboards, CNN classifiers, hybrid retrieval pipelines |

---

## Technical Stack

**Languages**: Python · TypeScript  
**Frameworks**: FastAPI · Streamlit · Flask  
**Databases**: PostgreSQL · SQLite · pgvector (vector search)  
**ML/AI**: scikit-learn · PyTorch · OpenCV · FAISS · NumPy  
**Infrastructure**: Docker · Docker Compose · Alembic · Poetry  
**Practices**: Clean Architecture · Domain-Driven Design · TDD · Event Sourcing

---

## Flagship Project

### [MemOps — Operational Memory Management System](https://github.com/HarshithGhanashyam/aioops)

[![CI Status](https://github.com/HarshithGhanashyam/aioops/actions/workflows/ci.yml/badge.svg)](https://github.com/HarshithGhanashyam/aioops/actions)

> A production-grade Python service for structured **operational memory** storage, versioning, retrieval, and diagnosis — built for AI/LLM operational environments.

**Problem:** AI and production systems accumulate critical operational knowledge (incident resolutions, root causes, config decisions) across disconnected tools. This knowledge degrades, contradicts itself, and is impossible to retrieve reliably when needed.

**Solution:** A multi-tenant REST API + CLI that stores operational memories with full versioning, attaches evidence and provenance, runs hybrid semantic+lexical retrieval with confidence decay and environment drift detection, and detects contradictions between conflicting memories.

**Built with:** FastAPI · PostgreSQL · pgvector · SQLAlchemy · OpenTelemetry · Poetry · Docker  
**Architecture:** Clean Architecture (Domain → Application → Infrastructure → Interface → Agents)

**Key technical highlights:**
- 5-signal ranking pipeline: vector similarity (35%) + lexical (25%) + confidence decay (15%) + environment fingerprint (15%) + lifecycle state (10%)
- Multi-stage memory lifecycle: PROPOSED → CONFIRMED → SUPERSEDED → CONTRADICTED → ARCHIVED
- Deterministic diagnosis engine — no LLM dependency, fully auditable reasoning
- Scoped API-key RBAC + sliding-window rate limiting + request telemetry
- Comprehensive test suite: unit / integration / e2e

---

## Featured Projects

### [Autonomous Research Agent](https://github.com/HarshithGhanashyam/05-agentic-research-agent)
[![CI Status](https://github.com/HarshithGhanashyam/05-agentic-research-agent/actions/workflows/ci.yml/badge.svg)](https://github.com/HarshithGhanashyam/05-agentic-research-agent/actions)

ReAct-style agent (Thought → Action → Observation) with 5 tools — calculator, Wikipedia, web search, URL fetch, notepad. Core planning is deterministic, requiring **zero API keys**. Designed so swapping in a real LLM is a one-function change.

**Stack:** FastAPI · Python · ReAct architecture

---

### [Q-Learning Agent from Scratch](https://github.com/HarshithGhanashyam/08-rl-learning-agent)
[![CI Status](https://github.com/HarshithGhanashyam/08-rl-learning-agent/actions/workflows/ci.yml/badge.svg)](https://github.com/HarshithGhanashyam/08-rl-learning-agent/actions)

Tabular Q-learning implemented from scratch (no RL library — pure NumPy/dicts) on GridWorld and Tic-Tac-Toe, with ε-greedy exploration and Streamlit UI. GridWorld: episode reward improved from ≈−125 (untrained) to near-optimal.

**Stack:** Python · NumPy · Streamlit

---

### [Real-Time Visual Intelligence System](https://github.com/HarshithGhanashyam/surveillance-project)
Real-time surveillance system: face recognition, YOLO object detection, person tracking, and trace logging over live video streams. Built with FastAPI backend and a searchable incident log.

**Stack:** Python · YOLO · InsightFace · OpenCV · FastAPI · SQLite

---

### [PDF Document Chatbot (RAG)](https://github.com/HarshithGhanashyam/06-rag-pdf-chatbot)
End-to-end RAG pipeline: PDF extraction → chunking → LSA embeddings → FAISS indexing → sentence re-ranking → extractive answer with page citations. Runs entirely locally — no API keys.

**Stack:** Python · FAISS · TF-IDF/SVD (LSA) · pypdf · Streamlit

---

### [Customer Churn Dashboard](https://github.com/HarshithGhanashyam/01-churn-dashboard)
Synthetic telecom dataset generator + 3 trained classifiers (LR / RF / GBM, auto-selected by ROC-AUC) + Streamlit dashboard with single prediction, batch CSV upload, model comparison, and data exploration.

**Stack:** Python · scikit-learn · pandas · Streamlit

---

## AI Engineering Series

A progression through the ML/AI stack, building increasingly complex systems:

| # | Project | Focus |
|---|---------|-------|
| [01](https://github.com/HarshithGhanashyam/01-churn-dashboard) | Churn Prediction Dashboard | Classical ML, model comparison, Streamlit |
| [02](https://github.com/HarshithGhanashyam/02-cnn-image-classifier) | CNN Image Classifier | Deep learning, convolutional networks |
| [03](https://github.com/HarshithGhanashyam/03-gan-digit-generator) | GAN Digit Generator | Generative models, adversarial training |
| [04](https://github.com/HarshithGhanashyam/04-llm-summarizer-qa) | LLM Summarizer & QA | Language model integration |
| [05](https://github.com/HarshithGhanashyam/05-agentic-research-agent) | Agentic Research Agent | ReAct agents, tool use, planning |
| [06](https://github.com/HarshithGhanashyam/06-rag-pdf-chatbot) | RAG PDF Chatbot | Retrieval-augmented generation, FAISS |
| [07](https://github.com/HarshithGhanashyam/07-opencv-detection-suite) | OpenCV Detection Suite | Computer vision, real-time detection |
| [08](https://github.com/HarshithGhanashyam/08-rl-learning-agent) | RL Learning Agent | Reinforcement learning from scratch |

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=HarshithGhanashyam&show_icons=true&theme=dark&hide_border=true&count_private=true" alt="GitHub Stats" height="165"/>
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=HarshithGhanashyam&layout=compact&theme=dark&hide_border=true" alt="Top Languages" height="165"/>
</p>

---

<p align="center">
  <i>Always learning. Always building.</i>
</p>
