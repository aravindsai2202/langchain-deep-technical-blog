# LangChain Deep Technical Blog — Internship Assignment

A hands-on technical deep-dive into LangChain, covering core architecture, components, and working code implementations. Built as part of the Data Science Internship (Feb 2026) GenAI assignment.

## 📌 Overview

This repository contains a fully working Jupyter/Colab notebook demonstrating the core building blocks of LangChain — from basic LLM calls to agents with tool-calling and vector-based semantic search. All examples are original, tested, and run end-to-end using free, open-source models via HuggingFace Inference Providers.

## 🧠 Concepts Covered

| Component | What It Does |
|---|---|
| **LLMs & Chat Models** | Interfacing with language models through a unified API |
| **Prompt Templates** | Reusable, parameterized prompt structures |
| **Chains (LCEL)** | Composing prompt → LLM → parser pipelines using the `|` operator |
| **Memory** | Persisting conversation context across turns |
| **Agents & Tools** | Letting the model decide when to invoke external functions |
| **Vector Stores** | Semantic search over documents using embeddings (FAISS) |

## 🛠️ Tech Stack

- **Python 3**
- **LangChain** (`langchain`, `langchain-core`, `langchain-community`, `langchain-huggingface`)
- **HuggingFace Inference Providers** — free-tier model access (Qwen 2.5-7B-Instruct)
- **FAISS** — vector similarity search
- **Sentence Transformers** — text embeddings
- **Google Colab** — development environment

## 📂 Repository Structure
langchain-deep-technical-blog/
├── LangChain_Deep_Technical_Blog.ipynb # Full notebook with all code + explanations
└── README.md

## 🚀 Running This Notebook

1. Open `LangChain_Deep_Technical_Blog.ipynb` in Google Colab or Jupyter
2. Install dependencies:
```bash
   pip install langchain langchain-huggingface langchain-community huggingface_hub faiss-cpu sentence-transformers python-dotenv
```
3. Get a free HuggingFace access token from [huggingface.co/settings/tokens](https://huggingface.co/settings/tokens) (enable **"Make calls to Inference Providers"** permission)
4. Set it as an environment variable:
```python
   import os
   os.environ["HUGGINGFACEHUB_API_TOKEN"] = "your_token_here"
```
5. Run all cells top to bottom

## ✨ Key Highlights

- Uses **modern LCEL syntax** (`prompt | llm | parser`) rather than deprecated legacy chains
- **Agent with custom tool** demonstrates function-calling / tool-use reasoning
- **Session-based memory** using `RunnableWithMessageHistory`
- **FAISS vector store** for semantic similarity search, forming the foundation of RAG pipelines
- All models used are **free-tier** — no paid API keys required

## 👤 Author

Aravind Sai Thanneru — Data Science Intern
