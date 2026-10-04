---
title: "How we cut LiteLLM's Redis round trips per request by 64%"
url: "https://docs.litellm.ai/blog/redis-request-pipelines"
date: "2026-10-01"
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
A governed request to the LiteLLM AI Gateway waited on Redis 22 times. It now waits 8 times: one pipeline per Redis backend before the model call, one after.
