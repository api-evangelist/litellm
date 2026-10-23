---
title: "Decision models on LiteLLM: /v1/decisions and /v1/systemone"
url: "https://docs.litellm.ai/blog/decision-models"
date: "2026-10-14"
author: "Kerry Lu"
feed_url: "https://docs.litellm.ai/blog/atom.xml"
---
Decision models return probabilities instead of text, which makes routing, triage and guardrail checks cheap and deterministic. LiteLLM serves nine providers of them behind one request shape.
