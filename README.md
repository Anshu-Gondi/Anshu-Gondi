# 👋 Hi, I’m Anshu Gondi

> 💼 **Open to internships and remote collaborations** — focused on **systems-oriented full-stack development and applied AI architectures**.

🎓 **B.Tech 1st Year Student (India)**
💻 **Systems-Oriented Full-Stack Developer** · 🤖 **Applied AI Systems Builder** · 🌍 **Open-Source Contributor**

---

## About Me

I’m a first-year engineering student who builds **production-oriented software systems**, not just demos. I focus on **clean architecture, correctness boundaries, and performance-aware design**, especially in systems that combine AI with real-world constraints.

I’m particularly interested in **hybrid architectures** where:

* deterministic, safety-critical logic is enforced at the systems level (Rust / C / C++)
* higher-level orchestration, APIs, and UX are handled by Python or web frameworks
* AI components are treated as *untrusted but useful* tools, never as sources of truth

I started with **low-level languages early in my B.Tech**, which shaped how I think about memory safety, latency, and verifiability. I prioritize **shipping, testing, and real usage feedback** over theoretical perfection.

---

## Core Strengths

* Designing **hybrid AI systems** with explicit trust boundaries
* Rust-based performance engines integrated into Python and web stacks
* Safe language interop (PyO3, FFI, CXX)
* Backend systems emphasizing **correctness, observability, and scalability**
* Turning experimental ideas into **deployable, maintainable services**

---

## Tech Stack

### Languages

Python · TypeScript · JavaScript · Rust · C++ · C · SQL

### Frontend

React · React Native · Angular

### Backend & Frameworks

Django · FastAPI · Node.js · Express · **Axum (Rust)** · Actix (Rust) · Warp (Rust)

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

**Overview:**
CampusVision is a multi-camera, multi-campus attendance platform designed with a **strict separation between AI inference, system correctness, and API orchestration**.

**Architecture Highlights:**

* All computer-vision logic (face detection, embeddings, vector search) runs in **Rust** for determinism, memory safety, and predictable latency
* **Axum (Rust)** is used as a high-throughput web backend for **heavy, performance-critical workloads** (camera ingestion, inference pipelines, vector queries)
* Django is used strictly for orchestration, authentication, business rules, and REST APIs
* HNSW-based vector search enables low-latency real-time face matching
* Rust modules are fully tested and validated *before* being exposed to any API layer
* Frontend access via React (admin dashboard) and React Native (mobile clients)

**Focus:** Scalability, correctness, and real-world deployment constraints rather than model novelty.

---

### 💰 FinTally — Personal Finance Tracker with AI Insights

**Status:** Active development

**Overview:**
FinTally explores **multi-language backend architectures** and performance-sensitive computation in financial systems.

**Architecture Highlights:**

* Node.js for fast user-facing APIs
* Django for analytics and reporting workflows
* Rust for memory-safe, low-latency financial computations
* C++ modules integrated via FFI for high-performance numerical workloads and legacy compatibility
* Conversational chatbot implemented strictly as a **UX layer**
* LLMs used only for intent parsing and natural-language explanations
* All financial rules, calculations, and validations enforced by deterministic Rust modules
* Chatbot outputs validated against backend invariants before execution

**Key Learnings:** System boundaries, interop costs, and the trade-off between developer velocity and runtime performance.

---

### 📂 Taskflow-Ngnode — AI-Assisted Task Management Platform

**Status:** Complete & deployed

**Features:**

* Rule-based + ML-assisted task scheduling
* Role-based access control and notifications
* AI services isolated behind a FastAPI microservice

**Focus:** Practical ML integration without coupling core business logic to probabilistic components.

---

### 📈 Revenue-AI — Financial Forecasting & EDA Platform

**Status:** Complete & deployed

**Features:**

* Time-series forecasting and exploratory data analysis
* Multiple classical and ML models with comparative evaluation
* Exportable results (CSV, Excel, JSON)
* Secure authentication (JWT + OAuth2)

---

## Learning & Systems Background

### Systems Programming

* Strong foundations in **C, C++, and Rust** from early B.Tech coursework
* Focus on memory management, ownership models, concurrency, and safe interop
* Hands-on experience integrating Rust with Python and C++ in production-style systems

### Machine Learning

* From exploratory notebooks to modular, reusable pipelines
* Emphasis on **deployment readiness, reproducibility, and evaluation**
* Comfortable treating ML as a component within larger systems—not in isolation

---

## Security & Authentication

* JWT-based authentication flows
* OAuth 2.0 (Google)
* Secure token handling and session design

---

## Open Source & Activity

* Active GitHub contributor across full-stack, AI, and systems projects
* Preference for clean code, tests, and long-term maintainability

---

## Connect

📧 **Email:** [agondi982@gmail.com](mailto:agondi982@gmail.com)
📺 **YouTube:** @ag_youtube

---

> *Always building systems that work in practice — not just in theory.*
