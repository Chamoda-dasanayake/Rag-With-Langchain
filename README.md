# 🚀 RagWithLangchain – RAG-based Document QA System

RagWithLangchain is a **Retrieval-Augmented Generation (RAG)** project built using LangChain.  
It enables users to ask questions about their own documents and receive accurate, context-based answers powered by LLMs.

---

## 📌 Project Overview
This project demonstrates how to build a **document-aware AI system** by combining:
- Document retrieval (vector search)
- Context augmentation
- Large Language Model (LLM) generation  

The system ensures responses are grounded in your documents rather than relying only on pre-trained knowledge.

---

## 💡 What This Project Does

| Stage | Description |
|------|------------|
| Document Ingestion | Loads PDFs, splits them into chunks, and generates embeddings |
| Vector Storage | Stores embeddings in Chroma vector database |
| Retrieval | Finds relevant document chunks based on user queries |
| Generation | Uses an LLM (Groq) to generate answers using retrieved context |

---

## ⚙️ Workflow
PDF Files → Load → Split → Embed → Store in Chroma
↓
User Query → Embed → Similarity Search → Retrieve Chunks
↓
LLM (Groq) → Generate Answer based on Context

---

## 🧩 Key Components

| File | Purpose |
|-----|--------|
| `langchain_rag_doc_ingetion.ipynb` | Loads PDFs, splits text, creates embeddings, stores in Chroma |
| `langchain_rag_retrieval.ipynb` | Retrieves documents and generates answers using LLM |
| `docs_dir/` | Contains source PDF documents |
| `vector_db/` | Persistent Chroma vector database |
| `requirement.txt` | Project dependencies |
| `clean_secret.py` | Handles API keys and secrets |

---

## 🛠️ Tech Stack

- **Framework:** LangChain  
- **Embeddings:** HuggingFace (sentence-transformers)  
- **Vector Database:** Chroma  
- **LLM:** Groq (ChatGroq - Llama models)  
- **Text Splitting:** CharacterTextSplitter  
- **Document Loader:** UnstructuredFileLoader  

---

## ✨ Key Features

- 📄 Ask questions over your own PDF documents  
- 🔍 Semantic search using vector embeddings  
- 🤖 Context-aware answer generation  
- ⚡ Fast inference with Groq LLM  
- 🧠 Modular and extensible RAG pipeline  

---

## 🎯 Use Cases

- Research paper analysis  
- Internal document search  
- Knowledge base systems  
- Academic and technical Q&A  

---

## ⚙️ How to Run

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/RagWithLangchain.git
cd RagWithLangchain
