# Perplexity 2.0 – AI Chat Assistant

A modern, responsive AI chat interface with integrated web search functionality. Perplexity 2.0 provides a clean UI similar to Perplexity.ai, combining conversational AI with real-time search capabilities.

---

## ✨ Features

* Real-time AI Responses (streaming)
* Integrated Web Search (Tavily API)
* Conversation Memory
* Search Process Transparency
* Responsive UI

---

## 🏗️ Architecture

Perplexity 2.0 follows a client-server architecture:

### Client (Next.js + React)

* Modern React application built with Next.js
* Real-time streaming using Server-Sent Events (SSE)
* Components for chat UI and interaction

### Server (FastAPI)

* Python backend using FastAPI
* LLM API integration for response generation
* Tavily API integration for web search
* Streaming responses using SSE

---

## 🚀 Getting Started

### Prerequisites

* Node.js 18+
* Python 3.10+
* OpenAI API Key
* Tavily API Key

---

## ⚙️ Installation

### 1. Clone Repository

```bash
git clone https://github.com/AquibAslam1/Perplexity-2.0-AI-Chat-Assistant
cd perplexity_2.0
```

### 2. Setup Backend

```bash
cd server
python -m venv venv
venv\Scripts\activate   # Windows
pip install -r requirements.txt
```

Create `.env` file:

```
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key
```

---

### 3. Setup Frontend

```bash
cd ../client
npm install
```

---

## ▶️ Run Application

### Start Backend

```bash
cd server
uvicorn app:app --reload
```

### Start Frontend

```bash
cd client
npm run dev
```

👉 Open: http://localhost:3000

---

## 🔍 How It Works

1. User sends a message
2. Backend processes input using LLM
3. If needed, web search is triggered
4. Tavily API returns relevant results
5. LLM generates final response
6. Response is streamed to UI

---

## 🛠 Tech Stack

* Frontend: React (Next.js)
* Backend: FastAPI
* AI: LLM API Integration
* Search: Tavily API

---

## 📝 License

MIT License

---

## 🙏 Acknowledgments

* Inspired by Perplexity AI
* Built using Next.js, React, FastAPI
* Powered by OpenAI & Tavily API
