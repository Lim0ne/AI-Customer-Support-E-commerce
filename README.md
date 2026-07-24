# Sharkbay AI Customer Support System

Official RAG-powered AI customer support and shopping assistant backend for **sharkbay.shop**, Malta's premier localized e-commerce platform.

---

## Core Features
- **Local Knowledge Base RAG**: Built with LangChain and ChromaDB, strictly referencing official enterprise policy documents regarding shipping, pickup, and returns in Malta.
- **Local LLM Integration**: Powered by Qwen 2.5 (via Ollama) for precise, context-aware, and data-secure responses.
- **FastAPI Backend**: High-performance, asynchronous RESTful API wrapper.
- **Developer Friendly**: Fully documented interactive Swagger UI (`/docs`).

---

## Project Structure
```text
sharkbay-ai-support/
├── sharkbay_knowledge_base.md   # Official enterprise knowledge base / policy manual
├── main.py                      # FastAPI application and RAG pipeline logic
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
