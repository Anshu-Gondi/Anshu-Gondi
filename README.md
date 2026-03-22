# 👋 Hi, I’m Anshu Gondi

**Systems & Backend Developer focused on performance, FFI-based optimization, and CPU-constrained environments.**

🎓 B.Tech (1st Year) — India  
💻 Interested in **systems engineering**, **financial software**, and **high-performance backend infrastructure**

Open to **internships**, **backend roles**, and **technical collaborations**.

---

## About Me

I design backend systems that prioritize **correctness**, **performance**, and **measurable behavior** — especially in **CPU-constrained environments**.

Low-resource hardware experience taught me to treat performance as an **engineering problem to be measured**, not assumed.

Workflow emphasis:
- **Profiling before optimization**
- **Clear boundaries** between deterministic logic and ML subsystems
- **Rust/C++ only** when benchmarks justify the added complexity

Core loop:

```
Build → Measure → Refactor → Re-measure
```

Long-term goal: reliable financial and analytical platforms at scale.

---

## Core Engineering Focus

- Performance-aware backend systems  
- Rust/C++ acceleration via FFI  
- Deterministic financial computation  
- ML systems with strict control boundaries  

---

## Technical Stack

**Languages**  
Python · Rust · C++ · C · TypeScript · SQL  

**Backend**  
FastAPI · Django · Axum (Rust) · Actix Web · Node.js / Express  

**Databases**  
PostgreSQL · MySQL · MongoDB · **Redis** · MinIO  

**Machine Learning**  
PyTorch · scikit-learn · NumPy · Pandas · ONNX Runtime 

**Native Extensions & ML Systems (FFI / Bindings)**  

- **PyO3** — Rust ↔ Python (performance-critical modules)  
- **napi-rs / N-API** — Rust/C++ ↔ Node.js (native backend acceleration)  
- **tch-rs / ONNX Runtime** — running ML inference in Rust  
- **opencv-rs** — CV pipelines (face processing, embeddings)  

Focus:
- Eliminating Python/JS bottlenecks  
- Measuring FFI overhead vs real gains  
- Moving critical ML/CV paths to native execution  

**Infrastructure**  
Docker · Linux · Git · CI/CD · Render · Railway · GCP  

**Other**  
GenAI API integration (LLM APIs, structured prompting, system-level usage constraints)

---

## Flagship Project

### 🏫 CampusVision  
**Real-Time Face-Based Attendance Infrastructure** (In Development)

Reliable CPU-only classroom attendance system combining computer vision, high-performance backend, and scalable identity search — deployable on low-cost hardware.

**Architecture**  
- **Detection & Recognition**: YuNet (face detection) + ArcFace (embeddings)  
- **Performance Layer**: Rust-based embedding processing + HNSW (Hierarchical Navigable Small World) approximate nearest-neighbor search  
- **Backend**: Axum (Rust ingestion APIs) + Django (authentication/orchestration) + MinIO (object storage)  
- **Clients**: React web dashboard + React Native mobile  

**Deployment Strategy**  
- Primary: webcam / mobile camera recognition  
- Audit: CCTV for verification trail  
- Scalability: location-aware indexing  

**Benchmark Environment**  
```
Intel Celeron N4020
2 cores / 2 threads
8GB RAM
CPU-only inference
```

**Sample Benchmarks**

| Operation                | Rust  | Python |
|--------------------------|-------|--------|
| Embedding inference      | 12 ms | 35 ms  |
| HNSW search (1000 faces) | 18 ms | 50 ms  |

**Current Focus**  
- Multi-frame recognition validation  
- Location-based face index architecture  
- Real-classroom pilot deployment  

---

### 💰 FinTally  
**Deterministic Personal Finance Analytics System**

Transparent computation platform — no opaque AI automation.

**Architecture**  
- **Backend**: Node.js (transaction ingestion) + Django (analytics engine)  
- **Performance Layer**: Rust aggregation modules + selective C++ acceleration  
- **ML Usage**: LLM only for intent parsing; core financial logic fully deterministic  

**Benchmarks**

| Operation                      | Python | Rust   |
|--------------------------------|--------|--------|
| Aggregation (10k transactions) | 1.2 s  | 0.4 s  |
| Monthly summary                | 0.8 s  | 0.25 s |

---

## Experimental Projects

**📈 Revenue-AI**  
Financial forecasting & EDA platform testing time-series models under CPU-only constraints.  
Focus: model comparison, training efficiency, system performance profiling.

**📂 Taskflow-Ngnode**  
AI-assisted task management with clean separation between deterministic rules and ML scoring systems.

---

## Engineering Challenges Explored

- CPU-efficient neural network inference  
- Measuring PyO3 / FFI boundary overhead  
- Scaling approximate nearest-neighbor search  
- Maintaining deterministic control over ML outputs  
- Evaluating complexity vs measurable performance gains  

---

## Current Technical Priorities

- Concurrency patterns in backend systems  
- Automated benchmarking pipelines  
- Production observability and system instrumentation  

---

📧 **Email**: [agondi982@gmail.com](mailto:agondi982@gmail.com)  
📺 **YouTube**: [https://www.youtube.com/@ag_youtube](https://www.youtube.com/@ag_youtube)

---

> Build under constraints. Measure honestly. Refactor intentionally.
