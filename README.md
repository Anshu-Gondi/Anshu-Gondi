# 👋 Hi, I’m Anshu Gondi

> Open to internships and remote collaborations
> Focused on backend systems, performance-aware design, and applied ML under real-world constraints.

🎓 B.Tech (1st Year) — India
💻 Backend & Systems-Focused Developer

---

## About Me

I build systems under constrained hardware and treat performance, correctness, and architecture as measurable concerns — not abstract goals.

My early work began with Python desktop and full-stack applications. As I integrated ML components, I encountered real bottlenecks: CPU limits, architectural coupling, and latency ceilings on low-end hardware.

That pushed me toward:

* Profiling before optimizing
* Designing explicit boundaries between deterministic logic and probabilistic AI
* Introducing Rust/C++ only when profiling justified it

My workflow is simple:

**Build → Measure → Refactor → Re-measure**

---

## Core Focus

* Backend systems with explicit correctness boundaries
* CPU-constrained performance optimization
* Selective Rust/C++ integration via FFI (PyO3, CXX)
* ML as a bounded subsystem, not a decision authority
* Refactoring early-stage systems toward production discipline

---

## Tech Stack

### Languages

Python · Rust · C++ · C · TypeScript · SQL

### Backend

Django · FastAPI · Node.js · Express
Axum (Rust) · Actix (Rust)

### Frontend

React · React Native · Angular

### Databases & Storage

PostgreSQL · MySQL · MongoDB
MinIO (S3-compatible object storage)

### ML / Data

PyTorch · Scikit-learn · NumPy · Pandas · ONNX Runtime

### Systems & Interop

PyO3 · FFI · CXX · bindgen · OpenCV-rs · hnsw_rs

### DevOps

Docker · Linux · Git · CI pipelines
Deployments on Render, Railway, GCP

---

# Featured Projects

All major projects developed and benchmarked on:

**Intel Celeron N4020 (Gemini Lake, 2017)**
2 cores / 2 threads · 1.10 GHz · 8GB RAM · CPU-only
No GPU acceleration · Single-machine deployment

---

## 🏫 CampusVision

Real-Time Face-Based Attendance System
**Status:** Active Development

### Engineering Context

* End-to-end inference benchmarked on 2C/2T CPU
* No CUDA/GPU
* Evaluating scaling behavior as face count increases

### Architecture

* Face detection, embeddings, and HNSW search implemented in Rust
* Axum for performance-sensitive ingestion
* Django for authentication and orchestration
* MinIO for image storage
* React / React Native clients

### Current Work

* Measuring Rust vs Python latency under CPU limits
* Profiling PyO3 boundary overhead
* Validating whether Rust gains justify architectural cost

---

## 💰 FinTally

Personal Finance Tracker with Deterministic Computation Core
**Status:** Active Development

### Engineering Context

* Built under strict CPU constraints
* No horizontal scaling assumptions
* No production microservice deployment

### Architecture

* Node.js API layer
* Django analytics workflows
* Rust modules for financial aggregation
* Selective C++ via FFI
* LLM restricted to UX-level intent parsing

### Current Work

* Profiling financial aggregation bottlenecks
* Comparing pure Python vs Rust implementations
* Measuring real latency improvement vs complexity increase

---

## 📂 Taskflow-Ngnode

AI-Assisted Task Management Platform
**Status:** Complete & Deployed

* ML isolated behind FastAPI service
* Deterministic task rules separated from probabilistic scoring
* Single-node deployment

Focus: clean separation between business logic and ML.

---

## 📈 Revenue-AI

Financial Forecasting & EDA Platform
**Status:** Complete & Deployed

* CPU-only model training and inference
* Comparative time-series evaluation
* JWT & OAuth2 authentication

This project reflects my earlier ML architecture phase before adopting stricter performance measurement discipline.

---

# Engineering Philosophy

* Prefer measured claims over adjectives
* Optimize only after profiling
* Remove complexity if performance gain is marginal
* Keep deterministic logic in control of critical decisions

Current areas of improvement:

* Concurrency design
* Benchmark automation
* Production hardening
* Observability

---

📧 [agondi982@gmail.com](mailto:agondi982@gmail.com)
📺 YouTube: @ag_youtube

> Build under constraints. Measure honestly. Refactor intentionally.

---
