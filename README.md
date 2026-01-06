# 👋 Hi, I'm **Anshu Gondi**

> 💼 **Open to internships or remote collaborations – focused on full-stack + AI systems.**

🎓 **1st Semester B.Tech Student (India)**  
💻 **Full-Stack Developer** | 🤖 **AI & Data Science Enthusiast** | 🌍 **Open Source Builder**

---

> “Driven by curiosity. Obsessed with innovation. Building the future—one project at a time.”

I’m a passionate engineering student turning ideas into impact through code.  
From **AI-powered finance systems** to **intelligent productivity tools**, I love building at the intersection of **creativity, data, and engineering**.

---

## 🚀 Currently Exploring

* **Full-Stack Development:** MERN stack · Django · Angular · FastAPI
* **AI / ML Systems:** PyTorch · Scikit-learn · Scalable ML pipelines
* **Cloud & Deployments:** Docker · Render · Vercel · Railway
* **Systems Thinking:** Hybrid backends · service orchestration · Rust extensions *(in progress)*

💡 My learning path: notebooks → hybrid workflows → production-ready systems.

---

## 🧠 New Milestone: C Language Conquered!

In just **11 days**, I explored and built multiple projects in **C**, mastering core concepts from beginner to advanced level.  
Check out the repo 👇  
🔗 [C-Language-Project-beginner-to-advanced-level](https://github.com/Anshu-Gondi/C-Language-Project-beginner-to-advanced-level)

---

## 🧠 New Milestone: Rust Mastery (FFI & Web Backends)

In **2.5 months**, I completed a focused learning and project sprint on **Rust**, achieving:

* Mastery of Rust fundamentals and advanced patterns
* Building and consuming Rust libraries via **FFI** (integrating with C and other languages)
* Developing web backends and services using Rust web frameworks (e.g., Actix, Warp)
* Production-oriented practices: memory-safe, high-performance modules for hybrid backends

This milestone helped me integrate Rust modules into existing projects and leverage its performance and safety for backend services.

---

## 🧠 New Milestone: C++ Mastery (OOP, STL & Interop with Rust)

After solidifying my Rust expertise, I dove into **C++** to deepen my understanding of systems programming and enable powerful interop in hybrid backends:

* Mastered modern C++ (11/14/17/20/23 features), OOP principles, templates, STL containers & algorithms
* Built high-performance projects using RAII, smart pointers, multithreading, and fine-grained memory control
* Focused heavily on **C++/Rust interop** via FFI, CXX, and bindgen – seamless integration of C++ modules into Rust codebases and vice versa
* Emphasis on zero-cost abstractions, idiomatic patterns, and safe bridging between C++ and Rust for real-world hybrid systems

This milestone allows me to selectively use C++ for legacy integration, performance-critical libraries, or GPU/parallel computing while keeping the safety guarantees of Rust in production services.

---

## 🧰 Tech Stack

**Languages:**  
Python · JavaScript · TypeScript · C · Rust · **C++** · SQL · PostgreSQL · MySQL

**Frameworks & Libraries:**  
Django · Node.js · Express · React · Angular · FastAPI

**Databases:**  
MongoDB · PostgreSQL · MySQL

**AI / ML:**  
PyTorch · NumPy · Pandas · Scikit-learn

**Tools & Platforms:**  
Docker · Git · Google Cloud · Render · Vercel

---

## 🌟 Featured Projects

### 💰 FinTally – Money Tracker App + AI Insights

Status: Upgrading

🧩 **Tech:** React + Node.js + Django + MongoDB + Rust  
🧠 **Hybrid backend**: Node.js for fast APIs, Django for data analytics & insights, and Rust modules for high-performance, low-memory operations.

**Highlights:**
* Smart finance manager with recurring transactions, PDF exports, and categorized analytics
* Real-time insights: daily, weekly, and lifetime summaries via Django backend
* **Hybrid architecture**: Node.js + Django + Rust for seamless data sync, performance boosting, and efficient memory usage
* Rust modules integrated for critical paths (e.g. data processing, computation-heavy tasks)
* Pagination & infinite scroll for smooth UX
* **AI Chatbot:** planned integration for smart financial suggestions *(under development)*

---

### 🏫 CampusVision — Face-based Attendance & Verification *(In building)*

**Status:** In building  

**TL;DR:**  
A real-time, CCTV-based campus attendance system powered by a fully Rust-built face recognition and vector search engine (ONNX + HNSW), integrated with Django via PyO3.

A campus-level attendance and verification system that blends teacher-managed class data with automated face verification using CCTV.

### 🧩 Tech Stack & Core Architecture

- **Backend:** Django + Django REST Framework  
- **Database:** PostgreSQL  
- **Frontend:** React.js  

**Vision, Vector Search & Intelligence Layer (Fully Rust-based)**
- **Rust Core Engine** — High-performance, memory-safe processing
- **PyO3** — Rust ↔ Python bindings for seamless Django integration
- **ONNX Runtime (Rust)** — Inference for face embedding models
- **tch (PyTorch for Rust)** — Custom tensor operations & experimentation
- **opencv-rs** — CCTV frame ingestion, face detection & preprocessing
- **hnsw_rs** — Approximate Nearest Neighbor (ANN) vector search
- **Vector Storage:** Face embeddings stored as high-dimensional vectors

**Architecture Style**
- Django handles APIs, authentication, analytics, and orchestration  
- Rust handles vision, embeddings, vector search, and scheduling logic  
- Python interacts with Rust modules exclusively via **PyO3**

### 🔍 How It Works

* Teachers or school/college units enter branch and class details through a simple interface (teacher part remains manual and unchanged).
* Students register once; face embeddings are generated using ONNX models running inside Rust.
* CCTV streams are continuously processed using **opencv-rs**.
* Detected faces are converted into embeddings and matched using **HNSW-based vector search**.
* Manual attendance outside campus is tracked and later reconciled once CCTV verification confirms physical presence.
* Django dashboards display attendance status, analytics, and reports.

### 🧠 Vector Search & Scheduling Algorithms

**Graph-based (Primary – Real-time Matching)**
- **HNSW (Hierarchical Navigable Small World Graph)**
- Implemented using **`hnsw_rs`**
- Used for identity verification and low-latency vector similarity search

**Tree-based (Secondary – Scheduling & Coordination)**
- **KD-Tree / Ball Tree–style partitioning**
- Used for attendance scheduling, zone-wise verification, and time-based reconciliation

**Hybrid Strategy**
- Graph-based search → Fast identity matching  
- Tree-based logic → Structured scheduling and conflict resolution  

### 🎯 Design Focus

- Real-time, low-latency verification
- Fully Rust-driven vision & vector intelligence
- Safe Python integration via PyO3
- Scalable across multiple campuses and CCTV feeds
- Clear separation between UI, orchestration, and intelligence layers

This project is currently in active development and is being designed to scale across colleges and schools.

---

### 📂 Taskflow-Ngnode – AI-Powered Task Management

Status: Complete

🧠 **Purpose:** Automate daily planning with intelligent scheduling.

**Core Features:**

* **AI Scheduler:** Rule-based + ML hybrid (MiniBatchKMeans, IsolationForest, PyTorch custom models)
* **Team Roles:** Admin / Editor / Viewer with email notifications via Resend API
* **Design Inspirations:** *Among Us* (team join flow) & *Clash of Clans* (role hierarchy)
* Auto-load fallback for pretrained models
* Adaptive ML scheduling with real-time rule updates

**Stack:**  
Angular · Node.js · FastAPI (AI microservice)

---

### 📈 Revenue-AI – Financial Forecasting & EDA Platform

Status: Complete

**Tech:** Django + DRF + PyTorch + Node.js Proxy + PostgreSQL

**Capabilities:**

* End-to-end EDA and ML forecasting workflows
* Interactive model selection (Linear, DecisionTree, XGB, LGBM, RandomForest)
* Multi-export support: JSON · CSV · Excel · Image
* Modular ML design: deploy-ready via Render / Railway / Vercel
* Integrated Auth (JWT + OAuth2.0)

---

## 🧪 Data Science Journey

From small notebooks to production-grade ML pipelines 🚀

* [**Data-Science-Projects**](https://github.com/Anshu-Gondi/Data-Science-Projects) – EDA, visualizations, starter ML
* [**Data-Science-Project-Alternate**](https://github.com/Anshu-Gondi/Data-Science-Project-Alternate) – modular scripts, configs, and reusable ML pipelines

Next stages:
✔ Modular data → modeling → evaluation design
✔ Parallelized training
✔ Documentation & reproducibility

---

## 🔐 OAuth2.0 & Authentication Work

* Secure login with **Google OAuth2.0**
* **JWT** authentication in Node.js + Django apps
* Refresh token and session management systems

---

## 📊 GitHub Activity

🔹 Active contributor across full-stack, AI, and systems projects  
🔹 Consistent project-based commits  
🔹 Focus on production-ready repositories over vanity metrics

---

## 🌐 Connect with Me

* 📺 YouTube: [@ag_youtube](https://youtube.com/@ag_youtube)
* 📧 Email: [agondi982@gmail.com](mailto:agondi982@gmail.com)

---

> ✨ “Always building, always learning. From concept to code to creation.” 🚀
