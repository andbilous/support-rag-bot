# Support Policy RAG Bot

This project demonstrates a simple **Retrieval-Augmented Generation (RAG)** pipeline using `LangChain`, `FAISS`, and `OpenAI`.  
It allows you to load a PDF file (e.g., a support policy document), convert it into vector embeddings, and query it via a chatbot powered by GPT.

---

##  Features

- Loads and splits a support policy PDF
-  Creates document chunks with overlapping context
-  Embeds the text using `gte-small` from HuggingFace
-  Stores and retrieves similar chunks using `FAISS`
-  Answers user questions using GPT-3.5-turbo + relevant chunks (RAG-style)

---

##  Requirements

Install dependencies:

```bash
pip install langchain openai transformers faiss-cpu python-dotenv
