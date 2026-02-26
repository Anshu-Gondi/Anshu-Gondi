# 👋 Hi, I’m Anshu Gondi

> 💼 Open to internships and remote collaborations
> Focused on backend systems, performance-aware design, and applied AI under real-world constraints.

🎓 B.Tech (1st Year) — India
💻 Backend & Systems-Focused Developer
🤖 Applied ML in Production-Oriented Systems

---

## About Me

I’m a first-year engineering student focused on building **real, working systems** rather than isolated prototypes.

My early work began with Python desktop apps and full-stack web projects. As I moved into ML-backed systems, I started encountering real limitations — performance bottlenecks, system coupling, and architectural rigidity.

That pushed me toward:

* Understanding performance boundaries
* Profiling real bottlenecks
* Designing clearer separation between deterministic logic and AI components
* Introducing Rust/C++ selectively where constraints demanded it

I care less about “using advanced tools” and more about:

* Why they are used
* What measurable benefit they provide
* Whether the added complexity is justified

My approach is iterative:
Build → Measure → Refactor → Re-measure.

---

## Core Focus Areas

* Backend systems with explicit correctness boundaries
* Performance-aware Python systems
* Selective Rust/C++ integration via FFI (PyO3, CXX)
* AI used as a bounded tool, not a source of truth
* Refactoring early-stage projects into production-oriented architectures

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

---

## 🏫 CampusVision

Real-Time Face-Based Attendance System
**Status:** Active Development
**Hardware Baseline:** Intel Celeron N4020 (Gemini Lake, 2017) · 2C/2T · 1.10GHz · No GPU acceleration

### Engineering Context

All inference benchmarks are measured on:

* Intel Celeron N4020
* 2 cores / 2 threads
* 8GB RAM
* CPU-only execution
* Single-machine deployment

The goal is to understand system behavior under constrained compute rather than relying on high-performance hardware.

### Architecture

* Face detection, embeddings, and HNSW vector search implemented in Rust
* Axum for performance-sensitive ingestion endpoints
* Django for orchestration and authentication
* MinIO for object storage
* React / React Native clients

### Current Focus

* Measuring end-to-end latency on CPU-only inference
* Profiling Python vs Rust boundaries (PyO3 overhead)
* Determining if Rust gains justify architectural complexity
* Evaluating scaling behavior as face count increases

---

## 💰 FinTally

Personal Finance Tracker with Deterministic Computation Core
**Status:** Active Development
**Hardware Baseline:** Intel Celeron N4020 · 2C/2T · No distributed infra

### Engineering Context

Developed and tested entirely on low-power CPU hardware.

* No microservice deployment in production
* No horizontal scaling
* No assumed concurrency beyond hardware limits

### Architecture

* Node.js API layer
* Django analytics workflows
* Rust modules for financial aggregation
* Selective C++ interop via FFI
* LLM restricted to UX layer only

### Current Focus

* Profiling financial aggregation bottlenecks
* Comparing pure Python vs Rust performance on low-core CPU
* Measuring actual latency gains vs added maintenance cost
* Avoiding premature distributed architecture

---

## 📂 Taskflow-Ngnode

AI-Assisted Task Management Platform
**Status:** Complete & Deployed
**Hardware Baseline:** Developed on Intel Celeron N4020 · CPU-only

### Engineering Context

Designed without assuming GPU or high-core systems.

* ML isolated behind FastAPI service
* Single-node deployment
* Focus on separation of probabilistic scoring and deterministic task logic

Emphasis: maintainability under resource constraints.

---

## 📈 Revenue-AI

Financial Forecasting & EDA Platform
**Status:** Complete & Deployed
**Hardware Baseline:** Intel Celeron N4020 · CPU-only ML workloads

### Engineering Context

* CPU-only model training and inference
* No distributed compute
* Early-stage profiling discipline (being revisited)

This project represents my initial ML systems phase before adopting stronger performance-measurement practices in later projects.

# Engineering Philosophy

I prefer:

* Measured claims over adjectives
* Explicit bottlenecks over assumed ones
* Refactoring over constant new project creation
* Deterministic logic owning business-critical decisions

I am currently focused on strengthening:

* Profiling discipline
* Performance benchmarking
* Concurrency design
* Production-hardening existing systems

---

## Contact

📧 [agondi982@gmail.com](mailto:agondi982@gmail.com)
📺 YouTube: @ag_youtube

---

> Build first. Measure honestly. Refactor intentionally.

---
