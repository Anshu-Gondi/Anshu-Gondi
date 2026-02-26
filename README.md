# 👋 Hi, I’m Anshu Gondi

**Open to internships and remote collaborations**  
**Focused on backend systems, performance-aware design, and applied ML under real-world constraints**

🎓 B.Tech (1st Year) — India  
💻 Backend & Systems-Focused Developer

---

## About Me

I build systems that run efficiently under **constrained hardware**, treating **performance**, **correctness**, and **architecture** as **measurable engineering concerns** — not vague aspirations.

Early Python desktop and full-stack projects revealed hard limits: CPU bottlenecks, tight architectural coupling, and latency ceilings on low-end devices. This drove me toward deliberate practices:

- Profiling **before** any optimization
- Designing clear boundaries between deterministic logic and probabilistic ML
- Introducing Rust or C++ **only** when profiling shows meaningful gains

**Core workflow:** Build → Measure → Refactor → Re-measure

---

## Core Focus Areas

- Backend systems with explicit correctness & safety boundaries
- Performance optimization on CPU-constrained environments
- Selective Rust/C++ integration via FFI (PyO3, CXX)
- Treating ML as a **bounded subsystem**, never the decision authority
- Refactoring early-stage codebases toward production-grade discipline

---

## Tech Stack

**Languages**  
Python · Rust · C++ · C · TypeScript · SQL

**Backend**  
FastAPI · Django · Axum (Rust) · Actix Web (Rust) · Node.js / Express

**Frontend**  
React · React Native · Angular

**Databases & Storage**  
PostgreSQL · MySQL · MongoDB · MinIO (S3-compatible)

**ML & Data**  
PyTorch · scikit-learn · NumPy · Pandas · ONNX Runtime

**Interop & Systems**  
PyO3 · CXX · bindgen · OpenCV-rs · hnsw_rs

**DevOps & Tools**  
Docker · Linux · Git · CI/CD pipelines · Render · Railway · GCP

---

## Featured Projects

**All projects are benchmarked on the same constrained baseline hardware:**  
Intel Celeron N4020 (2C/2T @ 1.10 GHz), 8 GB RAM, CPU-only, single-machine deployment

### 🏫 CampusVision  
**Real-Time Face-Based Attendance System** | In active development

**Key constraints & decisions**  
- CPU-only inference (no CUDA/GPU)  
- Scaling behavior validated with increasing face counts

**Architecture**  
- Rust: face detection, embeddings generation, HNSW approximate nearest-neighbor search  
- Axum (Rust) for high-performance ingestion API  
- Django for authentication & orchestration  
- MinIO for image/object storage  
- React + React Native clients

**Mini Benchmark (CPU-only)**

| Operation                  | Rust     | Python   |
|----------------------------|----------|----------|
| Embedding inference (per image) | 12 ms   | 35 ms   |
| HNSW search (1,000 faces)  | 18 ms   | 50 ms   |

**Current focus**  
- Profiling PyO3 boundary overhead  
- Quantifying Rust vs Python latency trade-offs  
- Evaluating architectural complexity vs performance gain

### 💰 FinTally  
**Personal Finance Tracker with Deterministic Core** | In active development

**Key constraints**  
- Single-node, CPU-constrained (no horizontal scaling or microservices)

**Architecture**  
- Node.js API + Django analytics backend  
- Rust modules for high-speed aggregation  
- Selective C++ via FFI for critical paths  
- LLM used only for UX intent parsing (never for core logic)

**Mini Benchmark (CPU-only)**

| Operation             | Python | Rust  |
|-----------------------|--------|-------|
| Aggregation (10k tx)  | 1.2 s | 0.4 s |
| Monthly summary       | 0.8 s | 0.25 s|

**Current focus**  
- Identifying remaining bottlenecks  
- Measuring latency gains against added complexity

### 📂 Taskflow-Ngnode  
**AI-Assisted Task Management Platform** | Deployed

- ML isolated behind FastAPI microservice  
- Strict separation: deterministic rules vs probabilistic scoring  
- Single-node deployment

**Philosophy**  
Clean decoupling of business logic from ML components

### 📈 Revenue-AI  
**Financial Forecasting & EDA Platform** | Deployed

- CPU-only training & inference pipelines  
- JWT + OAuth2 authentication  
- Comparative evaluation of time-series models

**Mini Benchmark (CPU-only, 5k rows)**

| Model              | Training Time    |
|--------------------|------------------|
| Linear Regression  | 0.8 s           |
| Random Forest      | 3.2 s           |
| PyTorch NN         | ~3–4 min        |

**Focus**  
Early-stage ML architecture, later refined with rigorous performance measurement

---

## Challenges I’ve Tackled

- Efficient CPU-only neural network inference & optimization
- Measuring & minimizing PyO3 / FFI boundary overhead
- Scaling HNSW-based embedding search under memory/CPU limits
- Enforcing separation between deterministic business rules and ML outputs
- Quantifying actual latency wins vs added system complexity

---

## Engineering Philosophy

- Prefer **measured claims** over adjectives
- Optimize **only after profiling**
- Ruthlessly remove complexity when gains are marginal
- Keep deterministic logic in full control of critical decisions

**Current priorities**  
- Effective concurrency design  
- Automated benchmarking pipelines  
- Production hardening & observability

---

📧 [agondi982@gmail.com](mailto:agondi982@gmail.com)  
📺 YouTube: [@ag_youtube](https://www.youtube.com/@ag_youtube)

> Build under constraints. Measure honestly. Refactor intentionally.
