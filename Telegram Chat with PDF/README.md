# 🤖 Telegram PDF Intellectual Assistant (RAG)
> **Turn your Telegram into a smart knowledge base with PDF-powered AI.**

![n8n](https://img.shields.io/badge/Orchestration-n8n-red)
![Gemini](https://img.shields.io/badge/AI-Google%20Gemini%201.5%20Pro-blue)
![VectorDB](https://img.shields.io/badge/Search-Pinecone%20(RAG)-green)
![Status](https://img.shields.io/badge/Type-Knowledge%20Base-gold)

The **Telegram PDF Intellectual Assistant** is a Retrieval-Augmented Generation (RAG) solution that allows users to upload PDF documents via Telegram and immediately "chat" with their content. Using **Google Gemini 1.5 Pro** and **Pinecone**, the bot provides precise, context-aware answers directly extracted from your documents.

---

## 🚀 Core Functionalities

### 📂 Dynamic PDF Ingestion
Directly upload PDF files in a Telegram chat. The bot automatically:
1.  **Extracts text** using the Default Data Loader.
2.  **Splits content** into intelligent chunks with Recursive Text Splitting.
3.  **Embeds** the knowledge into a high-dimensional vector store (Pinecone).

### 💬 Intelligent Retrieval-Augmented Chat (RAG)
Once a document is uploaded, you can ask questions like:
- *"What is the main argument in section 4?"*
- *"Summarize the financial projections for 2026."*
- *"Does this document mention Ethiopian Telebirr integration?"*

The bot retrieves the most relevant snippets from your PDFs and uses Gemini to formulate a natural response.

### ⚡ Powering the Brain: Google Gemini
This workflow has been migrated to use **Google Gemini 1.5 Pro** for both LLM responses and high-performance embeddings, ensuring the highest level of reasoning and accuracy.

---

## 🛠 Tech Stack

- **n8n**: The glue that connects Telegram, PDF processing, and AI logic.
- **Google Gemini 1.5 Pro**: Advanced reasoning and document understanding.
- **Pinecone**: High-performance vector database for instant document retrieval.
- **Telegram Bot API**: The interface for user interaction.

---

## 📦 Setup & Installation

### Option 1: Docker (Recommended)
The fastest way to get the environment running.

1.  **Launch the stack**:
    ```bash
    docker-compose up -d
    ```
2.  **Access n8n**: Open `http://localhost:5679` in your browser.

### Option 2: Manual n8n Import
1.  Navigate to your n8n dashboard.
2.  Click **Workflows** > **Import from File...** and select `telegramChatWithPDF.json`.
3.  **Configure Credentials**: Open the Gemini, Telegram, and Pinecone nodes and add your credentials.

### 3. Pinecone Configuration
- Ensure your Pinecone index is named **`telegram`** or update the name inside the `Pinecone Vector Store` nodes in n8n.

---

## 📂 Project Directory
```bash
.
├── telegramChatWithPDF.json  # The RAG Orchestration Workflow
├── Dockerfile                # Container configuration
├── docker-compose.yml        # Multi-container orchestration
└── README.md                 # Technical Documentation
```

---

## 🌍 Strategic Advantage for Ethiopia
This tool is perfect for:
- **Legal Professionals**: Instantly search through long Ethiopian proclamations.
- **Students**: Chat with textbooks and lecture notes in Amharic or English.
- **Researchers**: Rapidly summarize local reports and data files.

---
*Empowering Ethiopian knowledge workers with AI.*
