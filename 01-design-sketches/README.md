# Design sketches

One system design problem a week. The method matters more than the answer:

1. **20 minutes** sketching boxes and arrows, on paper, with no references.
2. **10 minutes** on rough numbers — QPS, storage, cost per 1,000 requests, p95 latency.
3. **20–30 minutes** reading a reference write-up, or having an AI critique the sketch as a staff
   engineer would, then listing what I missed.

Each week is a folder with `diagram.md`, `numbers.md`, `notes.md` and a README.

## The ladder

| # | Problem | What it teaches |
|---|---|---|
| 01 | URL shortener | Capacity estimation, hash vs counter IDs, cache in front of a read-heavy DB |
| 02 | Rate limiter for a paid API | Token bucket vs sliding window, shared counters, per-user quotas |
| 03 | Image upload and processing | Object storage, job queues, workers, polling vs webhooks |
| 04 | Model serving API | Dynamic batching, latency vs throughput, autoscaling, canary rollout |
| 05 | Feature and batch prediction pipeline | Offline vs online paths, training-serving skew, feature stores |
| 06 | Recommendation system | Cheap candidate generation then expensive ranking, cold start |
| 07 | RAG document Q&A at scale | Ingestion, chunking, hybrid search, reranking, evaluation |
| 08 | LLM gateway: routing, caching, fallback | Classifier routing, semantic cache, provider fallback, budget caps |
| 09 | Agentic task platform | Orchestration, checkpointing, context growth, sandboxing, cost caps |
| 10 | Real-time video analytics | Edge vs cloud inference, frame sampling, GPU scheduling, storage tiering |

Weeks 6, 8 and 10 are the same idea in three costumes: something cheap filters, something
expensive decides.
