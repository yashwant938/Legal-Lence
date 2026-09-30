# Legal Lens — Project Index

Legal information retrieval and conversational search, developed collaboratively for CSE508 at IIIT Delhi.

**The implementation lives in [YashwantRana23/CSE508_Winter2024_Project](https://github.com/YashwantRana23/CSE508_Winter2024_Project).** This repository is a project index and does not contain a separate application.

## What the source project implements

- BM25 retrieval over a configured legal-document CSV, with a small fallback corpus for demonstration.
- TF-IDF pairwise document similarities, a graph view and a top-three ranking by average similarity.
- A separate PDF-based RAG chatbot using Hugging Face embeddings, FAISS, LangChain and an OpenAI model.
- A FastAPI backend and Next.js interface with registration/login, search, graph exploration, chat and feedback.

The BM25/graph pipeline and PDF chatbot are separate workflows. The graph ranking is a document-similarity heuristic rather than a query-aware relevance reranker. The project remains a prototype with dependency, evaluation and conversation-isolation work to complete.

## My contribution

I contributed the FastAPI/Next.js application refactor, including API routes, retrieval services and the web interface. See the [public contribution commit](https://github.com/YashwantRana23/CSE508_Winter2024_Project/commit/d681f4b01e1ca9872389c9a47ae59097a888d7a0).

The project was developed by **Harsh Patel, Sahil More, Sarthak Pol, Vinayak Katoch and Yashwant Rana**. The source repository retains the original experiments and team history.

## Explore the project

- [Source, setup and project documentation](https://github.com/YashwantRana23/CSE508_Winter2024_Project)
- [BM25 service](https://github.com/YashwantRana23/CSE508_Winter2024_Project/blob/main/backend/app/services/bm25_service.py)
- [TF-IDF graph and similarity ranking](https://github.com/YashwantRana23/CSE508_Winter2024_Project/blob/main/backend/app/services/knowledge_graph_service.py)
- [PDF retrieval and chatbot service](https://github.com/YashwantRana23/CSE508_Winter2024_Project/blob/main/backend/app/services/chatbot_service.py)

