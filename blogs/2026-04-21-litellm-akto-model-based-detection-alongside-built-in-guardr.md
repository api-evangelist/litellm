---
title: "LiteLLM × Akto: Model-Based Detection Alongside Built-in Guardrails"
url: "https://docs.litellm.ai/blog/akto-partnership"
date: "Tue, 21 Apr 2026 10:00:00 GMT"
author: ""
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
<p><img alt="LiteLLM x Akto Partnership" class="img_ev3q" height="2508" src="https://docs.litellm.ai/assets/images/litellm_akto_announcement-7c5324c9fff708aff8679285950386be.png" width="4800" /></p>
<p><a href="https://akto.io/" rel="noopener noreferrer" target="_blank">Akto</a> now runs natively inside the LiteLLM proxy as a chained guardrail.</p>
<!-- -->
<p>LiteLLM already ships with built-in guardrails for fast, deterministic checks (regex-based PII, secret scanning, banned-word lists). Akto adds a second layer on top — <strong>model-based detection</strong> for the cases deterministic rules can't cover: prompt injection, semantic PII leaks, and custom policy violations that require an LLM to classify intent.</p>
<p>You run them together. LiteLLM's guardrails handle the cheap, fast checks; Akto handles the scenarios that need a model in the loop.</p>
<p><img alt="Guardrail Chaining: Client → LiteLLM Proxy → LLMs / MCPs / Agents, with LiteLLM Guardrails chaining to Akto" class="img_ev3q" height="1100" src="https://docs.litellm.ai/assets/images/litellm_guardrail_chaining-7e31a7d5f6a5a6d1abc930ee0a3d7434.png" width="1760" /></p>
<p>Akto runs in <strong>sync mode</strong> (block on violation before the LLM is called) or <strong>async mode</strong> (log and alert without adding latency). Configure it as a callback on your existing proxy — no app-level changes.</p>
<p><strong>Get started:</strong> <a href="https://docs.litellm.ai/docs/proxy/guardrails/akto">Akto guardrail setup guide</a></p>
<p><strong>Read the full announcement</strong> on <a href="https://www.akto.io/blog/akto-partners-litellm-ai-gateway-security-agents" rel="noopener noreferrer" target="_blank">Akto's blog →</a></p>
