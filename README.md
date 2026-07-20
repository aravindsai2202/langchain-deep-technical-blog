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
