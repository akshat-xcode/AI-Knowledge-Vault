# 🧠 AI-Knowledge-Vault

Welcome to the **AI-Knowledge-Vault**! This project is a next-generation AI-powered learning assistant designed to help you interact with your documents, generate flashcards, take quizzes, and retrieve information seamlessly.

## 🚀 Features (MVP Phase)
- **Document Ingestion:** Upload PDFs and extract text efficiently.
- **Smart AI Chat (RAG):** Ask questions directly to your documents. The AI searches via vector embeddings and provides accurate answers with source citations.
- **AI Learning Tools:** Automatically generate flashcards and quizzes from your notes.
- **Premium UI/UX:** A fast, responsive, and visually stunning frontend built with Next.js and Vanilla CSS (Dark Mode & Glassmorphism).
- **Scalable Architecture:** Containerized with Docker, backed by PostgreSQL and `pgvector`.

## 🛠️ Tech Stack
- **Frontend:** Next.js (App Router), React, TypeScript, Vanilla CSS
- **Backend:** Python, FastAPI, LangChain / LlamaIndex
- **Database:** PostgreSQL with `pgvector` (for vector embeddings and auth)
- **Infrastructure:** Docker & Docker Compose

## 📂 Repository Structure
Since we are a collaborative team, the repository is split into independent folders to prevent merge conflicts:

```text
AI-Knowledge-Vault/
│
├── frontend/      # Next.js App (UI & UX)
├── backend/       # FastAPI Server (Logic & APIs)
├── ai/            # Python scripts for LLM testing, PDF Parsing & Embeddings
├── docker/        # Dockerfiles and infrastructure configs
└── docs/          # Architecture diagrams and API documentation
```

## 💻 Getting Started (Team Guide)
Clone this repository and navigate to your respective folder.

### 1. Frontend Setup
```bash
cd frontend
npm install
npm run dev
```
Access the UI at `http://localhost:3000`.

### 2. Backend Setup
```bash
cd backend
python -m venv venv
# activate venv (source venv/bin/activate OR venv\Scripts\activate)
pip install -r requirements.txt
uvicorn main:app --reload
```

### 3. Infrastructure (Database)
```bash
docker-compose up -d
```

## 🤝 Collaboration Rules
- Always work **strictly inside your assigned folder** (`frontend/`, `backend/`, or `ai/`).
- Commit and push your code at the end of every day.
- Do not modify another team member's folder without permission.

---
*Built with ❤️ by an awesome team of 3 named as tyagi,guptaa,sakkk 🔥*
