# RAG-Based AI Chatbot on Human Nutrition PDF

A Retrieval-Augmented Generation (RAG) chatbot designed completely from SCRATCH to provide context-aware answers derived directly from *Human Nutrition* documents.  
Built using Python, OpenAI Embeddings, Supabase (PostgreSQL + pgvector), and GPT-4o-mini.

---

## Overview

This project implements a complete **Retrieval-Augmented Generation (RAG)** pipeline that enables users to query a chatbot trained on a human nutrition knowledge base.  
The system processes a PDF document, stores its vector embeddings, retrieves relevant information for a user’s query, and generates grounded responses using GPT-4o-mini.

Key components such as **text chunking**, **vector generation**, **storage**, and **semantic retrieval** were developed manually to demonstrate a complete understanding of end-to-end RAG architecture.

---

## Features

- **Custom Text Chunking** – Implemented fixed-size chunking in Python to preprocess long PDF documents.  
- **OpenAI Embeddings** – Each chunk is converted into vector form for semantic similarity search.  
- **Supabase + pgvector** – Stores embeddings efficiently in a PostgreSQL database.  
- **Custom Retrieval Function** – `match_documents()` retrieves the most relevant document chunks based on user queries.  
- **GPT-4o-mini Integration** – Generates the final answer using retrieved context and the user’s input.  
- **Domain-Specific Responses** – All answers are grounded in the content of the Human Nutrition PDF.

---

## Tech Stack

| Component | Technology |
|------------|-------------|
| Programming Language | Python |
| Large Language Model | OpenAI GPT-4o-mini |
| Embeddings | OpenAI Text Embeddings |
| Database | Supabase (PostgreSQL + pgvector) |
| Libraries | openai, supabase, numpy, pandas, dotenv, tiktoken |
| Data Source | Human Nutrition PDF |
