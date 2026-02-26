# 👋 Hi, I’m Anshu Gondi

> Open to internships and remote collaborations
> Focused on backend systems, performance-aware design, and applied ML under real-world constraints.

🎓 B.Tech (1st Year) — India
💻 Backend & Systems-Focused Developer

---

## About Me

I build systems under **constrained hardware**, treating **performance, correctness, and architecture as measurable concerns** — not abstract goals.

Early work in Python desktop and full-stack apps exposed bottlenecks: CPU limits, architectural coupling, and latency ceilings on low-end hardware.

That pushed me toward:

* Profiling **before optimizing**
* Designing explicit boundaries between deterministic logic and probabilistic AI
* Introducing Rust/C++ only when profiling justifies it

**Workflow:**
**Build → Measure → Refactor → Re-measure**

---

## Core Focus

* Backend systems with explicit correctness boundaries
* CPU-constrained performance optimization
* Selective Rust/C++ integration via FFI (PyO3, CXX)
* ML as a bounded subsystem, **not a decision authority**
* Refactoring early-stage systems toward production discipline

---

## Tech Stack

**Languages:** Python · Rust · C++ · C · TypeScript · SQL
**Backend:** Django · FastAPI · Node.js · Express · Axum (Rust) · Actix (Rust)
**Frontend:** React · React Native · Angular
**Databases / Storage:** PostgreSQL · MySQL · MongoDB · MinIO (S3-compatible)
**ML / Data:** PyTorch · Scikit-learn · NumPy · Pandas · ONNX Runtime
**Interop / Systems:** PyO3 · FFI · CXX · bindgen · OpenCV-rs · hnsw_rs
**DevOps:** Docker · Linux · Git · CI pipelines · Render · Railway · GCP

---

# Featured Projects

**Hardware Baseline (all projects):**
Intel Celeron N4020, 2C/2T, 1.10 GHz, 8GB RAM, CPU-only, single-machine deployment

---

## 🏫 CampusVision

**Real-Time Face-Based Attendance System** | Active Development

**Engineering Context:**

* CPU-only inference, no CUDA/GPU
* Scaling behavior tested as face count increases

**Architecture:**

* Rust: face detection, embeddings, HNSW search
* Axum for ingestion; Django for auth & orchestration
* MinIO for image storage; React/React Native clients

**Mini Benchmark (CPU-only):**

| Operation              | Rust     | Python   |
| ---------------------- | -------- | -------- |
| Embedding inference    | 12ms/img | 35ms/img |
| HNSW search (1k faces) | 18ms     | 50ms     |

**Current Work:**

* Profiling PyO3 boundaries
* Measuring Rust vs Python latency
* Evaluating architectural cost vs gain

---

## 💰 FinTally

**Personal Finance Tracker with Deterministic Core** | Active Development

**Engineering Context:**

* CPU-constrained; no horizontal scaling
* No microservice deployment; single-node focus

**Architecture:**

* Node.js API, Django analytics
* Rust modules for aggregation; selective C++ via FFI
* LLM restricted to UX intent parsing

**Mini Benchmark (CPU-only):**

| Operation          | Python | Rust  |
| ------------------ | ------ | ----- |
| Aggregation 10k tx | 1.2s   | 0.4s  |
| Monthly summary    | 0.8s   | 0.25s |

**Current Work:**

* Profiling bottlenecks
* Measuring latency improvement vs complexity
* Comparing Python vs Rust implementations

---

## 📂 Taskflow-Ngnode

**AI-Assisted Task Management Platform** | Deployed

* ML isolated behind FastAPI service
* Deterministic rules separate from probabilistic scoring
* Single-node deployment

**Focus:** Clean separation between business logic and ML

---

## 📈 Revenue-AI

**Financial Forecasting & EDA Platform** | Deployed

* CPU-only ML training & inference
* JWT & OAuth2 authentication
* Comparative time-series evaluation

**Mini Benchmark (CPU-only):**

| Dataset | Model             | Training Time |
| ------- | ----------------- | ------------- |
| 5k rows | Linear Regression | 0.8s          |
| 5k rows | Random Forest     | 3.2s          |
| 5k rows | PyTorch NN        | ~3–4 min      |

**Focus:** Early ML architecture phase, later refined for performance measurement

---

## Challenges Solved

* CPU-only neural network inference & optimization
* Profiling PyO3 & FFI overheads
* Scaling HNSW search for embeddings
* Separating deterministic business logic from ML scoring
* Measuring real latency gains vs added complexity

---

## Engineering Philosophy

* Prefer **measured claims** over adjectives
* Optimize **only after profiling**
* Remove complexity if gain is marginal
* Keep deterministic logic in control of critical decisions

Current focus areas:

* Concurrency design
* Benchmark automation
* Production hardening
* Observability

---

📧 [agondi982@gmail.com](mailto:agondi982@gmail.com)
📺 YouTube: @ag_youtube

> Build under constraints. Measure honestly. Refactor intentionally.

---
