# Anshu Gondi

**Backend & systems engineer.** I build things that have to work on real hardware.

B.Tech (1st year) · India · Open to internships, backend roles, technical collaboration

📧 [agondi982@gmail.com](mailto:agondi982@gmail.com) · 📺 [youtube.com/@ag_youtube](https://www.youtube.com/@ag_youtube)

---

## About

Most backend systems are designed assuming fast hardware. I build under the opposite assumption — everything I ship is benchmarked on a dual-core Celeron with 8 GB RAM and no GPU. That constraint isn't a limitation I work around; it's the discipline I design with.

My focus is on systems where correctness is non-negotiable and performance has to be earned: financial computation, identity matching at scale, and ML pipelines that run without cloud infrastructure.

> **Intel Celeron N4020 · 2 cores · 8 GB RAM · CPU-only inference**  
> Benchmarks on this machine, not a dev server.

---

## What I focus on

**Performance under constraint**  
Profile first. Reach for Rust/C++ only when benchmarks justify the complexity cost.

**Deterministic financial logic**  
Numbers that compute the same way every time. LLMs handle intent, not arithmetic.

**Controlled ML boundaries**  
ML outputs are validated before they touch data. No black-box mutations.

**FFI with real measurement**  
PyO3, napi-rs — used where the numbers prove it, not assumed.

---

## Projects

### 🏫 CampusVision
**Face-based attendance system for real classrooms — deployable on low-cost hardware** · `In Development`

**Problem**  
Manual attendance in large classrooms is slow, error-prone, and frequently gamed. Existing automated systems require expensive cameras or cloud inference.

**Solution**  
CPU-only face detection (YuNet) + ArcFace embeddings with a Rust-accelerated HNSW index for sub-20ms identity lookup. Runs on the same commodity hardware schools already own.

**Why it matters**  
Accuracy and latency that make real-classroom deployment viable without a hardware budget. The system degrades gracefully — CCTV provides audit trails when live detection is uncertain.

**Benchmarks**

| Operation | Python | Rust | Gain |
|-----------|--------|------|------|
| Embedding inference | 35 ms | **12 ms** | **2.9×** |
| HNSW search (1k faces) | 50 ms | **18 ms** | **2.8×** |

**Stack:** `Axum` `Django` `Rust/PyO3` `HNSW` `ArcFace` `MinIO` `React Native`

---

### 💰 FinTally
**Personal finance analytics — fully deterministic core, LLM used strictly for intent parsing** · `Stable + Active Dev`

**Problem**  
Personal finance tools either over-automate (opaque AI decisions on your money) or under-deliver (dumb spreadsheets with no insight layer).

**Solution**  
Hard separation: the Rust aggregation engine owns all numbers. An LLM layer — running locally via llama.cpp — translates natural-language queries into validated intent objects. The engine executes them. The LLM never touches raw figures.

**Why it matters**  
You can audit every computation. LLM confidence below threshold falls back to deterministic rules automatically. Financial logic that behaves the same way regardless of what the model does.

**Benchmarks**

| Operation | Python | Rust | Gain |
|-----------|--------|------|------|
| Aggregation (10k transactions) | 1.2 s | **0.4 s** | **3.0×** |
| Monthly summary | 0.8 s | **0.25 s** | **3.2×** |

**Stack:** `Node.js` `Django` `Rust/PyO3` `llama.cpp` `FastAPI` `PostgreSQL`

---

## Experiments

**📈 Revenue-AI**  
Financial forecasting testbed — comparing time-series models and profiling training efficiency under CPU-only constraints.

**📂 Taskflow-Ngnode**  
Task management with a clean boundary between deterministic scheduling rules and ML-assisted priority scoring.

---

## Stack

**Languages**  
`Python` `Rust` `C++` `TypeScript` `SQL`

**Backend**  
`FastAPI` `Django` `Axum` `Actix Web` `Node.js`

**FFI / Native**  
`PyO3` `napi-rs` `ONNX Runtime` `opencv-rs` `tch-rs`

**Data / Infra**  
`PostgreSQL` `Redis` `MinIO` `Docker` `GCP` `Linux`

---

> *Build under constraints. Measure honestly. Refactor intentionally.*
