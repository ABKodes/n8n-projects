# 🇪🇹 Ethiopian Enterprise AI Chatbot
> **Bridging the gap between Ethiopian Businesses and Customers with AI Excellence.**

![Architecture](https://img.shields.io/badge/Architecture-n8n-red)
![AI Model](https://img.shields.io/badge/Brain-Google%20Gemini%201.5%20Pro-blue)
![Localization](https://img.shields.io/badge/Locale-Ethiopia%20(Amharic/English)-green)
![Status](https://img.shields.io/badge/Status-Production%20Ready-gold)

The **Ethiopian Enterprise AI Chatbot** is a state-of-the-art customer engagement solution specifically engineered for the Ethiopian digital landscape. It combines the reasoning power of **Google Gemini 1.5 Pro** with the flexibility of **n8n** automation to deliver a chatbot that understands not just the language, but the cultural nuances of Ethiopian hospitality.

---

## 🌟 Key Value Propositions

### 🏛 Cultural Intelligence
Built-in awareness of **Ethiopian Hospitality ('Kibur')**. The AI is programmed to use respectful formal Amharic (e.g., *Erswo*, *Tenayistilign*) and navigate cultural expectations with grace.

### � Local Financial Integration
Pre-configured to support **Ethiopian Birr (ETB)** and natively prepared to assist with payments via localized systems like **Telebirr**, **CBE (Commercial Bank of Ethiopia)**, and traditional cash transactions.

### � Dynamic Inventory Management
Utilizes **Google Sheets** as a headless CMS, allowing business owners to update product availability, pricing, and descriptions in real-time without touching a single line of code.

### � Conversational Sales Engine
Beyond just answering questions, the bot is trained to guide users through the sales funnel, capture high-intent leads (Name/Phone), and instantly notify the sales team via **Gmail integration**.

---

## 🛠 Technical Overview

| Component | Technology | Role |
| :--- | :--- | :--- |
| **Orchestration** | n8n | Workflow & Logic Engine |
| **Large Language Model** | Google Gemini 1.5 Pro | Natural Language Processing |
| **Framework** | LangChain AI | Tool-calling & Memory Management |
| **Database** | Google Sheets | Product & Lead Storage |
| **Containerization** | Docker | Environment Virtualization |

---

## 🚀 Deployment Instructions

### Option 1: Docker (Recommended)
The fastest way to get the environment running is using Docker Compose.

1. **Clone the repository** and navigate to the project folder.
2. **Launch the stack**:
   ```bash
   docker-compose up -d
   ```
3. **Access n8n**: Open `http://localhost:5678` in your browser.

### Option 2: Manual n8n Import
1. Install n8n (Desktop or npm).
2. Click **Workflow** > **Import from File...** and select `companyChatbot.json`.

---

## ⚙️ Configuration & Secrets

To activate the AI's full potential, you must configure the following in your n8n instance:

1. **Google Gemini API**:
   - Obtain an API key from [Google AI Studio](https://aistudio.google.com/).
   - Add it to the Gemini node credentials.
2. **Google Sheets Integration**:
   - Replace the Spreadsheet ID in the Google Sheets node with your own.
   - [Template CSV File](products.csv)
3. **Gmail Notifications**:
   - Authenticate your Gmail account.
   - Set the `sendTo` address to your official business email (currently set to `abthevillain@gmail.com`).

---

## 📂 Project Directory
```bash
.
├── companyChatbot.json   # Core n8n Workflow Logic
├── products.csv          # Sample Product Database
├── Dockerfile            # Container configuration
├── docker-compose.yml    # Multi-container orchestration
└── README.md             # Documentation (You are here)
```

---

## 🤝 Contribution & License
This project is open-source. We welcome contributions that improve Amharic NLP prompts, add Telebirr API integrations, or enhance the lead-capture logic.

**Built with ❤️ for Ethiopia.**
