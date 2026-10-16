# ✈️ Telegram AI Support Agent - Luxury on the GO

An automated, intelligent customer support agent designed specifically for the travel agency **"Luxury on the GO"**. Built using **n8n**, **LangChain Agent nodes**, and **Groq's ultra-fast Llama 3.3 model**, this workflow instantly answers customer questions regarding visa requirements, tour packages, pricing, office hours, and booking procedures via Telegram.

---

## 🏗️ Workflow Architecture

The workflow consists of four core n8n nodes working seamlessly together:

1. **Telegram Trigger**: Listens for incoming messages (`message` updates) sent to your Telegram bot.
2. **AI Agent (LangChain)**: Processes the incoming text prompt using a specialized system persona and conversational logic.
3. **Groq Chat Model**: Leverages the high-speed `llama-3.3-70b-versatile` model to generate accurate and context-aware responses[cite: 1].
4. **Send a text message (Telegram)**: Delivers the AI's final formatted response directly back to the correct Telegram chat ID[cite: 1].

---

## 🤖 Agent Persona & Guidelines

The agent is pre-configured with a specialized system prompt tailored for **Luxury on the GO**[cite: 1]:

* **Core Domain Focus**: Visa requirements, tour packages, office hours, pricing, and booking procedures[cite: 1].
* **Behavioral Rules**:
  * Always maintain a polite, warm, and professional tone[cite: 1].
  * Ask clear follow-up questions if critical details are missing (e.g., asking for a destination country when queried about visas)[cite: 1].
  * Politely decline and redirect off-topic inquiries back to travel services[cite: 1].
  * Keep replies concise and readable for mobile chat apps[cite: 1].
  * Avoid fabricating exact prices or strict visa rules without real data—offering general guidance and advising confirmation with a human agent when necessary[cite: 1].

---

## 📁 Repository Structure

```text
.
├── workflows/
│   └── Assignment 1.json        # Main n8n workflow export file
└── README.md                    # Project documentation
