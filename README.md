<div align="center">

<img src="./banner.svg" width="100%" alt="Harshith Ghanashyam — software engineer"/>

<br/>

<a href="mailto:harshithghanashyam@gmail.com"><img src="https://img.shields.io/badge/EMAIL-0d1117?style=for-the-badge&logo=gmail&logoColor=EA4335&labelColor=161b22" alt="Email"/></a>
&nbsp;
<a href="https://github.com/HarshithGhanashyam"><img src="https://img.shields.io/badge/GITHUB-0d1117?style=for-the-badge&logo=github&logoColor=ffffff&labelColor=161b22" alt="GitHub"/></a>

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=15&duration=2600&pause=900&color=58A6FF&center=true&vCenter=true&width=760&lines=Clean+Architecture+%C2%B7+Domain-Driven+Design+%C2%B7+Event+Sourcing;RAG+Pipelines+%C2%B7+ReAct+Agents+%C2%B7+Computer+Vision;Building+systems+that+remain+inspectable+after+the+demo" alt="Engineering focus"/>

</div>

---

<div align="center">

`SYSTEMS`　·　`MEMOPS`　·　`PROJECTS`　·　`ARCHITECTURE`　·　`STACK`　·　`ACTIVITY`

</div>

---

# `01` / SYSTEM PROFILE

<table width="100%">
<tr>
<td width="25%" align="center" valign="top">

### BACKEND

**APIs**  
**Services**  
**Data systems**

</td>
<td width="25%" align="center" valign="top">

### ARCHITECTURE

**Boundaries**  
**Dependencies**  
**Verification**

</td>
<td width="25%" align="center" valign="top">

### INTELLIGENCE

**RAG**  
**Agents**  
**RL**

</td>
<td width="25%" align="center" valign="top">

### VISION

**Detection**  
**Tracking**  
**Recognition**

</td>
</tr>
</table>

<div align="center">

> **The direction is deliberate: move from isolated models toward complete, auditable systems.**

</div>

---

# `02` / FLAGSHIP — MEMOPS

<div align="center">

## MEMOPS

### Operational memory infrastructure for AI and production systems.

<a href="https://github.com/HarshithGhanashyam/aioops"><img src="https://img.shields.io/badge/%E2%86%92%20VIEW%20REPOSITORY-58A6FF?style=for-the-badge&labelColor=0d1117&color=58A6FF" alt="View MemOps repository"/></a>

</div>

<br/>

<table width="100%">
<tr>
<td width="50%" valign="top">

### THE PROBLEM

Operational knowledge — incident resolutions, root causes, configuration decisions — scatters across tools, decays, contradicts itself, and becomes unreliable when it is needed.

### THE SYSTEM

A **multi-tenant REST API + CLI** for storing, versioning, retrieving, and diagnosing operational memories, with evidence and provenance attached to entries.

</td>
<td width="50%" valign="top">

### SYSTEM PIPELINE

```text
┌───────────────────────────────┐
│ INCIDENTS · FIXES · DECISIONS │
└───────────────┬───────────────┘
                ▼
        ┌───────────────┐
        │   MEMOPS API  │
        └───────┬───────┘
                ▼
        ┌───────────────┐
        │ MEMORY ENGINE │
        └───────┬───────┘
          ┌──────┼──────┐
          ▼      ▼      ▼
      RETRIEVE  STATE  DIAGNOSE
          └──────┼──────┘
                 ▼
       PostgreSQL + pgvector
```

</td>
</tr>
</table>

### `HYBRID RETRIEVAL`

<div align="center">

| VECTOR | LEXICAL | DECAY | ENVIRONMENT | LIFECYCLE |
|:---:|:---:|:---:|:---:|:---:|
| similarity | match | confidence | fingerprint | state |
| `01` | `02` | `03` | `04` | `05` |

**5 signals → hybrid ranking → relevant operational memory**

</div>

### `MEMORY LIFECYCLE`

<div align="center">

```text
PROPOSED
   │
   ▼
CONFIRMED
   │
   ├──────────────► SUPERSEDED
   │
   ├──────────────► CONTRADICTED
   │
   └──────────────► ARCHIVED
```

</div>

<table width="100%">
<tr>
<td width="25%" valign="top"><b>DIAGNOSIS</b><br/>Deterministic<br/>Zero LLM dependency<br/>Fully auditable</td>
<td width="25%" valign="top"><b>ACCESS</b><br/>Scoped API keys<br/>RBAC<br/>Rate limiting</td>
<td width="25%" valign="top"><b>VERIFICATION</b><br/>Unit tests<br/>Integration tests<br/>E2E tests · CI-gated</td>
<td width="25%" valign="top"><b>OBSERVABILITY</b><br/>OpenTelemetry<br/>Evidence<br/>Provenance</td>
</tr>
</table>

<div align="center">

`FastAPI` `PostgreSQL` `pgvector` `SQLAlchemy` `OpenTelemetry` `Poetry` `Docker`

</div>

---

# `03` / SELECTED SYSTEMS

<table width="100%">
<tr>
<td width="50%" valign="top">

### `01` / AUTONOMOUS RESEARCH AGENT

**ReAct-style research agent coordinating five tools.**

```text
INPUT
  ↓
REASON ←──────────────┐
  ↓                   │
TOOL → OBSERVATION ───┘
  ↓
ANSWER
```

Deterministic core planning. Zero API keys. LLM swap-in is isolated to one function.

`FastAPI` `Python` `ReAct`

<a href="https://github.com/HarshithGhanashyam/05-agentic-research-agent">→ repository</a>

</td>
<td width="50%" valign="top">

### `02` / VISUAL INTELLIGENCE

**Real-time video pipeline.**

```text
CAMERA
  ↓
YOLO DETECTION
  ↓
PERSON TRACKING
  ↓
FACE RECOGNITION
  ↓
INCIDENT LOG
```

Turns live video into searchable incidents.

`YOLO` `InsightFace` `OpenCV` `FastAPI`

<a href="https://github.com/HarshithGhanashyam/surveillance-project">→ repository</a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### `03` / PDF RAG

**Local retrieval pipeline with cited answers.**

```text
PDF → CHUNK → LSA → FAISS → RERANK → CITED ANSWER
```

No hosted vector database required.

`FAISS` `LSA` `pypdf` `Streamlit`

<a href="https://github.com/HarshithGhanashyam/06-rag-pdf-chatbot">→ repository</a>

</td>
<td width="50%" valign="top">

### `04` / Q-LEARNING

**Tabular Q-learning from scratch.**

```text
STATE → ACTION → REWARD → Q UPDATE → POLICY
  ↑                                      │
  └──────────────────────────────────────┘
```

Implemented without an RL library using NumPy.

`Python` `NumPy` `Streamlit`

<a href="https://github.com/HarshithGhanashyam/08-rl-learning-agent">→ repository</a>

</td>
</tr>
</table>

### PROJECT ARCHIVE

| # | SYSTEM | FOCUS | REPOSITORY |
|---:|---|---|---|
| `01` | **Customer Churn Dashboard** | Classification + analytics | [→ repo](https://github.com/HarshithGhanashyam/01-churn-dashboard) |
| `02` | **CNN Image Classifier** | Deep learning | [→ repo](https://github.com/HarshithGhanashyam/02-cnn-image-classifier) |
| `03` | **GAN Digit Generator** | Generative models | [→ repo](https://github.com/HarshithGhanashyam/03-gan-digit-generator) |
| `04` | **LLM Summarizer / QA** | LLM integration | [→ repo](https://github.com/HarshithGhanashyam/04-llm-summarizer-qa) |
| `07` | **OpenCV Detection Suite** | Computer vision | [→ repo](https://github.com/HarshithGhanashyam/07-opencv-detection-suite) |

---

# `04` / ENGINEERING MODEL

<div align="center">

### FROM MODELS → TO SYSTEMS → TO INFRASTRUCTURE

```text
┌────────────┐
│   MODELS   │
└─────┬──────┘
      ↓
┌────────────┐
│ AI         │
│ COMPONENTS │
└─────┬──────┘
      ↓
┌────────────┐
│INTELLIGENT │
│APPLICATIONS│
└─────┬──────┘
      ↓
┌────────────┐
│ AGENTS +   │
│ RETRIEVAL  │
└─────┬──────┘
      ↓
┌────────────┐
│  SYSTEMS   │
└─────┬──────┘
      ↓
┌────────────────┐
│ AI INFRASTRUCTURE │
└───────┬────────┘
        ↓
      MEMOPS
```

</div>

### ARCHITECTURE PRINCIPLE

<div align="center">

```text
DOMAIN → APPLICATION → INFRASTRUCTURE → INTERFACE → AGENTS
  │
  └─────────────── dependencies stay controlled ────────────────┘
```

</div>

> **Core behavior should not become a hostage to frameworks, databases, models, or external APIs.**

---

# `05` / TECHNOLOGY

<div align="center">

<table width="90%">
<tr><td><b>LANGUAGES</b></td><td>Python · TypeScript · JavaScript · C · Java</td></tr>
<tr><td><b>BACKEND</b></td><td>FastAPI · Flask · REST</td></tr>
<tr><td><b>DATA</b></td><td>PostgreSQL · pgvector · SQLite · MySQL</td></tr>
<tr><td><b>AI / ML</b></td><td>PyTorch · scikit-learn · NumPy</td></tr>
<tr><td><b>INTELLIGENT SYSTEMS</b></td><td>RAG · Agents · LLM Integration · Reinforcement Learning</td></tr>
<tr><td><b>VISION</b></td><td>OpenCV · YOLO · InsightFace</td></tr>
<tr><td><b>INFRASTRUCTURE</b></td><td>Docker · OpenTelemetry · Poetry · Git · GitHub</td></tr>
</table>

<br/>

<img src="https://skillicons.dev/icons?i=py,ts,fastapi,flask,postgres,sqlite,docker,pytorch,sklearn,opencv,git,github&theme=dark&perline=6" alt="Technology stack"/>

</div>

---

# `06` / ACTIVITY

<div align="center">

<!-- Generated by metrics.yml -->
<img src="./metrics.svg" width="100%" alt="GitHub metrics dashboard"/>

<br/>

<img src="https://github-readme-stats.vercel.app/api?username=HarshithGhanashyam&show_icons=true&theme=github_dark&hide_border=true&count_private=true&bg_color=0d1117&title_color=58a6ff&icon_color=a371f7&text_color=c9d1d9" height="165" alt="GitHub statistics"/>
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=HarshithGhanashyam&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9" height="165" alt="Top languages"/>

<br/><br/>

<!-- Generated by snake.yml -->
<img src="https://raw.githubusercontent.com/HarshithGhanashyam/HarshithGhanashyam/output/snake-dark.svg" width="100%" alt="GitHub contribution snake"/>

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:161b22,100:0d1117&height=100&section=footer" width="100%" alt=""/>

### SYSTEM STATUS

`● BUILDING`

**CURRENT FOCUS — MEMOPS**

Operational memory infrastructure for AI systems.

<br/>

<a href="mailto:harshithghanashyam@gmail.com">harshithghanashyam@gmail.com</a>
&nbsp; · &nbsp;
<a href="https://github.com/HarshithGhanashyam">github.com/HarshithGhanashyam</a>

<br/><br/>

`SYSTEMS` · `ARCHITECTURE` · `AI ENGINEERING`

</div>
