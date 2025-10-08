# 🧠 Conversational RAG Q&A With PDF Uploads and Chat History

[![Made with Streamlit](https://img.shields.io/badge/Made%20with-Streamlit-FF4B4B?logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Powered by LangChain](https://img.shields.io/badge/Powered%20by-LangChain-1D9BF0?logo=chainlink&logoColor=white)](https://www.langchain.com/)
[![Groq API](https://img.shields.io/badge/LLM-Groq%20Gemma2--9b--It-8A2BE2?logo=groq&logoColor=white)](https://console.groq.com/)
[![HuggingFace](https://img.shields.io/badge/Embeddings-HuggingFace-yellow?logo=huggingface&logoColor=white)](https://huggingface.co/)
[![Python](https://img.shields.io/badge/Built%20with-Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Google Colab](https://img.shields.io/badge/Run%20in-Google%20Colab-orange?logo=googlecolab&logoColor=white)](https://colab.research.google.com/)

---

### 📘 Overview

This project is a **Conversational Retrieval-Augmented Generation (RAG)** system that lets you:

- 📂 Upload multiple **PDF files**
- 💬 Chat interactively with their content
- 🧠 Maintain **conversation history**
- 🚀 Run seamlessly inside **Google Colab** using **Ngrok**
- 🤖 Powered by **Groq LLMs** and **LangChain**

---

## 🧩 Features

✅ PDF Uploads — drag, drop, and analyze instantly  
✅ Context-aware Conversations — chat with memory  
✅ Groq LLM Integration — blazing-fast inference  
✅ HuggingFace Embeddings — semantic vector search  
✅ Chroma Vector Store — document retrieval at scale  
✅ Streamlit Interface — elegant and interactive  

---

## 🏗️ Architecture

```text
        ┌────────────┐
        │   PDF(s)   │
        └─────┬──────┘
              │
     Text Extraction (PyPDFLoader)
              │
    Text Splitting (Recursive Splitter)
              │
   Embedding (HuggingFace MiniLM)
              │
 Vector Store (Chroma for Retrieval)
              │
      RAG Pipeline (LangChain)
              │
  LLM (Groq Gemma2-9b-It) → Response
```
### ⚙️ Installation (Google Colab)

Install dependencies:

!pip install -r requirements.txt

### 🔑 API Keys Setup

You’ll need three tokens before running the app:

API Key	Purpose	Get It From
🧠 Groq API Key	To use Groq’s Gemma2-9b-It LLM	https://console.groq.com/keys

🤗 HuggingFace Token	For embeddings (all-MiniLM-L6-v2)	https://huggingface.co/settings/tokens

🌍 Ngrok Auth Token	For public access to Streamlit in Colab	https://dashboard.ngrok.com/get-started/your-authtoken



