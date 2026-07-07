# 🧠 AI-Knowledge-Vault

> **An intelligent, hyper-personalized AI learning assistant that transforms static documents into interactive knowledge bases.**

Welcome to **AI-Knowledge-Vault**. This repository houses the core architecture for a next-generation AI platform designed to seamlessly ingest documents, generate automated flashcards and quizzes, and provide context-aware answers using advanced Retrieval-Augmented Generation (RAG).

---

## 🎯 Project Vision & MVP Scope
The primary objective of the MVP is to establish a robust, high-performance foundation capable of processing PDFs and delivering accurate, cited answers at lightning speed.

- **Intelligent Ingestion:** Rapid PDF parsing and text extraction.
- **Vector Search & RAG:** High-dimensional semantic search using embedded knowledge graphs.
- **Cognitive Tools:** Automated flashcard generation and quiz evaluations.
- **Aesthetic Excellence:** A highly responsive, glassmorphism-inspired UI designed for deep focus.
- **Containerized Infrastructure:** Seamless deployment using Docker and PostgreSQL.

---

## 👥 Team Architecture & Role Split

This project is built using a highly decoupled micro-architecture, maintained by a specialized team of 3 developers. The work is explicitly split as follows:

### 🎨 1. Frontend Engineering (UI/UX)
**Tech Stack:** Next.js (App Router), React, TypeScript, Vanilla CSS
**Responsibilities:**
- Designing a premium, Dark Mode + Glassmorphism user interface.
- Managing client-side state, API integrations, and routing.
- Ensuring a fluid, micro-animated user experience.
*Directory:* `/frontend`

### ⚙️ 2. Backend Engineering (Core API)
**Tech Stack:** Python, FastAPI, JWT Auth
**Responsibilities:**
- Building highly concurrent, asynchronous REST APIs.
- Managing User Authentication, session states, and Conversation History.
- Orchestrating the data flow between the client and the AI models.
*Directory:* `/backend`

### 🤖 3. AI/ML & Infrastructure (Data Pipeline)
**Tech Stack:** LangChain, LlamaIndex, PostgreSQL (`pgvector`), Docker
**Responsibilities:**
- Implementing the RAG pipeline (Chunking, Embeddings, Vector Search).
- Writing scripts for deep PDF parsing and prompt engineering.
- Managing the database infrastructure and Docker containerization.
*Directories:* `/ai`, `/docker`

---

## 🚀 Getting Started (Local Development)

To avoid merge conflicts and preserve the micro-architecture, **only run the setup for your assigned role.**

### Frontend Node Setup
```bash
cd frontend
npm install
npm run dev
```

### Backend API Setup
```bash
cd backend
python -m venv venv
# Activate venv (source venv/bin/activate OR venv\Scripts\activate)
pip install -r requirements.txt
uvicorn main:app --reload
```

### Database & AI Infrastructure
```bash
docker-compose up -d
```

---
*Architected with precision and passion.*
