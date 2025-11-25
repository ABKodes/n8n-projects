# 🚀 Personal n8n AI Projects
> **A collection of custom AI-driven automation workflows I built to solve complex business and productivity challenges.**

![Portfolio Hero Preview](./image.png)

![Total Projects](https://img.shields.io/badge/Projects-3-blue)
![Platform](https://img.shields.io/badge/Platform-n8n-red)
![AI-Powered](https://img.shields.io/badge/Brain-Google%20Gemini%201.5%20Pro-blue)

This repository serves as a showcase of my personal work with **n8n orchestration** and **Google Gemini 1.5 Pro**. My goal was to move beyond simple automation and build enterprise-grade, localized AI solutions that handle real-world data, cultural nuances, and complex RAG (Retrieval-Augmented Generation) patterns.

---

## 📂 The Work I've Done

### 1. 🇪🇹 Ethiopian Enterprise AI Chatbot
**Location:** [`/Company Chatbot`](./Company%20Chatbot/)  
In this project, I focused on **cultural localization**. I built a chatbot specifically for the Ethiopian market, implementing "Kibur" hospitality standards, formal Amharic greetings, and local payment references (Telebirr/CBE).
- **Technical Achievement**: Bridged Google Sheets for dynamic inventory and Gmail for automated order notifications.

### 2. 🤖 Telegram PDF Intellectual Assistant (RAG)
**Location:** [`/Telegram Chat with PDF`](./Telegram%20Chat%20with%20PDF/)  
My objective here was to master **RAG (Retrieval-Augmented Generation)**. I built a system where users can upload PDFs to Telegram and "interview" the documents.
- **Technical Achievement**: Implemented a vector database pipeline using **Pinecone** and Gemini embeddings to provide context-accurate answers.

### 3. 📊 AI Sentiment Analysis Intelligence
**Location:** [`/Sentiment Analysis Bot`](./Sentiment%20Analysis%20Bot/)  
I designed this bot to solve the problem of scaling customer feedback analysis. It classifies Telegram reviews as Positive, Neutral, or Negative.
- **Technical Achievement**: Used structured output parsing to force the AI into returning strict JSON, ensuring the data logs perfectly into analysis spreadsheets.

---

## 🛠 My Technical Toolkit

- **Workflow Orchestration**: n8n
- **Artificial Intelligence**: Google Gemini 1.5 Pro (Vision/Pro models)
- **Vector Search**: Pinecone
- **DevOps**: Docker & Docker Compose
- **Integrations**: Telegram Bot API, Google Sheets, Gmail

---

## 🚀 How to Run My Projects

I have dockerized every project to make deployment seamless. Each bot runs on its own port:

| My Project | Port | Deployment Command |
| :--- | :--- | :--- |
| **Enterprise Chatbot** | `5678` | `cd "Company Chatbot" && docker-compose up -d` |
| **PDF RAG Assistant** | `5679` | `cd "Telegram Chat with PDF" && docker-compose up -d` |
| **Sentiment Analysis** | `5680` | `cd "Sentiment Analysis Bot" && docker-compose up -d` |

---

## 👨‍💻 About the Developer
I am passionate about building AI that actually works for people. Whether it's localized hospitality bots or deep document search, I focus on building stable, professional, and useful software.

*Built with ❤️ by ABKodes*
