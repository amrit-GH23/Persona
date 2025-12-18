# 🧠 Political Persona Chat API (FastAPI + Gemini)

A FastAPI-based backend that simulates conversational personas of **Narendra Modi ji** and **Rahul Gandhi ji** using Google’s **Gemini API (OpenAI-compatible endpoint)**.

⚠️ **Reality check:**  
This project is **demo / experimental only**. It is **not production-ready** and **cannot be reliably hosted** on Gemini’s free tier due to extremely low and shared request limits.

---

## 🚀 Features

- Persona-driven responses using strong system prompts
- Two supported personas:
  - **Modiji** – Authoritative, nationalist, governance-focused
  - **Rahulji** – Conversational, critical, inequality-focused
- REST API built with FastAPI
- Simple persona switching via request payload
- Uses Gemini through OpenAI-compatible SDK

---

## 🧩 Tech Stack

- Python 3.10+
- FastAPI
- Pydantic
- Google Gemini API
- OpenAI Python SDK (compatibility mode)
- python-dotenv

---

## 🔑 Environment Variables

Create a `.env` file in the project root:

env
- GEMINI_API_KEY=your_google_gemini_api_key_here


⚠️ Once the quota is exhausted, requests will fail.
This is a Gemini limitation, not a code issue.

📦 Installation
- git clone https://github.com/amrit-GH23/Persona
- cd persona

# Windows:
- python -m venv venv
- venv\Scripts\activate

- pip install -r requirements.txt

▶️ Running the Server
- fastapi dev main.py

**Server URL**:
- http://127.0.0.1:8000

**Swagger Docs**:
- http://127.0.0.1:8000/docs

**🔗 API Endpoint**
- POST /chat
- Request Body
- {
  "message": "What is your vision for India?",
  "persona": "modiji"
  }

- Supported personas
  - modiji
  - rahulji

- Response
- {
  "response": "Persona-based generated reply"
 }


## 🧑‍💻 Author
- Amrit Kumar
- Purpose: Learning, experimentation, and understanding LLM persona design.

