# 🤖 Agentic RAG Course Assistant

An intelligent conversational assistant built with **Python**, **Google Gemini API** (`gemini-3.6-flash`), and the **OpenAI SDK** compatibility layer. The agent uses function calling to search a local FAQ knowledge base, handle multi-turn message history, and execute auto-retry rate limit handling.

---

## 🌟 Key Features

* **Function Calling Loop:** Dynamically determines when to execute external search tools vs. returning a direct response.
* **Multi-Turn Context:** Retains multi-step conversation context and appends tool execution outputs back into message histories.
* **Rate Limit Resiliency:** Implemented exponential backoff and error handling for API call quotas using `tenacity`.
* **Database & Ingestion:** Local SQLite (`faq.db`) integration for querying structured course data.

---

## 🚀 Getting Started

### 1. Prerequisites
* Python 3.10+
* Google Gemini API Key

### 2. Setup & Installation
```bash
git clone [https://github.com/Saquib-DA/LLM-code.git](https://github.com/Saquib-DA/LLM-code.git)
cd LLM-code
source .venv-1/bin/activate
pip install -r requirements.txt
