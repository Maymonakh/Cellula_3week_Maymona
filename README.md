# Cellula Internship — 2 Week Tasks

This repository contains my solutions for the tasks completed during my 3-week internship at **Cellula Technologies**.

## Task 0 — BigBird Model Research

Research about the **BigBird Transformer model** and how it handles long sequences more efficiently than standard Transformers.

The task covers:

* The quadratic complexity of standard self-attention
* BigBird architecture and sparse attention
* Local, random, and global attention
* Block-sparse attention patterns
* Computational complexity comparison between BigBird, BERT, and Longformer
* Applications, advantages, and limitations of BigBird

---

## Task 1 — Retrieval-Augmented Generation (RAG)

The goal was to build a simple **RAG system** that answers questions using information retrieved from a personal information document.

The system follows this workflow:

```text
Personal Information Document
            ↓
      Text Splitting
            ↓
       Embeddings
            ↓
     FAISS Vector Store
            ↓
    Retrieve Relevant Text
            ↓
       Prompt Template
            ↓
     Language Model (LLM)
            ↓
          Answer
```

### Main Components

* **Text Splitting:** Dividing the document into smaller text chunks.
* **Embeddings:** Converting text chunks into numerical representations using a Hugging Face embedding model.
* **FAISS:** Storing embeddings and retrieving relevant information based on semantic similarity.
* **Prompt Template:** Providing the retrieved context and user's question to the model.
* **LLM:** Generating answers using the OpenRouter API.

### Technologies

* Python
* LangChain
* Hugging Face
* FAISS
* OpenRouter API
* Google Colab / Jupyter Notebook
