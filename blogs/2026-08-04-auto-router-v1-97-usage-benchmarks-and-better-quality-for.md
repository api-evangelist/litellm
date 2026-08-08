---
title: "Auto Router v1.97: usage benchmarks and better quality for lower cost"
url: "https://docs.litellm.ai/blog/auto-router-context-and-benchmarks"
date: "2026-08-04"
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
v1.97 adds cost and usage benchmarks for the auto router, gives the LLM classifier a window of prior turns, and turns session affinity off by default. Across 5,600 live classifier calls, prior turns raised tier agreement on referential follow-ups from 14% to 78% at under a tenth of a cent per request, with no measurable latency change.
