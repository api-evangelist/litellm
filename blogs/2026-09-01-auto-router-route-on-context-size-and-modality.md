---
title: "Auto-Router: Route on Context Size and Modality"
url: "https://docs.litellm.ai/blog/auto-router-more-routing-configurations"
date: "2026-09-01"
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
The Auto-Router now supports more routing configurations: context-window escalation moves oversized prompts to the cheapest tier that fits them before dispatch, modality routing sends image requests to tiers that can see, classification can run on user turns only, and shadow evaluations can compare several router configs on a team's live traffic.
