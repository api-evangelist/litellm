---
title: "Shadow Evaluations: Test the Auto-Router on Your Own Production Traffic"
url: "https://docs.litellm.ai/blog/auto-router-shadow-evaluations"
date: "2026-08-18"
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
Shadow evaluations duplicate a sampled slice of one key's live traffic through an auto-router and have an LLM judge blindly compare the answers. On our own traffic the router matched or beat the current model on 88.1% of judged responses, measured before a single user-facing response changed.
