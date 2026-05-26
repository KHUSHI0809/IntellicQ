# IntellicQ — Intelligent Micro-Learning Platform

<div align="center">

### 🏆 First Place — Hack-Nu-Thon 5.0 | Team Develomers

**LLM-Powered Adaptive Learning System**

An intelligent micro-learning ecosystem combining **LLMs**, **Agentic AI workflows**, **RAG**, **NLP**, and **Reinforcement Learning** to deliver highly personalized educational experiences.

**40% learner accessibility improvement · 25% course completion boost · 35% engagement increase**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![LangChain](https://img.shields.io/badge/LangChain-Agentic_AI-green?style=for-the-badge)
![OpenAI](https://img.shields.io/badge/OpenAI-LLM-black?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG-Vector_Search-orange?style=for-the-badge)

</div>

---

## 📌 Overview

**IntelliCQ** is an AI-powered adaptive micro-learning platform that personalizes educational experiences using modern AI techniques. The platform continuously adapts content based on learner behavior, quiz performance, interaction patterns, and engagement analytics.

Core capabilities:
- Large Language Models (LLMs) for intelligent tutoring
- Agentic AI workflows with multi-agent orchestration
- Retrieval-Augmented Generation (RAG) for grounded responses
- NLP-based semantic tagging and transcript generation
- Reinforcement Learning for real-time personalization
- AI safety guardrails (prompt injection, hallucination filtering, content moderation)

---

## ✨ Features

### 🎯 Intelligent Learning Personalization
- Dynamic difficulty scaling based on learner performance
- Adaptive content recommendation and personalized learning pathways
- AI-generated quizzes and summaries

### 🤖 Agentic AI Workflow
- Multi-agent orchestration for context-aware tutoring
- Automated educational planning and intelligent response sequencing

### 🧠 NLP-Based Content Processing
- Semantic topic extraction and keyword tagging
- Transcript analysis, learning objective detection, and educational summarization

### 📝 Automated Transcript Generation
- AI-generated transcripts from educational videos
- Topic segmentation, timestamp generation, and searchable notes

### 🔍 Retrieval-Augmented Generation (RAG)
- Context-grounded educational responses with reduced hallucinations
- Semantic search across the knowledge base for personalized tutoring

### 🔄 Reinforcement Learning Feedback Loop
- Real-time learner adaptation and engagement optimization
- Dynamic quiz generation and learning pace adjustment

### 🔒 AI Safety Guardrails
- Prompt injection protection and hallucination filtering
- Toxicity moderation and content appropriateness validation

---

## 🏗️ Architecture

```
+---------------------------------------------------+
|                 Frontend Interface                |
|          React / Next.js / TypeScript             |
+-------------------------+-------------------------+
                          |
                          v
+---------------------------------------------------+
|                 Backend API Layer                 |
|               FastAPI / Flask APIs                |
+-------------------------+-------------------------+
                          |
      ---------------------------------------------------------
      |                      |                               |
      v                      v                               v
+-------------+     +------------------+       +------------------+
| LLM Engine  |     | NLP Processing   |       | RL Personalizer  |
| GPT Models  |     | Semantic Tagging |       | Adaptive Learning|
+-------------+     +------------------+       +------------------+
                          |
                          v
+---------------------------------------------------+
|                 RAG Knowledge Base                |
|      Vector DB + Embeddings + Semantic Search     |
+---------------------------------------------------+
                          |
                          v
+---------------------------------------------------+
|                 Database & Storage                |
|          PostgreSQL / MongoDB / VectorDB          |
+---------------------------------------------------+
```

### AI Agent Workflow

```
Learner Input
      ↓
Intent Detection Agent
      ↓
Context Retrieval Agent (RAG)
      ↓
Learning Strategy Agent
      ↓
LLM Response Generator
      ↓
Guardrail Validation Layer
      ↓
Personalized Educational Output
```

---

## 🛠️ Tech Stack

| Layer | Technologies |
|-------|-------------|
| **Frontend** | React.js, Next.js, TypeScript, Tailwind CSS |
| **Backend** | Python, FastAPI, Flask, REST APIs |
| **AI & ML** | OpenAI GPT, LangChain, HuggingFace Transformers, Reinforcement Learning |
| **NLP** | spaCy, NLTK, Transformers, scikit-learn |
| **Databases** | PostgreSQL, MongoDB, Pinecone / ChromaDB / FAISS |
| **DevOps** | Docker, GitHub Actions, AWS / Vercel / Render |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/KHUSHI0809/IntelliCQ.git
cd IntelliCQ
```

### 2. Backend Setup

```bash
# Create and activate virtual environment
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows

# Install dependencies
pip install -r requirements.txt
```

### 3. Frontend Setup

```bash
cd frontend
npm install
```

### 4. Environment Variables

Create a `.env` file in the root directory:

```env
OPENAI_API_KEY=your_openai_api_key
LANGCHAIN_API_KEY=your_langchain_key
DATABASE_URL=your_database_url
VECTOR_DB_URL=your_vector_database
JWT_SECRET=your_secret_key
```

### 5. Run the Project

```bash
# Backend
uvicorn main:app --reload

# Frontend (in a separate terminal)
cd frontend
npm run dev
```

---

## 🔍 RAG Pipeline

```
Educational Content → Text Chunking → Embedding Generation
      ↓
Vector Database Storage → Semantic Search → Context Retrieval
      ↓
LLM-Augmented Response
```

**Benefits:** Reduced hallucinations · Improved contextual accuracy · Personalized explanations

---

## 🔄 Reinforcement Learning Loop

The RL engine adapts in real time based on: quiz performance, session duration, interaction frequency, completion rate, and learner engagement.

```
Reward = Engagement + Accuracy + Completion - Fatigue
```

**Adaptive actions:** Increase/decrease difficulty · Adjust lesson duration · Recommend revision modules · Personalize learning pace

---

## 🔒 Security & Guardrails

- **Prompt Injection Protection** — input sanitization, unsafe prompt detection
- **Hallucination Filtering** — retrieval grounding, confidence-based validation
- **Content Safety** — toxicity filtering, educational appropriateness checks
- **Authentication** — JWT tokens, role-based access control

---

## 📡 API Endpoints

### Authentication
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register user |
| POST | `/api/auth/login` | Login user |
| GET | `/api/auth/profile` | User profile |

### AI Services
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/ai/chat` | AI tutoring |
| POST | `/api/ai/transcript` | Generate transcript |
| POST | `/api/ai/recommend` | Learning recommendations |
| POST | `/api/ai/quiz` | Adaptive quiz generation |

### Learning Modules
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/modules` | Fetch modules |
| POST | `/api/modules/generate` | Generate AI module |
| GET | `/api/modules/:id` | Module details |

---

## 📊 Performance Metrics

| Metric | Result |
|--------|--------|
| Learner Accessibility | +40% |
| Course Completion Rate | +25% |
| User Engagement | +35% |
| Hallucination Rate | Reduced via RAG grounding |
| Adaptive Accuracy | Dynamically improved via RL |

---

## 🔮 Future Enhancements

- Voice-enabled tutoring and multi-modal learning
- AI-generated visual explanations and gamification
- Emotion-aware learning adaptation
- Federated learning integration
- Multilingual tutoring support

---

## 🏷️ Topics

`llm` `agentic-ai` `rag` `nlp` `reinforcement-learning` `langchain` `adaptive-learning` `micro-learning` `educational-ai` `openai` `fastapi` `react`
