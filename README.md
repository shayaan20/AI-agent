# AI Local Agent – Email Assistant  

This project is a **local AI-powered agent** that connects to your e-mail inbox and helps you manage messages with natural language. It uses **LangChain**, **LangGraph**, and a local LLM (via [Ollama](https://ollama.ai)) to provide a conversational interface for tasks like listing unread emails and summarizing message content.  

## ✨ Features  
- 🔑 **Secure IMAP Connection** – Reads emails directly from your inbox using credentials stored in `.env`.  
- 📬 **List Unread Emails** – Returns metadata (UID, subject, date, sender) of unread messages.  
- 📝 **Summarize Emails** – Generates a concise summary of any email by IMAP UID.  
- 💬 **Conversational Agent** – Interact with your inbox using natural instructions like:  
  - `Show me my unread emails`  
  - `Summarize the latest message from John`  
- 🔄 **Tool-Oriented Workflow** – The agent routes between the LLM and specialized tools to complete tasks.  

## ⚙️ Tech Stack  
- **Python 3.9+**  
- **LangChain + LangGraph** – for chat model orchestration  
- **Ollama (qwen3:8b)** – local LLM backend  
- **imap-tools** – secure IMAP email fetching  
- **dotenv** – for environment configuration  

