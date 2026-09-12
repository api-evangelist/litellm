---
title: "AutoRouter Per-Hop Compression: Cut LLM Classifier Costs Another 32%"
url: "https://docs.litellm.ai/blog/auto-router-per-hop-compression"
date: "2026-09-05"
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
The complexity router's LLM classifier can now use different compression than the model call it routes to. The classifier only needs enough context to route correctly, not to generate an answer. In internal testing, compressing it aggressively cut classification costs a further 32% beyond shared compression, with no change in routing accuracy.
