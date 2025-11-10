# 📊 AI Sentiment Analysis Intelligence
> **Real-time customer feedback classification powered by Google Gemini 1.5 Pro.**

![n8n](https://img.shields.io/badge/Logic-n8n-red)
![Gemini](https://img.shields.io/badge/Sentiment-Google%20Gemini%201.5%20Pro-blue)
![Sheets](https://img.shields.io/badge/Database-Google%20Sheets-green)
![Telegram](https://img.shields.io/badge/Input-Telegram--Trigger-blue)

The **AI Sentiment Analysis Intelligence** bot is a sophisticated solution designed to monitor customer feedback in real-time via Telegram. It automatically classifies reviews into **Positive**, **Neutral**, or **Negative** categories and logs the structured data directly into Google Sheets for operational analysis.

---

## 🎯 Strategic Value
- **Immediate Response**: Identify negative sentiment the moment it happens.
- **Data-Driven Insights**: Build a historical database of customer reviews.
- **Structured Precision**: Uses Gemini 1.5 Pro's advanced reasoning to understand nuanced human emotions accurately.

---

## 🚀 Key Features

### 📨 Telegram Integration
- Listens for incoming messages from users.
- Connects directly via the Telegram API for low-latency triggers.

### 🧠 Sentiment Brain (Gemini 1.5 Pro)
- **Advanced Classification**: Goes beyond simple keyword matching to understand context.
- **Strict JSON Output**: Ensures data integrity by forcing the AI to output machine-readable formats.

### 📈 Automated Reporting
- Appends every review, user ID, and sentiment label to a centralized **Google Sheet**.
- Ready for visualization in tools like Looker Studio or Excel.

---

## 🛠 Tech Stack
- **n8n**: Workflow automation and orchestration.
- **Google Gemini 1.5 Pro**: The cutting-edge LLM for sentiment classification.
- **Google Sheets**: Reliable, accessible storage for review data.
- **Telegram Bot API**: High-engagement interface for collecting reviews.

---

## 📦 Setup & Installation

### Option 1: Docker (Fastest)
1. **Launch the bot**:
   ```bash
   docker-compose up -d
   ```
2. **Access n8n**: Open `http://localhost:5680`.

### Option 2: Manual Workflow Import
1. Import `sentimentAnalysisBot.json` into your n8n instance.
2. Configure **Google Gemini**, **Telegram**, and **Google Sheets** credentials.
3. Activate the workflow.

---

## 📂 Project Structure
```bash
.
├── sentimentAnalysisBot.json  # The core n8n automation logic
├── Dockerfile                 # Container image definition
├── docker-compose.yml         # Deployment orchestration
└── README.md                  # Professional documentation
```

---
*Transforming customer feedback into actionable business intelligence.*
