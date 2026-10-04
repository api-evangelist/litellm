---
title: "Claude Code server-side auto mode through LiteLLM"
url: "https://docs.litellm.ai/blog/claude-code-server-side-auto-mode"
date: "2026-09-21"
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
Anthropic is moving Claude Code auto mode's safety classifier server-side. LiteLLM's native /v1/messages route now forwards the safeguards contract, and the fix ships in the dev release on September 22. Here is the contract, what changed, when it ships, and how to verify it.
