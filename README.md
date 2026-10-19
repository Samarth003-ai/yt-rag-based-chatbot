# 🎥 YouTube Video RAG Chatbot

An end-to-end Retrieval-Augmented Generation (RAG) chatbot using LangChain, FAISS vector search, and open-source Large Language Models to ask questions and summarize YouTube videos.

## 🚀 Features
- **YouTube Transcript Extraction:** Automatically fetches transcripts using `youtube-transcript-api`.
- **Text Chunking:** Splits transcripts into semantically meaningful chunks with `RecursiveCharacterTextSplitter`.
- **Vector Search (FAISS):** Embeds chunks using Hugging Face embeddings and indexes them for high-speed similarity search.
- **LLM Reasoning:** Uses LangChain Expression Language (LCEL) connected to Groq (`llama-3.3-70b-versatile`) for fast and accurate context-grounded responses.

## 🛠️ Tech Stack
- **LangChain** (LCEL, Core, Community)
- **HuggingFace Embeddings** (`sentence-transformers/all-MiniLM-L6-v2` or `dmis-lab/UltraBERT-Embed-150M`)
- **FAISS CPU** for vector database
- **Groq API** (`ChatGroq`) for ultra-fast LLM generation
- **YouTube Transcript API**

## 📦 Installation

```bash
pip install -r requirements.txt
```

## 🔑 Setup API Keys

Create a `.env` file or export your keys in the environment:

```bash
export GROQ_API_KEY="your-groq-api-key"
export HUGGING_FACE_KEY="your-huggingface-token"
```

## 💻 Usage

Run the Jupyter Notebook:
```bash
jupyter notebook rag.ipynb
```
