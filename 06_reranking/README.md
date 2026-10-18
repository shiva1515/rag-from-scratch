# 06 · Reranking

Reranking is the critical second stage of modern information retrieval. While first-stage retrieval (dense vector search, BM25, and hybrid fusion) scans large collections at high speed, it relies on decoupled representations that lose fine-grained query-document interactions.

Reranking takes the top candidates from the first stage ($N = 50 - 100$) and applies deep, full cross-attention scoring to re-sort and prune them down to the final context ($K = 3 - 5$).

---

## Notebook Roadmap

| Notebook | Topic | Description |
|---|---|---|
| **01 · Reranking Fundamentals & Two-Stage Pipelines** | Two-stage cascade, candidate depth, and latency | Why bi-encoders are shallow, why two stages are required, cascade depth ($N$) vs recall starvation |
| **02 · Cross-Encoders From Scratch** | Full cross-attention query-document scoring | Joint token encoding, classification heads, hands-on scoring with open-source cross-encoders |
| **03 · ColBERT & Late Interaction** | Multi-vector token retrieval and MaxSim | Token-level embeddings, pre-computable document representations, MaxSim operator from scratch, alignment heatmaps |
| **04 · Score Calibration & Thresholding** | Dynamic filtering and rejecting irrelevant candidates | Sigmoid scaling, avoiding the "Top-K Fallacy", dynamic confidence thresholding ($\tau$) to prevent hallucinations |
| **05 · Diversity & Maximal Marginal Relevance (MMR)** | Redundancy reduction and information diversity | MMR algorithm from scratch, balancing relevance ($\lambda$) and novelty, preventing near-duplicate context crowding |
| **06 · LLM as a Reranker** | Pointwise, pairwise, and listwise reranking | Prompting models for ranking, RankGPT sliding-window listwise permutations, cost vs latency vs accuracy |
| **07 · Benchmarking & Production Optimization** | IR evaluation and high-throughput deployment | Measuring NDCG@K and MRR lift, ONNX runtime acceleration, dynamic batching, and production decision matrices |

---

## Pedagogical Philosophy

Every notebook in this module follows the repository's core philosophy:
- **Built from scratch in pure Python:** No opaque wrapper frameworks hiding the mechanics.
- **Transparent math & metrics:** Exact formulas for cross-attention, MaxSim, calibration, and MMR.
- **Visualized behavior:** Token alignment heatmaps, score distributions, and rank shift diagrams.
- **Hard edge cases & failure modes:** Testing recall starvation, length truncation, and threshold edge cases.

