---
title: "LangChain Chatbot with Ollama and Google Gemma"
excerpt: "An intelligent Q&A chatbot using LangChain, Ollama, and the Google Gemma 2B model.<br/><br/><img src='/parth-modi.github.io/images/ezgif-6eded561a97119.gif'>"
collection: portfolio
---

## Overview
<div style="text-align: justify;">
This project showcases an interactive chatbot built using <strong>LangChain</strong>, <strong>Ollama</strong>, and <strong>Google’s Gemma 2B</strong> large language model. The application allows users to ask natural language questions and receive AI-generated responses with real-time feedback. It demonstrates practical integration of LLMs using a modular and observable architecture.
</div>

## Table of Contents
- [Introduction](#introduction)
- [System Architecture](#system-architecture)
- [Demo](#demo)
- [Technologies Used](#technologies-used)

## Introduction
The chatbot application uses the `gemma:2b` model served locally via Ollama and orchestrated using LangChain. The user interface is built in Streamlit, and optional observability is enabled using LangSmith. This project is an example of how lightweight LLMs can be used efficiently in production-ready apps.

## System Architecture

### Prompt Engineering & LangChain
- A predefined system message and user query template are used for consistent interactions.
- The LangChain framework handles chaining and output parsing.

### Ollama LLM Backend
- The Gemma 2B model is served locally through Ollama for low-latency inference.
- This avoids dependency on external APIs for inference.

### Streamlit Frontend
- A lightweight Streamlit interface is provided for easy interaction.
- Users can type questions and get answers in real time.

![Architecture Diagram](/parth-modi.github.io/images/langchain_architecture.png)
<p align="center"><em>Figure 1: System Architecture Overview</em></p>

## Demo
![LangChain Chatbot Demo](/parth-modi.github.io/images/ezgif-6eded561a97119.gif)
<p align="center"><em>Figure 2: Real-time interaction with the chatbot</em></p>

## Technologies Used

- **LangChain** – for prompt orchestration and chaining
- **Ollama** – to serve Gemma 2B LLM locally
- **Google Gemma 2B** – open-source LLM for inference
- **Streamlit** – frontend interface
- **LangSmith** – optional observability for debugging chains
- **Python-dotenv** – for secure environment configuration

---

> 💡 This project highlights the power of local LLMs for real-world use cases and the potential of open-source tools in delivering high-quality AI applications.

