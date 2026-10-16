---
title: "How we cut time to first byte by 94% for long prompts"
url: "https://docs.litellm.ai/blog/long-prompt-latency"
date: "2026-10-03"
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
A 440k-token benchmark went from 553 ms to 35 ms median time to first byte. We removed unnecessary prompt-cache routing work before the model call.
