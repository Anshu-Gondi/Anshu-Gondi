# 👋 Hi, I'm Anshu Gondi

**Systems & Backend Developer** — performance, FFI-based optimization, and CPU-constrained environments.

🎓 B.Tech (1st Year) · India &nbsp;|&nbsp; 💼 Open to **internships**, **backend roles**, and **technical collaborations**

---

## About Me

I design backend systems that prioritize **correctness**, **performance**, and **measurable behavior** — especially in **CPU-constrained environments**.

Low-resource hardware experience taught me to treat performance as an **engineering problem to be measured**, not assumed.

**Workflow:**
- Profiling before optimization
- Clear boundaries between deterministic logic and ML subsystems
- Rust/C++ only when benchmarks justify the added complexity

```
Build → Measure → Refactor → Re-measure
```

**Long-term goal:** Reliable financial and analytical platforms at scale.

> **All projects are developed and benchmarked on the same machine:**
> ```
> Intel Celeron N4020 · 2 cores / 2 threads · 8 GB RAM · CPU-only inference
> ```
> Performance is not assumed — it is measured on constrained hardware from day one.

---

## Core Engineering Focus

- Performance-aware backend systems
- Rust/C++ acceleration via FFI
- Deterministic financial computation
- ML systems with strict control boundaries

---

## Technical Stack

**Languages**
`Python` `Rust` `C++` `C` `TypeScript` `SQL`

**Backend**
`FastAPI` `Django` `Axum (Rust)` `Actix Web` `Node.js / Express`

**Frontend**
`React (JS + TS)` `React Native` `Angular`

**Databases**
`PostgreSQL` `MySQL` `MongoDB` `Redis` `MinIO`

**Machine Learning**
`PyTorch` `scikit-learn` `NumPy` `Pandas` `ONNX Runtime`

**Native Extensions & FFI / Bindings**

| Binding | Use |
|---|---|
| **PyO3** | Rust ↔ Python (performance-critical modules) |
| **napi-rs / N-API** | Rust/C++ ↔ Node.js (native backend acceleration) |
| **tch-rs / ONNX Runtime** | ML inference in Rust |
| **opencv-rs** | CV pipelines (face processing, embeddings) |

Focus: eliminating Python/JS bottlenecks · measuring FFI overhead vs real gains · moving critical ML/CV paths to native execution.

**Infrastructure**
`Docker` `Linux` `Git` `CI/CD` `Render` `Railway` `GCP`

**Other**
GenAI API integration (LLM APIs, structured prompting, system-level usage constraints)

---

## Flagship Projects

---

### 🏫 CampusVision
**Real-Time Face-Based Attendance Infrastructure** · `In Development`

Reliable CPU-only classroom attendance system combining computer vision, high-performance backend, and scalable identity search — deployable on low-cost hardware.

**Architecture**
- **Detection & Recognition:** YuNet (face detection) + ArcFace (embeddings)
- **Performance Layer:** Rust-based embedding processing + HNSW approximate nearest-neighbor search
- **Backend:** Axum (Rust ingestion APIs) + Django (auth/orchestration) + MinIO (object storage)
- **Clients:** React web dashboard + React Native mobile

**Deployment Strategy**
- Primary: webcam / mobile camera recognition
- Audit: CCTV for verification trail
- Scalability: location-aware indexing

**Benchmarks**

| Operation | Python | Rust | Speedup |
|---|---|---|---|
| Embedding inference | 35 ms | **12 ms** | **2.9×** |
| HNSW search (1000 faces) | 50 ms | **18 ms** | **2.8×** |

**Current Focus**
- Multi-frame recognition validation
- Location-based face index architecture
- Real-classroom pilot deployment

---

### 💰 FinTally
**Deterministic Personal Finance Analytics System**

Transparent computation platform — no opaque AI automation. Core financial logic is fully deterministic; LLM is used only for intent parsing.

---

#### `main` — Stable Release

> Production-ready version. Deterministic aggregation engine with selective Rust/C++ acceleration.

**Architecture**
- **Backend:** Node.js (transaction ingestion) + Django (analytics engine)
- **Performance Layer:** Rust aggregation modules + selective C++ acceleration
- **ML Usage:** LLM only for intent parsing; all financial logic is deterministic

**Benchmarks**

| Operation | Python | Rust | Speedup |
|---|---|---|---|
| Aggregation (10k transactions) | 1.2 s | **0.4 s** | **3.0×** |
| Monthly summary | 0.8 s | **0.25 s** | **3.2×** |

---

#### `dev/llm-analytics` — Active Development Branch

> Extending FinTally with a richer LLM integration layer and a deeper analytics engine — while keeping the deterministic core untouched.

**LLM Stack**

| Component | Role |
|---|---|
| **FastAPI** | LLM service API — exposes intent endpoints to the main backend |
| **llama.cpp** | CPU-optimized local LLM inference (no GPU, no cloud dependency) |
| **PyO3** | Rust ↔ Python bridge — hot paths in the LLM pre/post processing offloaded to Rust |

Running quantized models via llama.cpp on the Celeron N4020 — inference is measured, not assumed viable.

**What's being added:**

- **Structured LLM pipeline** — moving from single-shot intent parsing to a multi-step reasoning chain:
  - Query classification → context injection → structured JSON output → deterministic execution
  - LLM never touches raw numbers; it only emits validated intent objects consumed by the Rust engine
  - PyO3 used to accelerate token pre-processing and schema validation at the Rust layer

- **Enhanced analytics engine:**
  - Spending pattern detection with configurable rule sets
  - Anomaly flagging (statistical thresholds, not ML black-boxes)
  - Multi-period trend analysis (MoM, YoY, rolling windows)
  - Category inference with LLM-assisted tagging (human-overridable)

- **LLM integration boundaries (strict):**
  - LLM output is always schema-validated before entering the computation layer
  - No LLM call can mutate financial records — read-only intent resolution only
  - Fallback to deterministic rules if LLM confidence score is below threshold

- **Observability additions:**
  - Per-request LLM latency and token throughput tracking (tokens/sec on CPU)
  - Token usage logging per intent type
  - Comparison dashboards: LLM-assisted vs rule-only results

**Design constraint being maintained:**
```
llama.cpp (FastAPI) = intent layer only        ← PyO3 bridges hot paths to Rust
Rust engine         = source of truth for all numbers
```

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

📧 **Email:** [agondi982@gmail.com](mailto:agondi982@gmail.com)
📺 **YouTube:** [youtube.com/@ag_youtube](https://www.youtube.com/@ag_youtube)

---

> *Build under constraints. Measure honestly. Refactor intentionally.*
