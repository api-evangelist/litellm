---
title: "Security Update: Mistral AI PyPI Supply Chain Attack — LiteLLM Not Impacted"
url: "https://docs.litellm.ai/blog/mistral-supply-chain-attack-may-2026"
date: "2026-05-12"
author: "Mubashir Osmani"
feed_url: "https://docs.litellm.ai/blog/atom.xml"
---
On May 11, 2026, a malicious version of the mistralai PyPI package was published as part of a coordinated supply chain attack. LiteLLM is not affected — we call Mistral exclusively via httpx, never by importing the mistralai SDK.
