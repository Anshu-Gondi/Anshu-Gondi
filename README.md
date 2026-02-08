# 👋 Hi, I’m Anshu Gondi

> 💼 **Open to internships and remote collaborations** — focused on **systems-oriented full-stack development and applied AI architectures**.

🎓 **B.Tech 1st Year Student (India)**
💻 **Systems-Oriented Full-Stack Developer** · 🤖 **Applied AI Systems Builder** · 🌍 **Open-Source Contributor**

---

## About Me

I’m a first-year engineering student who focuses on **building real, working systems**, not just prototypes or demos. My interest lies at the intersection of **backend systems, performance-aware design, and applied AI**, especially where correctness and real-world constraints matter more than model novelty.

My journey didn’t start with theory-heavy systems design. I began with **Python and Tkinter**, building small desktop applications and learning how software actually breaks when used by real people. From there, I moved into **web development**, building full-stack applications and gradually introducing data-driven and ML-based components.

As I worked across **web development and data/ML projects**, I started noticing the limitations of treating everything as a single monolithic web app. This pushed me toward understanding **system boundaries, performance bottlenecks, and reliability guarantees**, which eventually led me to **C, C++, and Rust**.

Today, I design **hybrid systems** where:

* deterministic and safety-critical logic lives in **Rust / C / C++**
* higher-level orchestration, APIs, and workflows are handled by **Python and web frameworks**
* AI is used as a **tool**, not a source of truth

My learning style is **build-first, theory-later**. In many cases, I’ve implemented systems extensively before learning their formal academic terminology. I actively close that gap by revisiting theory after implementation and using it to refine architecture and design decisions.

---

## Core Strengths

* Designing **hybrid AI systems** with explicit trust and correctness boundaries
* Performance-oriented backend development using **Rust**
* Safe multi-language interop (PyO3, FFI, CXX)
* Backend architectures emphasizing **correctness, observability, and scalability**
* Turning experimental ideas into **deployable, maintainable services**

---

## Tech Stack

### Languages

Python · TypeScript · JavaScript · Rust · C++ · C · SQL

### Frontend

React · React Native · Angular

### Backend & Frameworks

Django · FastAPI · Node.js · Express
**Axum (Rust)** · Actix (Rust) · Warp (Rust)

### Databases & Storage

PostgreSQL · MySQL · MongoDB
**MinIO (S3-compatible object storage for images and media)**

### AI / ML

PyTorch · Scikit-learn · NumPy · Pandas · ONNX Runtime

### Systems & Interop

PyO3 · FFI · CXX · bindgen · OpenCV-rs · hnsw_rs

### DevOps & Tooling

Docker · Git · Linux · CI-oriented development
Cloud deployments (Render, Railway, GCP)

---

## Featured Projects

### 🏫 CampusVision — Real-Time Face-Based Attendance System

**Status:** In active development

**Overview:**
CampusVision is a **real-time, multi-camera attendance system** designed with a strict separation between **AI inference, system correctness, and application logic**.

**Architecture Highlights:**

* All computer-vision pipelines (face detection, embeddings, vector search) run in **Rust** for deterministic behavior, memory safety, and predictable latency
* **Axum (Rust)** handles high-throughput, performance-critical workloads such as camera ingestion and inference pipelines
* **Django** is used for orchestration, authentication, business rules, and REST APIs
* **MinIO** is used as object storage for face images and camera snapshots, avoiding misuse of relational databases for binary data
* HNSW-based vector search enables low-latency real-time face matching
* Rust modules are validated and tested before being exposed to any API layer
* Frontend access via **React (admin dashboard)** and **React Native (mobile clients)**

**Focus:** Practical deployment, scalability, and correctness under real-world conditions.

---

### 💰 FinTally — Personal Finance Tracker with AI Insights

**Status:** Active development

**Overview:**
FinTally explores **multi-language backend architectures** and correctness-sensitive financial computation.

**Architecture Highlights:**

* Node.js for fast user-facing APIs
* Django for analytics and reporting workflows
* Rust for deterministic, low-latency financial calculations
* C++ modules integrated via FFI for high-performance numerical workloads
* Conversational chatbot used strictly as a **UX layer**
* LLMs limited to intent parsing and explanations
* All financial rules enforced by deterministic backend logic
* AI outputs validated against system invariants before execution

**Key Learnings:** Interop costs, system boundaries, and performance vs. developer velocity trade-offs.

---

### 📂 Taskflow-Ngnode — AI-Assisted Task Management Platform

**Status:** Complete & deployed

**Highlights:**

* Rule-based core with ML-assisted task prioritization
* Role-based access control and notifications
* AI isolated behind a FastAPI microservice

**Focus:** Integrating ML without coupling business logic to probabilistic behavior.

---

### 📈 Revenue-AI — Financial Forecasting & EDA Platform

**Status:** Complete & deployed

**Highlights:**

* Time-series forecasting and exploratory data analysis
* Multiple classical and ML models with comparative evaluation
* Exportable results (CSV, Excel, JSON)
* Secure authentication (JWT + OAuth2)

---

## Learning & Systems Background

### Systems Programming

* Hands-on experience with **C, C++, and Rust**
* Focus on memory safety, ownership, concurrency, and FFI
* Practical integration of Rust with Python and C++ in real systems

### Machine Learning

* From exploratory notebooks to modular pipelines
* Emphasis on **deployment readiness and reproducibility**
* ML treated as one component within larger systems

---

## Security & Authentication

* JWT-based authentication flows
* OAuth 2.0 (Google)
* Secure token handling and session design

---

## Open Source & Activity

* Active GitHub contributor across full-stack, AI, and systems projects
* Strong preference for clean code, tests, and long-term maintainability

---

## Connect

📧 **Email:** [agondi982@gmail.com](mailto:agondi982@gmail.com)
📺 **YouTube:** @ag_youtube

---

> *Focused on building systems that work in practice — and then understanding the theory behind them.*

---
