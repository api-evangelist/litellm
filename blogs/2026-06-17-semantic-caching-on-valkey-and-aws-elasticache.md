---
title: "Semantic Caching on Valkey and AWS ElastiCache"
url: "https://docs.litellm.ai/blog/valkey_semantic_caching"
date: "2026-06-17"
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
LiteLLM now supports semantic prompt caching on Valkey clusters and AWS ElastiCache without requiring RediSearch or Qdrant. The feature lets the gateway reuse responses for semantically similar prompts to cut latency and cost.
