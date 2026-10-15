# RAG101 — Retrieval-Augmented Generation

A hands-on project exploring the fundamentals of Retrieval-Augmented Generation (RAG) with Python.

## Overview

RAG (Retrieval-Augmented Generation) combines document retrieval with Large Language Models (LLMs). It allows a system to retrieve relevant information from a knowledge base and use that context to generate more relevant, grounded answers.

This project implements the foundational steps of a RAG pipeline, from document loading to vector storage.

## Features

- **Document Loading:** Load and extract content from PDF and text files.
- **Document Chunking:** Split documents into smaller chunks using `RecursiveCharacterTextSplitter`.
- **Embedding Generation:** Convert text into numerical vector representations using Sentence Transformers.
- **Vector Storage:** Store document embeddings and metadata in ChromaDB.
- **Persistent Storage:** Preserve the vector database locally for reuse.

## Tech Stack

- Python
- LangChain Community
- LangChain Text Splitters
- Sentence Transformers
- ChromaDB
- NumPy

## Project Workflow

```text
PDF / TXT Documents
        |
        v
 Document Loading
        |
        v
 Document Chunking
        |
        v
 Embedding Generation
        |
        v
 ChromaDB Vector Store
        |
        v
 Semantic Retrieval
```

## Project Structure

```text
RAG101/
├── src/
│   └── ...
├── data/
│   └── vector_store/
├── .gitignore
├── .python-version
├── pyproject.toml
├── requirements.txt
├── uv.lock
└── README.md
```

_The structure above is illustrative; update it to match the actual files in the project._

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/myriam2005/rag101.git
cd rag101
```

### 2. Set up the environment

If you use `uv`:

```bash
uv sync
```

Alternatively, create a virtual environment and install the requirements:

```bash
python -m venv .venv
```

Activate it on Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

Then install the dependencies:

```bash
pip install -r requirements.txt
```

### 3. Prepare your documents

Place the PDF or text files you want to process in the project's configured data directory.

### 4. Run the project

Run the relevant Python script or notebook from your development environment. The exact entry point depends on the modules implemented in `src/`.

## Learning Goals

- Understand the main stages of a RAG pipeline.
- Work with LangChain document loaders and splitters.
- Generate embeddings using Sentence Transformers.
- Store and organize vectors with ChromaDB.
- Prepare document data for semantic retrieval.

## Current Status

Foundational RAG components are being developed, including document loading, chunking, embedding generation, and vector-store initialization.

## Future Improvements

- Implement document insertion into ChromaDB.
- Add semantic similarity search.
- Retrieve relevant chunks for user queries.
- Integrate an LLM to generate context-aware answers.
- Build an end-to-end RAG pipeline.

## Author

**Myriam Kary**

GitHub: [@myriam2005](https://github.com/myriam2005)
