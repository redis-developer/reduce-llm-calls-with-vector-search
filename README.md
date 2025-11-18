# Reduce LLM Calls with Vector Search

This repository demonstrates techniques for reducing LLM API calls and costs by using vector search and semantic similarity matching. Each notebook showcases a different use case where vector embeddings can replace or augment traditional LLM-based approaches.

## Notebooks

### Python

| Notebook | Description |
|----------|-------------|
| [1_classification.ipynb](./python/1_classification.ipynb) | Semantic classification using vector embeddings instead of LLM-based classification |
| [2_tool_calling.ipynb](./python/2_tool_calling.ipynb) | Semantic tool calling/routing using similarity matching instead of LLM function calling |
| [3_1_pre_generated_semantic_caching.ipynb](./python/3_1_pre_generated_semantic_caching.ipynb) | Semantic caching with pre-generated FAQs to reduce redundant LLM calls |
| [3_2_semantic_caching.ipynb](./python/3_2_semantic_caching.ipynb) | Semantic caching for intelligent response retrieval based on query meaning |

### Kotlin

| Notebook | Description |
|----------|-------------|
| [1_classification.ipynb](./kotlin/1_classification.ipynb) | Semantic classification using vector embeddings (Kotlin implementation) |
| [2_tool_calling.ipynb](./kotlin/2_tool_calling.ipynb) | Semantic tool calling/routing (Kotlin implementation) |
| [3_guardrails.ipynb](./kotlin/3_guardrails.ipynb) | Semantic guardrails to block topics without LLM prompts |
| [4_1_pre_generated_semantic_caching.ipynb](./kotlin/4_1_pre_generated_semantic_caching.ipynb) | Semantic caching with pre-generated content (Kotlin implementation) |
| [4_2_semantic_caching_with_langcache.ipynb](./kotlin/4_2_semantic_caching_with_langcache.ipynb) | Semantic caching using LangCache library |

## Key Benefits

- **Cost Reduction**: Eliminate unnecessary LLM API calls by using vector similarity matching
- **Lower Latency**: Near-instantaneous responses through vector search instead of network round-trips
- **Higher Accuracy**: Deterministic results for classification and routing tasks
- **Scalability**: Handle high-volume requests without proportional cost increases

## Technologies Used

- **Redis**: Vector database for storing and searching embeddings
- **RedisVL**: Vector library providing abstractions for semantic routing, caching, and classification
- **Sentence Transformers**: Pre-trained models for text embeddings
- **Python & Kotlin**: Language implementations for broader accessibility