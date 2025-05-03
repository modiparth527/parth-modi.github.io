# 🧠 LangChain Chatbot with Ollama and Google Gemma

A minimal, end-to-end conversational AI web app that uses the **LangChain framework**, **Ollama backend**, and **Google’s Gemma 2B model**. It delivers an interactive chatbot experience with a clean interface built using **Streamlit**.

---

## 🔍 Overview

This project demonstrates how to:

- Integrate **LLMs** (like Gemma 2B) locally via **Ollama**
- Use **LangChain** to manage prompt engineering and response parsing
- Create a user-friendly interface with **Streamlit**
- Optionally connect with **LangSmith** for observability

The core use case is to build intelligent Q&A interfaces with customizable system prompts.

---

## 🎯 Key Features

- ✨ Lightweight and fast local inference with `gemma:2b`
- 🧱 Modular code using LangChain chains and parsers
- 🔧 `.env` driven configuration (ideal for deployment)
- 📊 Optional LangSmith tracing for debugging and monitoring

---

## 🖥️ Demo

![LangChain Chatbot Demo](ezgif-6eded561a97119.gif)

---

## ⚙️ Tech Stack

- **Python**
- **LangChain**
- **Streamlit**
- **Ollama** (LLM backend)
- **Google Gemma 2B**
- **LangSmith** (optional for tracing)
- **dotenv** for config management

---

## 🛠️ Setup Instructions

1. Clone the repo  
2. Install dependencies: `pip install -r requirements.txt`  
3. Set your `.env` variables (`LANGCHAIN_API_KEY`, `LANGCHAIN_PROJECT`)  
4. Run Ollama and download the model:  
   ```bash
   ollama run gemma:2b
   ```
5. Launch the app:  
   ```bash
   streamlit run app.py
   ```

---

## 📁 Project Structure

```
.
├── app.py            # Main Streamlit application
├── .env              # Environment variables
├── demo.gif          # Demo video as GIF
├── requirements.txt  # Dependencies
└── README.md
```

---

## 📌 Why This Project?

This project reflects my passion for practical LLM applications and full-stack ML integration. It’s lightweight, fast, and demonstrates real-world use of modern AI tooling — perfect for solo devs or rapid prototyping in enterprise contexts.

---

## 🔗 Live Demo / GitHub

> 🔗 [GitHub Repository](https://github.com/yourusername/langchain-gemma-chatbot)

---

Let me know if you'd like a deployable version (e.g., on Hugging Face Spaces or Streamlit Community Cloud) for embedding in your portfolio.
