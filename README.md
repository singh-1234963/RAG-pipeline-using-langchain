🤔 What is RAG?
Retrieval-Augmented Generation (RAG) is an AI architecture that combines two powerful components:

Retriever — Fetches relevant documents or chunks from a knowledge base (vector store) based on the user's query.
Generator — An LLM (e.g., GPT-4, Claude) that uses the retrieved context to generate an accurate, grounded response.
User Query
    │
    ▼
[Embedding Model]  ──► Query Vector
    │
    ▼
[Vector Store]  ──► Top-K Relevant Document Chunks
    │
    ▼
[Prompt Template]  ──► Context + Query → Prompt
    │
    ▼
[LLM (e.g. GPT-4)]  ──► Final Answer
User Query
    │
    ▼
[Embedding Model]  ──► Query Vector
    │
    ▼
[Vector Store]  ──► Top-K Relevant Document Chunks
    │
    ▼
[Prompt Template]  ──► Context + Query → Prompt
    │
    ▼
[LLM (e.g. GPT-4)]  ──► Final Answer
 │
    ▼
[Vector Store]  ──► Persisted Index
