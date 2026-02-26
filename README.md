# 👋 Hi, I’m Anshu Gondi

> Open to internships and remote collaborations
> Focused on backend systems, performance-aware design, and applied ML under real-world constraints.

🎓 B.Tech (1st Year) — India
💻 Backend & Systems-Focused Developer

---

## About Me

I build **systems under constrained hardware**, treating performance, correctness, and architecture as measurable engineering goals — not abstract terms.

Early projects with Python desktop apps and full-stack ML taught me **real bottlenecks**: CPU limits, architectural coupling, and latency ceilings on low-end hardware.

This led me to adopt a **measure-before-optimize workflow**:

**Build → Profile → Optimize → Re-measure → Refactor**

I selectively integrate Rust/C++ only where profiling proves measurable benefits.

---

## Core Focus

* Backend systems with explicit correctness boundaries
* CPU-constrained performance optimization
* Bounded ML integration with explicit resource control
* Rust/C++ via FFI for deterministic subsystems
* Profiling-driven design & production discipline

---

## Tech Stack

### Languages

Python · Rust · C++ · C · TypeScript · SQL

### Backend

Django · FastAPI · Node.js · Express · Axum · Actix

### Frontend

React · React Native · Angular

### Databases & Storage

PostgreSQL · MySQL · MongoDB · MinIO (S3-compatible)

### ML / Data

PyTorch · Scikit-learn · NumPy · Pandas · ONNX Runtime

### Systems & Interop

PyO3 · FFI · CXX · bindgen · OpenCV-rs · hnsw_rs

### DevOps

Docker · Linux · Git · CI/CD pipelines · Render · Railway · GCP

---

# 🚀 Featured Projects

**All benchmarks & development done on:**
Intel Celeron N4020 (2C/2T, 8GB RAM, CPU-only, 2017). Single-node, no GPU.

---

## 🏫 CampusVision

**Real-Time Face-Based Attendance System** | Active Development

**Engineering Context**

* End-to-end inference optimized for 2C/2T CPU
* Rust for face detection & embeddings
* Axum for ingestion & orchestration
* Django for authentication
* MinIO for storage
* React / React Native clients

**Current Work**

* Measuring latency & PyO3 FFI overhead
* Profiling CPU-only face embeddings vs Python baseline

> Benchmarks: Rust embedding search ~3–4x faster than Python under CPU-only

---

## 💰 FinTally

**Personal Finance Tracker** | Active Development

* Node.js API + Django analytics workflows
* Rust modules for aggregation, C++ via FFI for critical paths
* LLM restricted to UX-level parsing

**Focus**: deterministic aggregation & measurable CPU gains

> Benchmarks: Rust aggregation reduces 90th percentile latency by ~60% vs Python

---

## 📂 TaskFlow-NgNode

**AI-Assisted Task Management Platform** | Complete & Deployed

* Angular frontend, Node.js backend, MongoDB
* AI scheduler isolated behind FastAPI microservice
* Deterministic business rules separated from probabilistic ML scoring

**Highlights**: role-based access, team vs solo workspaces, Google auth, modern UI

---

## 📈 Revenue-AI

**Financial Forecasting & EDA Platform** | Complete & Deployed

* CPU-only ML: Linear Regression, Random Forest, PyTorch NN
* Benchmarked on small datasets (<5k rows)
* JWT & OAuth2 authentication

> Benchmarks: Random Forest ~3s, PyTorch NN ~3–4min CPU-only for 5k rows

---

## Engineering Philosophy

* **Measure first:** No optimization without profiling
* **Complexity vs gain:** Remove code if performance improvement is marginal
* **Bounded ML:** Deterministic logic drives decisions
* **Continuous refinement:** Concurrency, benchmarking, observability

---

📧 [agondi982@gmail.com](mailto:agondi982@gmail.com)
📺 YouTube: @ag_youtube

> Build under constraints. Measure honestly. Refactor intentionally.

---
