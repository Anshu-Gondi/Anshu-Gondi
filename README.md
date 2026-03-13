# 👋 Hi, I’m Anshu Gondi

**Backend & Systems-Focused Developer building performance-aware software under real-world constraints.**

🎓 B.Tech (1st Year) — India
💻 Interested in **systems engineering, financial software, and high-performance backend infrastructure**

Open to **internships, backend roles, and technical collaborations.**

---

# About Me

I design backend systems that prioritize **correctness, performance, and measurable system behavior**, especially in **CPU-constrained environments**.

Working on low-resource hardware pushed me to treat system performance as an **engineering problem that must be measured**, not assumed.

My development workflow emphasizes:

* **Profiling before optimization**
* **Clear boundaries between deterministic logic and ML subsystems**
* **Introducing Rust or C++ only when benchmarks justify it**

Core workflow:

```
Build → Measure → Refactor → Re-measure
```

My long-term goal is to build **reliable financial and analytical software platforms used at scale.**

---

# Core Engineering Focus

**Backend Systems**

* Performance-aware backend architectures
* Explicit correctness and safety boundaries
* Latency-focused design in constrained environments

**Systems Performance**

* Rust and C++ acceleration through FFI
* Profiling-driven optimization
* Quantifying complexity vs measurable performance gains

**Financial Software**

* Transaction analytics pipelines
* Deterministic financial computation systems
* Reliable data processing infrastructure

**Machine Learning Integration**

* ML treated strictly as a **bounded subsystem**
* Deterministic business logic retains final authority

---

# Technical Stack

**Languages**

Python · Rust · C++ · C · TypeScript · SQL

**Backend**

FastAPI · Django · Axum (Rust) · Actix Web · Node.js / Express

**Databases**

PostgreSQL · MySQL · MongoDB · MinIO

**Machine Learning**

PyTorch · scikit-learn · NumPy · Pandas · ONNX Runtime

**Systems / Interoperability**

PyO3 · CXX · bindgen · OpenCV-rs · hnsw_rs

**Infrastructure**

Docker · Linux · Git · CI/CD · Render · Railway · GCP

---

# Flagship Project

## 🏫 CampusVision

**Real-Time Face-Based Attendance Infrastructure (In Development)**

CampusVision is designed as a **reliable classroom attendance system operating on CPU-only hardware**.

The system combines **computer vision, high-performance backend infrastructure, and scalable identity search** to automate classroom attendance while remaining deployable on low-cost hardware.

### Architecture

Detection & Recognition

* Face detection using YuNet
* Embedding generation using ArcFace

Performance Layer

* Rust-based embedding processing
* HNSW approximate nearest-neighbor search using
  Hierarchical Navigable Small World

Backend

* Axum (Rust) ingestion APIs
* Django authentication and orchestration
* MinIO object storage

Client Interfaces

* React web dashboard
* React Native mobile client

### Deployment Strategy

* Primary recognition via **webcam / mobile camera**
* CCTV used for **verification and audit trail**
* Location-aware indexing for scalable identity search

### Benchmark Environment

All performance benchmarks run on the same baseline hardware:

```
Intel Celeron N4020
2 cores / 2 threads
8GB RAM
CPU-only inference
```

### Sample Benchmarks

| Operation                | Rust  | Python |
| ------------------------ | ----- | ------ |
| Embedding inference      | 12 ms | 35 ms  |
| HNSW search (1000 faces) | 18 ms | 50 ms  |

### Current Focus

* Multi-frame recognition validation
* Location-based face index architecture
* Real-classroom pilot deployment

---

# FinTech Project

## 💰 FinTally

**Deterministic Personal Finance Analytics System**

FinTally is a financial analytics platform focused on **transparent financial computation rather than opaque AI-driven automation.**

### Architecture

Backend

* Node.js transaction ingestion
* Django analytics engine

Performance Layer

* Rust aggregation modules
* Selective C++ acceleration

ML Usage

* LLM used only for **intent parsing**
* Core financial logic remains deterministic

### Benchmarks

| Operation                      | Python | Rust   |
| ------------------------------ | ------ | ------ |
| Aggregation (10k transactions) | 1.2 s  | 0.4 s  |
| Monthly summary                | 0.8 s  | 0.25 s |

---

# Experimental Projects

## 📈 Revenue-AI

Financial forecasting and exploratory data analysis platform for testing **time-series models under CPU-only environments.**

Focus:

* model comparison
* training efficiency
* system performance profiling

---

## 📂 Taskflow-Ngnode

AI-assisted task management platform demonstrating **clean separation between deterministic rules and ML scoring systems.**

---

# Engineering Challenges Explored

* CPU-efficient neural network inference
* Measuring PyO3 / FFI boundary overhead
* Scaling approximate nearest-neighbor search
* Maintaining deterministic control over ML outputs
* Evaluating complexity vs measurable performance gains

---

# Engineering Philosophy

* Prefer **measured claims over adjectives**
* Optimize **only after profiling**
* Remove complexity when gains are marginal
* Keep deterministic systems in control of critical decisions

---

# Current Technical Priorities

* Concurrency patterns in backend systems
* Automated benchmarking pipelines
* Production observability and system instrumentation

---

📧 **Email**
[agondi982@gmail.com](mailto:agondi982@gmail.com)

📺 **YouTube**
[https://www.youtube.com/@ag_youtube](https://www.youtube.com/@ag_youtube)

---

> Build under constraints. Measure honestly. Refactor intentionally.

---
