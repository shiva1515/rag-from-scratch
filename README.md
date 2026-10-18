# RAG From Scratch

A hands-on project for learning how Retrieval-Augmented Generation works, from embeddings and search through to generation. The notebooks explain core ideas and build selected components from scratch.

## What’s covered

- **Embeddings:** vector similarity, Word2Vec, BERT, bi-encoders, and ColBERT — [`02_embedding_models/`](02_embedding_models/)
- **Vector search:** exact search, IVF, product quantization, and HNSW — [`03_vector_search_and_indexing/`](03_vector_search_and_indexing/)
- **Vector databases:** records, CRUD, storage concepts, and a Qdrant walkthrough — [`04_vector_database/`](04_vector_database/)
- **Retrieval strategies:** fundamentals, dense & sparse (BM25), hybrid RRF fusion, filtered ANN, multi-query, decomposition, and parent-document retrieval — [`05_retrieval/`](05_retrieval/)

## What’s next

Reranking and cross-encoders ([`06_reranking/`](06_reranking/)), advanced retrieval extensions, document ingestion and chunking, LLM generation, memory, agentic RAG, and evaluation. See the [learning roadmap](docs/ROADMAP.md).

## Extras

See [papers and learning resources](docs/REFERENCES.md).

## Getting started

Set up Python and Jupyter using the [environment guide](docs/SETUP.md), then open a notebook from one of the covered modules. Each notebook describes its specific dependencies and setup where needed.