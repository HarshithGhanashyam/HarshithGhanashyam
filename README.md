<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:161b22&height=220&section=header&text=Harshith%20Ghanashyam&fontSize=44&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Software%20Engineer%20%7C%20Systems%20%7C%20AI%20Engineering&descAlignY=58&descSize=17" width="100%"/>

<br/>

### Building reliable systems where **software architecture meets intelligence.**

Backend systems · AI pipelines · Agents · RAG · Computer Vision

<br/>

<a href="mailto:harshithghanashyam@gmail.com">
<img src="https://img.shields.io/badge/EMAIL-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>
&nbsp;
<a href="https://github.com/HarshithGhanashyam">
<img src="https://img.shields.io/badge/GITHUB-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=16&pause=1200&color=58A6FF&center=true&vCenter=true&width=720&lines=Designing+systems%2C+not+just+features.;Clean+Architecture+%C2%B7+RAG+%C2%B7+Agents+%C2%B7+Computer+Vision;Currently+building+MemOps+%E2%80%94+operational+memory+for+AI+systems." alt="Typing SVG"/>

</div>

---

# 01 / What I Build

I focus on the engineering layer behind intelligent software.

Not just models.
Not just APIs.
**Systems that are structured, testable, observable, and designed to evolve.**

My work sits at the intersection of:

```text
┌─────────────────────────────────────────────────────────────┐
│                    INTELLIGENT SYSTEMS                      │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   Backend        AI / ML         Agents        Computer      │
│   Systems        Pipelines       & RAG         Vision       │
│                                                             │
│   APIs           Retrieval       Planning      Detection    │
│   Databases      Embeddings      Tools         Tracking     │
│   Architecture   Evaluation      Memory        Inference    │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Engineering principles

**Architecture over abstraction**
Use structure when it solves a real problem, not because a pattern exists.

**Determinism where possible**
Critical behavior should be reproducible and auditable.

**Evidence over assumptions**
Systems should expose why they produced a result.

**Simple cores, replaceable intelligence**
AI components should be replaceable without rewriting the system around them.

---

# 02 / Flagship

<div align="center">

## 🧠 MemOps

### Operational memory infrastructure for AI & production systems

**The problem**

Operational knowledge is everywhere:

```text
Incidents ──┐
Root Causes ├──► scattered across tools
Runbooks ───┤
Decisions ──┘
```

Over time it becomes:

```text
Scattered → duplicated → outdated → contradictory → difficult to retrieve
```

MemOps treats this knowledge as **versioned operational memory** rather than disposable documentation.

</div>

---

### What MemOps does

```text
                 ┌──────────────────────┐
                 │      Applications    │
                 │      AI Agents       │
                 │      CLI / Users     │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │       MemOps API     │
                 └──────────┬───────────┘
                            │
          ┌─────────────────┼─────────────────┐
          ▼                 ▼                 ▼
      Retrieval          Lifecycle        Diagnosis
          │                 │                 │
          ▼                 ▼                 ▼
   Hybrid Ranking      Memory State       Deterministic
   Vector + Lexical    & Versioning       Reasoning
          │                 │                 │
          └─────────────────┼─────────────────┘
                            ▼
                 ┌──────────────────────┐
                 │ PostgreSQL +         │
                 │ pgvector             │
                 └──────────────────────┘
```

### Core engineering

| System            | Design                                                     |
| ----------------- | ---------------------------------------------------------- |
| **Retrieval**     | Hybrid ranking using vector similarity + lexical matching  |
| **Confidence**    | Confidence decay over time                                 |
| **Context**       | Environment fingerprinting                                 |
| **Lifecycle**     | Explicit memory state transitions                          |
| **Diagnosis**     | Deterministic and LLM-independent                          |
| **Security**      | Scoped API-key RBAC                                        |
| **Reliability**   | Sliding-window rate limiting                               |
| **Observability** | OpenTelemetry                                              |
| **Verification**  | Unit + integration + E2E tests                             |
| **Architecture**  | Domain → Application → Infrastructure → Interface → Agents |

### Memory lifecycle

```text
                    ┌───────────┐
                    │ PROPOSED  │
                    └─────┬─────┘
                          │
                          ▼
                    ┌───────────┐
                    │ CONFIRMED │
                    └─────┬─────┘
                          │
              ┌───────────┼───────────┐
              ▼           ▼           ▼
        SUPERSEDED   CONTRADICTED   ARCHIVED
```

### Retrieval signals

MemOps doesn't rely on vector similarity alone.

```text
Retrieval Score
      │
      ├── Vector similarity
      ├── Lexical relevance
      ├── Confidence decay
      ├── Environment fingerprint
      └── Lifecycle state
```

**Five signals → one ranked operational-memory result.**

<div align="center">

### Stack

`FastAPI` · `PostgreSQL` · `pgvector` · `SQLAlchemy` · `OpenTelemetry` · `Poetry` · `Docker`

<br/>

<a href="https://github.com/HarshithGhanashyam/aioops">
<img src="https://img.shields.io/badge/VIEW%20MEMOPS%20REPOSITORY-58A6FF?style=for-the-badge&logo=github&logoColor=white"/>
</a>

</div>

---

# 03 / Selected Engineering Work

<table>
<tr>
<td width="50%" valign="top">

## 🔬 Autonomous Research Agent

A ReAct-style research system coordinating multiple tools through an explicit reasoning loop.

```text
Thought
   ↓
Action
   ↓
Observation
   ↓
Next Action
```

**Engineering focus**

* Deterministic core planning
* 5 coordinated tools
* LLM-optional architecture
* Zero API keys required

`Python` `FastAPI` `ReAct`

<br/>

<a href="https://github.com/HarshithGhanashyam/05-agentic-research-agent">→ Repository</a>

</td>

<td width="50%" valign="top">

## 🎯 Q-Learning Agent

A reinforcement-learning implementation built from the fundamentals rather than hiding the algorithm behind an RL framework.

**Engineering focus**

* Tabular Q-learning
* Pure NumPy implementation
* GridWorld environment
* Reward convergence analysis

```text
Untrained
≈ -125 reward

        ↓

Training

        ↓

Near-optimal policy
```

`Python` `NumPy` `Streamlit`

<br/>

<a href="https://github.com/HarshithGhanashyam/08-rl-learning-agent">→ Repository</a>

</td>
</tr>

<tr>
<td width="50%" valign="top">

## 👁️ Real-Time Visual Intelligence

A live-video intelligence pipeline combining detection, recognition, tracking, and searchable incident logging.

```text
Camera
  ↓
Detection
  ↓
Recognition
  ↓
Tracking
  ↓
Incident Log
```

**Stack**

`YOLO` `InsightFace` `OpenCV` `FastAPI`

<br/>

<a href="https://github.com/HarshithGhanashyam/surveillance-project">→ Repository</a>

</td>

<td width="50%" valign="top">

## 📄 PDF RAG Chatbot

A local retrieval pipeline designed to produce answers grounded in the source document.

```text
PDF
 ↓
Chunking
 ↓
LSA Embeddings
 ↓
FAISS
 ↓
Re-ranking
 ↓
Cited Answer
```

**Stack**

`FAISS` `LSA` `pypdf` `Streamlit`

<br/>

<a href="https://github.com/HarshithGhanashyam/06-rag-pdf-chatbot">→ Repository</a>

</td>
</tr>
</table>

---

# 04 / Engineering Progression

My projects represent a progression from individual ML algorithms toward complete intelligent systems.

```text
01
Classical ML
     │
     ▼
02
CNN
     │
     ▼
03
GAN
     │
     ▼
04
LLM Integration
     │
     ▼
05
Agents
     │
     ▼
06
RAG
     │
     ▼
07
Computer Vision
     │
     ▼
08
Reinforcement Learning
     │
     ▼
09
Operational AI Systems
     │
     ▼
   MemOps
```

| #  | Project                | Focus                  |
| -- | ---------------------- | ---------------------- |
| 01 | Churn Dashboard        | Classical ML           |
| 02 | CNN Image Classifier   | Deep Learning          |
| 03 | GAN Digit Generator    | Generative Models      |
| 04 | LLM Summarizer / QA    | LLM Integration        |
| 05 | Research Agent         | Agents                 |
| 06 | PDF Chatbot            | RAG                    |
| 07 | OpenCV Detection Suite | Computer Vision        |
| 08 | RL Learning Agent      | Reinforcement Learning |
| 09 | MemOps                 | AI Infrastructure      |

<div align="center">

<a href="https://github.com/HarshithGhanashyam/01-churn-dashboard">01</a>
 ·  <a href="https://github.com/HarshithGhanashyam/02-cnn-image-classifier">02</a>
 ·  <a href="https://github.com/HarshithGhanashyam/03-gan-digit-generator">03</a>
 ·  <a href="https://github.com/HarshithGhanashyam/04-llm-summarizer-qa">04</a>
 ·  <a href="https://github.com/HarshithGhanashyam/05-agentic-research-agent">05</a>
 ·  <a href="https://github.com/HarshithGhanashyam/06-rag-pdf-chatbot">06</a>
 ·  <a href="https://github.com/HarshithGhanashyam/07-opencv-detection-suite">07</a>
 ·  <a href="https://github.com/HarshithGhanashyam/08-rl-learning-agent">08</a>

</div>

---

# 05 / Technical Stack

<div align="center">

### Languages

<img src="https://skillicons.dev/icons?i=py,ts,js,c,java" />

### Backend & Data

<img src="https://skillicons.dev/icons?i=fastapi,flask,postgres,sqlite,mysql" />

### AI / ML

<img src="https://skillicons.dev/icons?i=pytorch,sklearn,opencv" />

### Infrastructure & Tooling

<img src="https://skillicons.dev/icons?i=docker,git,github,vscode" />

</div>

<br/>

```text
Languages       Python · TypeScript · JavaScript · C · Java

Backend         FastAPI · Flask · REST APIs

Data            PostgreSQL · pgvector · SQLite · MySQL

AI / ML         PyTorch · scikit-learn · Computer Vision
                RAG · Agents · Reinforcement Learning

Infrastructure  Docker · OpenTelemetry · Git · GitHub

Architecture    Clean Architecture · Layered Systems
                Deterministic Components · Modular Design
```

---

# 06 / GitHub Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=HarshithGhanashyam&show_icons=true&theme=github_dark&hide_border=true&count_private=true&bg_color=0d1117&title_color=58A6FF&icon_color=58A6FF"/>

<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=HarshithGhanashyam&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58A6FF"/>

<br/><br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=HarshithGhanashyam&theme=github-dark-blue&hide_border=true&background=0D1117"/>

<br/><br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=HarshithGhanashyam&theme=github-compact&hide_border=true&bg_color=0D1117&color=58A6FF&line=58A6FF&point=FFFFFF" width="95%"/>

</div>

---

# 07 / Currently Building

<div align="center">

## MemOps

**Operational memory infrastructure for AI systems.**

```text
Store → Retrieve → Diagnose → Version → Verify
```

The goal isn't to build another chatbot.

The goal is to build the **memory infrastructure intelligent systems can depend on.**

</div>

---

<div align="center">

### Let's build systems that are understandable, testable, and useful.

<br/>

<a href="mailto:harshithghanashyam@gmail.com">
**harshithghanashyam@gmail.com**
</a>

  ·  

<a href="https://github.com/HarshithGhanashyam">
**github.com/HarshithGhanashyam**
</a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:161b22,100:0d1117&height=100&section=footer" width="100%"/>

</div>
