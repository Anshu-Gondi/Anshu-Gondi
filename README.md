# Anshu Gondi

**Full-stack engineer with a systems depth.** I build end-to-end — from React UI to backend APIs to native performance layer — and I make it run on real hardware.

B.Tech (1st year) · India · Open to internships, full-stack/backend roles, technical collaboration

📧 [agondi982@gmail.com](mailto:agondi982@gmail.com) · 📺 [youtube.com/@ag_youtube](https://www.youtube.com/@ag_youtube)

---

## About

I ship complete products — frontend, backend, database, deployment, and where needed, native acceleration in Rust or C++. Most developers work within one layer; I build across all of them and care about how they connect.

What makes this unusual: everything I build is benchmarked on a dual-core Celeron with 8 GB RAM and no GPU. That forces real engineering decisions at every layer — you can't paper over a bad backend with a fast machine.

> **Intel Celeron N4020 · 2 cores · 8 GB RAM · CPU-only inference**  
> Benchmarks on this machine, not a dev server.

---

## How I build

**End-to-end ownership**  
React/Angular UI → Node/Django/FastAPI backend → PostgreSQL/Redis/MinIO data layer → Docker + GCP deployment. I ship the whole thing.

**Performance under constraint**  
Profile first. Reach for Rust/C++ via FFI only when benchmarks justify the complexity cost.

**Deterministic financial logic**  
Numbers that compute the same way every time. LLMs handle intent, not arithmetic.

**Controlled ML boundaries**  
ML outputs are validated before they touch data. No black-box mutations.

---

## Projects

### 🏫 CampusVision
**Full-stack attendance platform — React Native client, Rust/Django backend, three-layer anti-fraud verification** · `In Development`

**Problem**  
Manual attendance is slow and easy to game — proxies, photos, and impersonation are common. Existing automated systems either require expensive hardware or have no fraud detection layer at all.

**Solution**  
End-to-end system with a three-stage verification pipeline before attendance is ever marked:

1. **Face recognition** — YuNet detection + ArcFace embeddings matched against a Rust-accelerated HNSW index. Identifies the person.
2. **Liveness check via emotion** — Emotion-8-FerPlus model runs immediately after recognition. A static photo or screen replay produces flat/neutral affect; a real person in a live environment doesn't. Catches spoofing attempts that fool face recognition alone.
3. **CCTV cross-verification** — The recognized identity is cross-checked against CCTV footage to confirm physical presence in the room. Someone who passed recognition and liveness remotely still can't mark attendance without being physically there.

Only when all three stages pass does the backend mark attendance. Any stage failure is logged for manual review.

Full stack: React Native mobile client + React web dashboard → Axum (Rust) ingestion API → Django auth/orchestration → Rust-accelerated HNSW identity index → MinIO storage. Runs on commodity hardware, no GPU required.

**Why it matters**  
Most attendance systems stop at face recognition — that's one lock on the door. The emotion model catches spoofed media; CCTV catches physical proxies. Three layers together make fraud meaningfully harder without adding cost — CCTV infrastructure schools already have.

**Benchmarks**

| Operation | Python | Rust | Gain |
|-----------|--------|------|------|
| Embedding inference | 35 ms | **12 ms** | **2.9×** |
| HNSW search (1k faces) | 50 ms | **18 ms** | **2.8×** |

**Stack:** `React Native` `React` `Axum` `Django` `Rust/PyO3` `HNSW` `ArcFace` `Emotion-8-FerPlus` `ONNX Runtime` `MinIO` `Docker`

---

### 💰 FinTally
**Full-stack finance platform — React frontend, Node/Django backend, Rust aggregation engine, local LLM** · `Stable + Active Dev`

**Problem**  
Personal finance tools either over-automate (opaque AI decisions on your money) or under-deliver (dumb spreadsheets with no insight layer).

**Solution**  
Complete product: React dashboard → Node.js ingestion → Django analytics → Rust aggregation engine → llama.cpp local LLM for intent parsing. Hard separation: the Rust engine owns all numbers. The LLM translates natural-language queries into validated intent objects. It never touches raw figures.

**Why it matters**  
You get the insight layer without sacrificing auditability. LLM confidence below threshold falls back to deterministic rules. Runs fully local — no cloud dependency, no GPU required.

**Benchmarks**

| Operation | Python | Rust | Gain |
|-----------|--------|------|------|
| Aggregation (10k transactions) | 1.2 s | **0.4 s** | **3.0×** |
| Monthly summary | 0.8 s | **0.25 s** | **3.2×** |

**Stack:** `React` `Node.js` `Django` `FastAPI` `Rust/PyO3` `llama.cpp` `PostgreSQL` `Docker`

---

## Experiments

**📈 Revenue-AI**  
Financial forecasting testbed — comparing time-series models and profiling training efficiency under CPU-only constraints.

**📂 Taskflow-Ngnode**  
AI-assisted task management with a clean boundary between deterministic scheduling rules and ML-assisted priority scoring.

---

## Stack

**Languages**  
`Python` `Rust` `C++` `TypeScript` `JavaScript` `SQL`

**Frontend**  
`React` `React Native` `Angular` `TypeScript` `JavaScript`

**Backend**  
`FastAPI` `Django` `Axum` `Actix Web` `Node.js` `Express`

**FFI / Native**  
`PyO3` `napi-rs` `ONNX Runtime` `opencv-rs` `tch-rs`

**Data / Infra**  
`PostgreSQL` `Redis` `MinIO` `Docker` `GCP` `Linux`

---

> *Build under constraints. Measure honestly. Refactor intentionally.*
