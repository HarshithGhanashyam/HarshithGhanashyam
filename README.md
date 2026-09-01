<div align="center">

HARSHITH GHANASHYAM

SOFTWARE ENGINEER · SYSTEMS · ARCHITECTURE · AI ENGINEERING

Building reliable software where architecture meets intelligence.

<br>




<br>

┌─────────────────────────────────────────────────────────────────────┐
│  harshith@engineering                                      ● ONLINE │
│                                                                     │
│  $ ./run --profile                                                   │
│  > backend systems                                                   │
│  > retrieval                                                         │
│  > agents                                                            │
│  > computer vision                                                   │
│  > intelligent infrastructure                                       │
│                                                                     │
│  CURRENT SYSTEM  ────────────────────────────────────────  MEMOPS   │
└─────────────────────────────────────────────────────────────────────┘

SYSTEMS / BACKEND / AGENTS / RAG / COMPUTER VISION / INFRASTRUCTURE

</div>

<div align="center">

01 / SYSTEM PROFILE    02 / MEMOPS    03 / SYSTEMS    04 / ARCHITECTURE    05 / STACK

</div>

01 / SYSTEM PROFILE

I build software systems with an emphasis on explicit architecture, deterministic behavior, retrieval, orchestration, and verification.

<table>
<tr>
<td width="25%" align="center">

BACKEND

APIs
Services
Data systems

</td>
<td width="25%" align="center">

INTELLIGENCE

Agents
RAG
ML systems

</td>
<td width="25%" align="center">

VISION

Detection
Tracking
Recognition

</td>
<td width="25%" align="center">

ENGINEERING

Architecture
Testing
Observability

</td>
</tr>
</table>

Engineering direction: moving from individual models and experiments toward complete, auditable systems.

02 / CURRENT SYSTEM

<div align="center">

MEMOPS

Operational memory infrastructure for AI and production systems.

</div>

Operational knowledge — incident resolutions, root causes, configuration decisions, and other operational context — tends to scatter across systems, become outdated, contradict itself, and become difficult to retrieve when it matters.

MemOps treats that knowledge as versioned, retrievable, evidence-backed operational memory.

System map

flowchart TB
    A["OPERATIONAL KNOWLEDGE<br/>Incidents · Root Causes · Decisions · Configuration"]
    B["MEMOPS API"]
    C["MEMORY ENGINE"]
    D["RETRIEVAL"]
    E["LIFECYCLE"]
    F["DIAGNOSIS"]
    G[("PostgreSQL<br/>+ pgvector")]

    A --> B --> C
    C --> D
    C --> E
    C --> F
    D --> G
    E --> G
    F --> G

    classDef main fill:#161b22,stroke:#58a6ff,color:#ffffff,stroke-width:1px;
    classDef data fill:#0d1117,stroke:#79c0ff,color:#ffffff,stroke-width:1px;

    class A,B,C,D,E,F main;
    class G data;

Retrieval engine

MemOps combines multiple signals rather than relying on a single similarity score:

flowchart LR
    V["VECTOR<br/>SIMILARITY"]
    L["LEXICAL<br/>MATCH"]
    C["CONFIDENCE<br/>DECAY"]
    E["ENVIRONMENT<br/>FINGERPRINT"]
    S["LIFECYCLE<br/>STATE"]

    V --> H["HYBRID<br/>RANKING"]
    L --> H
    C --> H
    E --> H
    S --> H

    H --> R["RELEVANT<br/>MEMORY"]

    classDef signal fill:#161b22,stroke:#30363d,color:#c9d1d9;
    classDef core fill:#0d1117,stroke:#58a6ff,color:#ffffff,stroke-width:2px;
    class V,L,C,E,S signal;
    class H,R core;

Memory lifecycle

stateDiagram-v2
    [*] --> PROPOSED
    PROPOSED --> CONFIRMED
    CONFIRMED --> SUPERSEDED
    CONFIRMED --> CONTRADICTED
    CONFIRMED --> ARCHIVED
    SUPERSEDED --> [*]
    CONTRADICTED --> [*]
    ARCHIVED --> [*]

Engineering signals

SIGNAL

IMPLEMENTATION

Retrieval

Vector similarity · lexical matching · confidence decay · environment context

Lifecycle

PROPOSED → CONFIRMED → SUPERSEDED / CONTRADICTED / ARCHIVED

Diagnosis

Deterministic diagnosis engine with no LLM dependency

Access

Scoped API-key RBAC

Reliability

Sliding-window rate limiting · unit / integration / e2e testing

Observability

OpenTelemetry

Architecture

Domain → Application → Infrastructure → Interface → Agents

<div align="center">

FastAPI · PostgreSQL · pgvector · SQLAlchemy · OpenTelemetry · Poetry · Docker

<br>

→ View MemOps Repository

</div>

03 / SELECTED SYSTEMS

Four projects that show the progression from algorithms and models to complete intelligent systems.

<table>
<tr>
<td width="50%" valign="top">

01 / AUTONOMOUS RESEARCH AGENT

ReAct-style research agent coordinating five tools.

flowchart LR
    I["INPUT"] --> P["REASON"]
    P --> T["TOOL"]
    T --> O["OBSERVATION"]
    O --> P
    P --> A["ANSWER"]

Python FastAPI ReAct

Engineering signal: deterministic core planning with LLM integration kept replaceable.

→ Repository

</td>

<td width="50%" valign="top">

02 / VISUAL INTELLIGENCE

Live-video pipeline for detection, recognition, tracking, and incident logging.

flowchart LR
    C["CAMERA"] --> D["YOLO<br/>DETECTION"]
    D --> T["TRACKING"]
    T --> R["RECOGNITION"]
    R --> L["INCIDENT<br/>LOG"]

YOLO InsightFace OpenCV FastAPI

Engineering signal: real-time vision pipeline with searchable incident output.

→ Repository

</td>
</tr>

<tr>
<td width="50%" valign="top">

03 / PDF RAG

Local retrieval pipeline producing cited extractive answers.

flowchart LR
    P["PDF"] --> C["CHUNK"]
    C --> E["LSA"]
    E --> F["FAISS"]
    F --> R["RERANK"]
    R --> A["CITED<br/>ANSWER"]

FAISS LSA pypdf Streamlit

Engineering signal: retrieval pipeline without requiring a hosted vector service.

→ Repository

</td>

<td width="50%" valign="top">

04 / Q-LEARNING AGENT

Tabular Q-learning implemented from scratch using NumPy.

flowchart LR
    S["STATE"] --> A["ACTION"]
    A --> R["REWARD"]
    R --> Q["Q UPDATE"]
    Q --> P["POLICY"]
    P --> S

Python NumPy Streamlit

Engineering signal: RL fundamentals implemented without an RL library.

→ Repository

</td>
</tr>
</table>

<details>
<summary><b>PROJECT ARCHIVE</b></summary>

<br>

#

System

Focus

Stack

01

Customer Churn Dashboard

Classification + analytics

scikit-learn pandas Streamlit

02

CNN Image Classifier

Deep learning

Python

03

GAN Digit Generator

Generative models

Python

04

LLM Summarizer / QA

LLM integration

Python

05

OpenCV Detection Suite

Computer vision

OpenCV

</details>

04 / ENGINEERING MODEL

From models to systems.

flowchart LR
    M["MODELS"] --> C["AI<br/>COMPONENTS"]
    C --> A["INTELLIGENT<br/>APPLICATIONS"]
    A --> G["AGENTS +<br/>RETRIEVAL"]
    G --> S["SYSTEMS"]
    S --> I["AI<br/>INFRASTRUCTURE"]

    X["MEMOPS"] -.-> I

    classDef normal fill:#161b22,stroke:#30363d,color:#c9d1d9;
    classDef focus fill:#0d1117,stroke:#58a6ff,color:#ffffff,stroke-width:2px;

    class M,C,A,G,S normal;
    class I,X focus;

The project sequence reflects a deliberate shift:

learning algorithms → integrating models → orchestrating tools → building retrieval systems → designing infrastructure.

Architecture principles

flowchart TB
    D["DOMAIN"]
    A["APPLICATION"]
    I["INFRASTRUCTURE"]
    F["INTERFACE"]
    G["AGENTS"]

    D --> A --> I --> F --> G

    classDef layer fill:#161b22,stroke:#30363d,color:#c9d1d9;
    classDef domain fill:#0d1117,stroke:#58a6ff,color:#ffffff,stroke-width:2px;

    class D domain;
    class A,I,F,G layer;

The goal is straightforward:

Core behavior should not become a hostage to frameworks, databases, models, or external services.

That means keeping domain behavior explicit, infrastructure replaceable, and interfaces thin.

05 / STACK

<div align="center">

LANGUAGES

Python TypeScript JavaScript C Java

BACKEND

FastAPI Flask REST

DATA

PostgreSQL pgvector SQLite MySQL

AI / ML

PyTorch scikit-learn NumPy

INTELLIGENT SYSTEMS

RAG Agents LLM Integration Reinforcement Learning

COMPUTER VISION

OpenCV YOLO InsightFace

INFRASTRUCTURE

Docker OpenTelemetry Poetry Git GitHub

</div>

06 / GITHUB ACTIVITY

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=HarshithGhanashyam&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=58A6FF" height="165">

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=HarshithGhanashyam&layout=compact&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=58A6FF" height="165">

<br><br>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=HarshithGhanashyam&theme=github-compact&hide_border=true&bg_color=0D1117&color=58A6FF&line=58A6FF&point=FFFFFF" width="95%">

</div>

<div align="center">

┌──────────────────────────────────────────────────────────────┐
│                                                              │
│  SYSTEM STATUS                                               │
│  ● BUILDING                                                  │
│                                                              │
│  CURRENT FOCUS                                               │
│  MEMOPS                                                       │
│                                                              │
│  CONTACT                                                      │
│  harshithghanashyam@gmail.com                                │
│                                                              │
└──────────────────────────────────────────────────────────────┘

HARSHITH GHANASHYAM

SYSTEMS · ARCHITECTURE · AI ENGINEERING

GitHub · Email

</div>
