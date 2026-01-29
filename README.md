# 👋 Hi, I’m Anshu Gondi

> 💼 **Open to internships and remote collaborations** — focused on **systems-oriented full-stack development and applied AI architectures**.

🎓 **B.Tech 1st Year Student (India)**
💻 **Systems-Focused Full-Stack Developer** · 🤖 **Applied AI / ML Systems Builder** · 🌍 **Open-Source Contributor**

---

## About Me

I’m a first-year engineering student who builds **production-oriented software systems**, not just demos. My work focuses on **clean architecture, correctness boundaries, and performance-aware design**, especially in projects that combine AI with real-world constraints.

I’m particularly interested in **hybrid architectures** where:

* deterministic, safety-critical logic is enforced at the systems level (Rust / C / C++)
* higher-level orchestration and UX are handled by Python or web frameworks
* AI components are treated as *untrusted but useful* tools, not sources of truth

I prioritize **shipping, testing, and real usage feedback** over theoretical perfection.

---

## Core Strengths

* Designing **hybrid AI systems** with clear trust boundaries
* Rust-based performance modules integrated into Python and web stacks
* Safe language interop (PyO3, FFI, CXX)
* Backend systems that emphasize **correctness, observability, and scalability**
* Turning experimental ideas into **deployable services**

---

## Tech Stack

### Languages

Python · TypeScript · JavaScript · Rust · C++ · C · SQL

### Frontend

React · React Native · Angular

### Backend & Frameworks

FastAPI · Django · Node.js · Express · Actix (Rust) · Warp (Rust)

### Databases

PostgreSQL · MySQL · MongoDB

### AI / ML

PyTorch · Scikit-learn · NumPy · Pandas · ONNX Runtime

### Systems & Interop

PyO3 · FFI · CXX · bindgen · OpenCV-rs · hnsw_rs

### DevOps & Tooling

Docker · Git · Linux · CI-oriented development · Cloud deployments (Render, Railway, GCP)

---

## Featured Projects

### 🏫 CampusVision — Real-Time Face-Based Attendance System

**Status:** In active development

**Tech:** Django REST · React · React Native · PostgreSQL · Rust (core engine) · PyO3

**Overview:**
CampusVision is a multi-camera, multi-campus attendance platform designed with a **strict separation between AI inference and system correctness**.

**Key Design Decisions:**

* All computer-vision logic (face detection, embeddings, vector search) runs in **Rust** for determinism, memory safety, and predictable latency
* Python/Django is used strictly for orchestration, APIs, and authentication
* HNSW-based vector search enables low-latency real-time matching
* Rust modules are fully tested and validated *before* being exposed to the API layer
* Frontend access provided via React (dashboard) and React Native (mobile)

**Focus:** Scalability, correctness, and real-world deployment constraints rather than model novelty.

---

### 💰 FinTally — Personal Finance Tracker with AI Insights

**Status:** Active development

**Tech:** React · Node.js · Django · MongoDB · Rust · C++

**Overview:**
FinTally is a personal finance platform built to explore **multi-language backend architectures** and performance-sensitive computation.

**Architecture Highlights:**

* Node.js for fast API responses
* Django for analytics and data processing
* Rust for memory-safe, low-latency financial computations
* C++ modules integrated via FFI for high-performance numerical workloads and legacy compatibility
* Conversational chatbot implemented as a **UX layer** for querying financial data and explaining insights
* LLM used strictly for intent parsing and natural-language explanations
* All financial rules, calculations, and validations handled by deterministic Rust backend modules
* Chatbot outputs are validated and constrained by backend invariants before execution

**Key Learnings:** System boundaries, interop costs, and trade-offs between developer velocity and runtime performance.

---

### 📂 Taskflow-Ngnode — AI-Assisted Task Management Platform

**Status:** Complete & deployed

**Tech:** Angular · Node.js · FastAPI

**Features:**

* Rule-based + ML-assisted task scheduling
* Role-based access control and notifications
* AI services isolated behind a FastAPI microservice

**Focus:** Practical ML integration without coupling core logic to probabilistic components.

---

### 📈 Revenue-AI — Financial Forecasting & EDA Platform

**Status:** Complete & deployed

**Tech:** Django · PyTorch · PostgreSQL · Node.js (proxy)

**Features:**

* Time-series forecasting and exploratory data analysis
* Multiple classical and ML models with comparative evaluation
* Exportable results (CSV, Excel, JSON)
* Secure authentication (JWT + OAuth2)

---

## Learning & Systems Background

### Systems Programming

* Strong foundations in **C, C++, and Rust**
* Focus on memory management, ownership models, concurrency, and safe interop
* Experience integrating Rust with Python and C++ in real systems

### Machine Learning

* From exploratory notebooks to modular, reusable pipelines
* Emphasis on **deployment readiness, reproducibility, and evaluation**
* Comfortable using ML as a component within larger systems, not in isolation

---

## Security & Authentication

* JWT-based authentication flows
* OAuth 2.0 (Google)
* Secure token handling and session design

---

## Open Source & Activity

* Active GitHub contributor across full-stack, AI, and systems projects
* Preference for clean code, tests, and maintainable architectures

---

## Connect

📧 **Email:** [agondi982@gmail.com](mailto:agondi982@gmail.com)
📺 **YouTube:** @ag_youtube

---

> *Always building systems that work in practice — not just in theory.*
