# Sharkbay AI Customer Support System

Official RAG-powered AI customer support and shopping assistant backend for sharkbay.shop, Malta's premier localized e-commerce platform.

---

## Core Features
* **Local Knowledge Base RAG**: Built with LangChain and ChromaDB, strictly referencing official enterprise policy documents regarding shipping, pickup, and returns in Malta.
* **Local LLM Integration**: Powered by Qwen 2.5 (via Ollama) for precise, context-aware, and data-secure responses.
* **FastAPI Backend**: High-performance, asynchronous RESTful API wrapper.
* **Developer Friendly**: Fully documented interactive Swagger UI (/docs).

---

## Project Structure
```text
sharkbay-ai-support/
├── sharkbay_knowledge_base.md   # Official enterprise knowledge base / policy manual
├── main.py                      # FastAPI application and RAG pipeline logic
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation


```

---

## Getting Started & Installation

### 1. Prerequisites

* Python 3.10+
* Ollama installed locally with the qwen2.5:3b model pulled:
```bash
ollama run qwen2.5:3b

```



### 2. Clone the Repository

```bash
git clone [https://github.com/Lim0ne/sharkbay-ai-support.git](https://github.com/Lim0ne/sharkbay-ai-support.git)
cd sharkbay-ai-support

```

### 3. Install Dependencies

```bash
pip install -r requirements.txt

```

### 4. Run the Application

Start the FastAPI server:

```bash
uvicorn main:app --host 127.0.0.1 --port 8000 --reload

```

---

## API Usage

Once the server is running locally, you can access the interactive documentation at:
- Local: http://127.0.0.1:8000/docs
- Colab (via Localtunnel): Use your generated public URL followed by /docs (e.g., https://xxxx.loca.lt/docs)

### Endpoint: POST /api/chat

**Request Body:**

```json
{
  "message": "Where is your warehouse located for local pickup?"
}

```

**Response:**

```json
{
  "status": "success",
  "reply": "Our dedicated local warehouse is located at San Pawl, Triq MRU Giorgio Zarb, Qormi, offering 100% free local pickup with zero shipping fees."
}

```

---

## License

This project is proprietary and built for sharkbay.shop.
