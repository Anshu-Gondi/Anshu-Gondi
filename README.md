<!-- Header -->
<div align="center">

```
┌─────────────────────────────────────────────────────────────┐
│  Intel Celeron N4020 · 2 cores · 2 threads · 8 GB RAM                  │
│  CPU-only inference · No GPU · No cloud · No excuses                   │
└─────────────────────────────────────────────────────────────┘
```

# Anshu Gondi

**Full-stack engineer with systems depth.**  
React to Rust — all the way down.

`B.Tech · 1st year · India` · Open to internships in full-stack, backend, and systems roles

[![Email](https://img.shields.io/badge/agondi982@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:agondi982@gmail.com)
[![YouTube](https://img.shields.io/badge/@ag__youtube-FF0000?style=flat-square&logo=youtube&logoColor=white)](https://www.youtube.com/@ag_youtube)

</div>

---

## // about

I ship **complete products** — frontend, backend, database, deployment, and native acceleration in Rust & C++ where benchmarks justify it. Most developers work in one layer. I build across all of them and care deeply about how they connect and perform under real constraints.

**What makes this unusual:** Everything I build is benchmarked and optimized on a dual-core Celeron N4020 with 8 GB RAM — CPU-only. That constraint isn't a footnote. It's load-bearing. It forces honest engineering decisions at every level and makes every performance number mean something real.

---

## // how I build

| Principle | Practice |
|-----------|----------|
| **End-to-end ownership** | React / React Native → FastAPI / Axum → PostgreSQL / Redis / MinIO → Docker + GCP |
| **Performance under constraint** | Profile first. Rust + C++ via FFI for hot paths. Python only where it adds productivity without cost. |
| **Deterministic financial logic** | Rust/C++ owns all numbers and calculations. LLMs handle intent only — never raw data. |
| **Controlled ML boundaries** | ML outputs validated before touching core data. No black-box mutations. |

---

## // projects

### 🏫 CampusVision
> **Full-stack attendance platform with three-layer anti-fraud verification** · `In Development`

**Problem:** Manual attendance is trivially gamed — proxies, printed photos, screen replays are all common. Existing hardware-based solutions are expensive. Most software solutions have one layer of defense, which means one layer to defeat.

**Solution:** End-to-end system with a three-stage verification pipeline that must fully pass before attendance is marked:

```
Stage 1 → Face recognition
          YuNet detection + SFace embeddings
          matched against a Rust-accelerated HNSW index

Stage 2 → Liveness check via emotion
          Emotion-8-FerPlus model detects static photos
          and screen replays (flat/neutral affect signature)

Stage 3 → CCTV cross-verification
          Cross-checks identity against school CCTV
          to confirm physical presence in the building
```

**Architecture:** React Native mobile + React web dashboard → Rust (Axum) ingestion & orchestration API → C++ performance-critical components via FFI → Rust-accelerated HNSW index → MinIO storage. No GPU required.

**Benchmarks** *(Celeron N4020 · 2 cores · 2 threads · 8 GB RAM · CPU-only)*

| Operation | Time | vs baseline |
|-----------|------|-------------|
| Embedding inference | **< 12 ms** | ~3× faster |
| HNSW search (1k faces) | **< 18 ms** | ~2.8× faster |

**Stack:**
`React Native` `React` `Axum (Rust)` `C++ (FFI)` `SFace` `HNSW` `ONNX Runtime` `MinIO` `Docker`

---

### 💰 FinTally
> **Full-stack finance platform — React frontend, FastAPI + Rust extensions (stable) / Pure Rust (dev)** · `Stable + Active Dev`

**Problem:** Personal finance tools are either opaque (AI that auto-decides things for you) or shallow. You shouldn't have to trust a black box with your numbers.

**Solution:** Clean separation between deterministic calculations and intelligent intent parsing.

```
Stable version:
  React dashboard
  → FastAPI backend + Rust extensions (PyO3) for high-performance aggregation
  → Local llama.cpp for natural-language queries
    (LLM produces validated intent objects only — never touches raw numbers)

Dev version (Pure Rust):
  Candle for ML components
  → C++ FFI for the hottest numerical and aggregation paths
  → Maximum performance and control on constrained hardware
  → Fully local — no cloud or GPU dependency
```

**Benchmarks** *(Celeron N4020 · 2 cores · 2 threads · 8 GB RAM · CPU-only)*

| Operation | Python | Rust / Rust+C++ | Gain |
|-----------|--------|-----------------|------|
| Aggregation (10k transactions) | 1.2 s | **0.04 s** | **30×** |
| Monthly summary | 0.8 s | **0.025 s** | **32×** |

**Stack:**

- **Stable:** `React` `FastAPI` `Rust (PyO3)` `llama.cpp` `PostgreSQL` `Docker`
- **Dev:** `Rust` `Candle` `C++ (FFI)` `Axum` `Tokio`

---

## // experiments

**📈 Revenue-AI** — Financial forecasting testbed comparing time-series models under strict CPU-only constraints.

**📂 Taskflow-Ngnode** — AI-assisted task management with explicit boundaries between deterministic rules and ML-assisted scoring.

---

## // stack

```
Languages      Rust · C++ · Python · TypeScript · JavaScript · SQL

Frontend       React · React Native · Angular · TypeScript

Backend        FastAPI · Axum · Actix Web · Node.js

Native/Perf    PyO3 · C++ FFI · Candle · ONNX Runtime · HNSW · opencv-rs

Data/Infra     PostgreSQL · Redis · MinIO · Docker · GCP · Linux
```

---

<div align="center">

*build under constraints. measure honestly. refactor intentionally.*

</div>
