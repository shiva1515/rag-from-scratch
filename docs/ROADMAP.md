# Learning Roadmap

This roadmap tracks the topics covered by the notebooks and the main areas planned next. The sequence is a guide, not a requirement to complete every topic in order.

## Covered

| Module | Topics |
| --- | --- |
| [02 · Embedding models](../02_embedding_models/) | Vector fundamentals, Word2Vec, contextual embeddings, bi-encoders, advanced retrieval embeddings, and model evaluation |
| [03 · Vector search and indexing](../03_vector_search_and_indexing/) | Exact search, IVF, product quantization, and HNSW |
| [04 · Vector databases](../04_vector_database/) | Database fundamentals, records and CRUD, storage and indexing, and Qdrant |
| [05 · Retrieval strategies (Part 1)](../05_retrieval/) | Retrieval fundamentals, dense semantic search, sparse BM25, hybrid search (RRF), metadata-filtered retrieval, multi-query expansion, query decomposition, and parent-document / sentence-window retrieval |

## Planned

| Module | Topics |
| --- | --- |
| 01 · Ingestion and chunking | Document parsing, tokenization, chunking strategies, and metadata |
| [05 · Advanced retrieval extensions](../05_retrieval/) | HyDE & query rewriting, contextual retrieval (Anthropic style), self-querying (text-to-AST), semantic routing, contextual compression, graph-augmented retrieval, and IR benchmarking |
| [06 · Reranking](../06_reranking/) | Two-stage cascade, cross-encoders, ColBERT & late interaction, score calibration & thresholding, MMR diversity, LLM listwise reranking (RankGPT), and ONNX optimization |
| 07 · LLM generation | Transformer and attention fundamentals, KV cache, quantization, and grounded synthesis |
| 08 · Memory systems | Working, episodic, and semantic memory; hierarchical memory and consolidation |
| 09 · Agentic RAG | Self-correcting retrieval (CRAG), Self-RAG, routing, and iterative retrieval loops |
| 10 · Evaluation and production | End-to-end RAG evaluation, caching, guardrails, observability, and deployment considerations |

## Learning goal

Build an end-to-end understanding of a RAG system: ingest and prepare documents, retrieve relevant evidence, generate grounded answers, and evaluate the system.
