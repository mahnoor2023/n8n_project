# 🤖 Book Inventory Chat Bot (n8n & Airtable AI Assistant)

An intelligent, self-hosted n8n workflow that allows users to interact with and update an Airtable book inventory database using natural language chat commands powered by the Groq API.

## 🚀 Features
* **Natural Language Processing:** Uses an AI Agent with Groq LLM (`qwen/qwen3.8-27b`) to understand user chat prompts[cite: 6].
* **Airtable Integration:** Seamlessly searches and updates inventory records (such as book titles, authors, and quantities) in real-time.
* **Data Type Validation:** Handles strict schema mapping, ensuring numeric fields (like "Quantity on Hand") receive proper integer values.
* **Chat Memory:** Retains conversational context using n8n's memory buffer window.

## 🛠️️ Tech Stack
* **Workflow Automation:** n8n (Self-hosted via Docker)[cite: 1]
* **AI Engine:** Groq API / Qwen Model[cite: 6]
* **Database:** Airtable ("Book Inventory Tracker" base)[cite: 1]
* **Frontend/Interface:** n8n Chat Trigger Node

## 📂 Project Structure
* `Book Inventory Chat Bot.json`: The complete export file containing all nodes, agent configurations, and schema mappings for the n8n workflow[cite: 7].

## ⚙️ How to Use
1. Import the `Book Inventory Chat Bot.json` file into your self-hosted n8n instance.
2. Connect your **Groq API credentials** and **Airtable Personal Access Token**.
3. Open the chat interface and type natural commands (e.g., *"Update the quantity of Atomic Habits to 15"*).
