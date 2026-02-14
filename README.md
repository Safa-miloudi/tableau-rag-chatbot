## 🤖 Q&A Chatbot for Tableau Course (RAG Pipeline)

This project implements a **Retrieval-Augmented Generation (RAG)** chatbot capable of answering student questions based on the "Introduction to Tableau" course transcript.

Built using **LangChain**, **Google Gemini**, and **ChromaDB**, the system retrieves relevant course sections and generates context-aware answers with source citations.

## 🚀 Features
* **Document Loading**: Parses PDF course transcripts.
* **Smart Splitting**: Uses `MarkdownHeaderTextSplitter` to respect document hierarchy (Sections/Lectures).
* **Vector Search**: Embeds text using `gemini-embedding-001` and stores it in **ChromaDB**.
* **RAG Pipeline**: Retrieves relevant context using MMR (Maximal Marginal Relevance) to reduce redundancy.
* **Streaming Responses**: Provides real-time token streaming for a better user experience.

## 🛠️ Tech Stack
* **Python 3.9+**
* **LangChain** (Orchestration)
* **Google Gemini API** (LLM & Embeddings)
* **ChromaDB** (Vector Store)

## 📂 Project Structure
```bash
├── data/                  # Contains the source PDF transcript
├── LangChain_Project.ipynb       # Main Jupyter Notebook with the RAG pipeline
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation
