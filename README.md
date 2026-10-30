# LiteLLM

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

LiteLLM is an open-source Python SDK and proxy server providing a unified OpenAI-compatible interface to 100+ LLM providers.

**Areas:** Gateways · AI Gateway

## LiteLLM on APIs.io

Everything profiled for LiteLLM is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/litellm/](https://apis.io/providers/litellm/)** — or go straight to one of the APIs or properties below.

### APIs (33)

- [LiteLLM Completions API](https://apis.io/apis/litellm/completions-api/) — Provides an OpenAI-compatible /completions endpoint for text completion requests routed through the LiteLLM proxy to supported LLM providers.
- [LiteLLM Responses API](https://apis.io/apis/litellm/responses-api/) — Provides an OpenAI-compatible /responses endpoint supporting the Responses API specification, including conversation history compression via /responses/compact.
- [LiteLLM Embeddings API](https://apis.io/apis/litellm/embeddings-api/) — Provides an OpenAI-compatible /embeddings endpoint for generating text embeddings across multiple providers including OpenAI, Cohere, HuggingFace, and…
- [LiteLLM Image Generation API](https://apis.io/apis/litellm/image-generation-api/) — Provides OpenAI-compatible /images/generations, /images/edits, and /images/variations endpoints for image generation and manipulation routed through the…
- [LiteLLM Audio API](https://apis.io/apis/litellm/audio-api/) — Provides OpenAI-compatible /audio/transcriptions and /audio/speech endpoints for audio transcription and text-to-speech conversion across supported providers.
- [LiteLLM Moderations API](https://apis.io/apis/litellm/moderations-api/) — Provides an OpenAI-compatible /moderations endpoint for content moderation across supported providers through the LiteLLM proxy.
- [LiteLLM Batches API](https://apis.io/apis/litellm/batches-api/) — Provides an OpenAI-compatible /batches endpoint for batch processing operations, enabling bulk request handling across LLM providers.
- [LiteLLM Files API](https://apis.io/apis/litellm/files-api/) — Provides an OpenAI-compatible /files endpoint for file management operations used in conjunction with fine-tuning and batch processing.
- [LiteLLM Fine-Tuning API](https://apis.io/apis/litellm/fine-tuning-api/) — Provides an OpenAI-compatible /fine_tuning endpoint for model fine-tuning operations across supported providers through the LiteLLM proxy.
- [LiteLLM Rerank API](https://apis.io/apis/litellm/rerank-api/) — Provides a /rerank endpoint for document reranking operations, supporting providers like Cohere through the LiteLLM proxy with a unified interface.
- [LiteLLM Vector Stores API](https://apis.io/apis/litellm/vector-stores-api/) — Provides /vector_stores endpoints for creating and managing vector stores, file operations within vector stores, and search functionality for…
- [LiteLLM Anthropic Messages API](https://apis.io/apis/litellm/messages-api/) — Provides Anthropic-compatible /v1/messages and /v1/messages/count_tokens endpoints for native Anthropic API format support through the LiteLLM proxy.
- [LiteLLM Realtime API](https://apis.io/apis/litellm/realtime-api/) — Provides /realtime WebSocket endpoints for real-time model interactions with load balancing and guardrails support across providers.
- [LiteLLM MCP API](https://apis.io/apis/litellm/mcp-api/) — Provides /mcp endpoints for Model Context Protocol (MCP) integration, enabling LLMs to interact with external tools and APIs through OpenAPI specifications.
- [LiteLLM OCR API](https://apis.io/apis/litellm/ocr-api/) — Provides an /ocr endpoint for optical character recognition, enabling text extraction from images through supported providers via the LiteLLM proxy.
- [LiteLLM Guardrails API](https://apis.io/apis/litellm/guardrails-api/) — Provides /guardrails/apply_guardrail endpoint for applying configured content filtering and safety guardrails to LLM requests and responses.
- [LiteLLM Evals API](https://apis.io/apis/litellm/evals-api/) — Provides /evals endpoints for the Evaluations API, enabling measurement and benchmarking of model performance through the LiteLLM proxy.
- [LiteLLM A2A Agent Gateway API](https://apis.io/apis/litellm/a2a-api/) — Provides /a2a endpoints for the Agent-to-Agent (A2A) gateway, enabling agent registration, publishing, and inter-agent communication.
- [LiteLLM Videos API](https://apis.io/apis/litellm/videos-api/) — Provides /videos endpoints for video generation and handling through supported providers like RunwayML via the LiteLLM proxy.
- [LiteLLM Assistants API](https://apis.io/apis/litellm/litellm-assistants-api/) — The Assistants API from LiteLLM — 1 operation(s) for assistants.
- [LiteLLM Audio API](https://apis.io/apis/litellm/litellm-audio-api/) — The Audio API from LiteLLM — 2 operation(s) for audio.
- [LiteLLM Batches API](https://apis.io/apis/litellm/litellm-batches-api/) — The Batches API from LiteLLM — 1 operation(s) for batches.
- [LiteLLM Completions API](https://apis.io/apis/litellm/litellm-completions-api/) — The Completions API from LiteLLM — 1 operation(s) for completions.
- [LiteLLM Embeddings API](https://apis.io/apis/litellm/litellm-embeddings-api/) — The Embeddings API from LiteLLM — 1 operation(s) for embeddings.
- [LiteLLM Fine Tuning API](https://apis.io/apis/litellm/litellm-fine-tuning-api/) — The Fine Tuning API from LiteLLM — 1 operation(s) for fine tuning.
- [LiteLLM Images API](https://apis.io/apis/litellm/litellm-images-api/) — The Images API from LiteLLM — 3 operation(s) for images.
- [LiteLLM Messages API](https://apis.io/apis/litellm/litellm-messages-api/) — The Messages API from LiteLLM — 2 operation(s) for messages.
- [LiteLLM Moderations API](https://apis.io/apis/litellm/litellm-moderations-api/) — The Moderations API from LiteLLM — 1 operation(s) for moderations.
- [LiteLLM Ocr API](https://apis.io/apis/litellm/litellm-ocr-api/) — The Ocr API from LiteLLM — 1 operation(s) for ocr.
- [LiteLLM Rag API](https://apis.io/apis/litellm/litellm-rag-api/) — The Rag API from LiteLLM — 2 operation(s) for rag.
- [LiteLLM Rerank API](https://apis.io/apis/litellm/litellm-rerank-api/) — The Rerank API from LiteLLM — 1 operation(s) for rerank.
- [LiteLLM Vector Stores API](https://apis.io/apis/litellm/litellm-vector-stores-api/) — The Vector Stores API from LiteLLM — 2 operation(s) for vector stores.
- [LiteLLM Chat Completions API](https://apis.io/apis/litellm/litellm-chat-completions-api/) — The Chat Completions API from LiteLLM — 1 operation(s) for chat completions.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Litellm Agentic Access](https://apis.io/agentic-access/litellm/litellm-agentic-access/)

#### Collections (15)

Postman and Open Collection request collections.

- [LiteLLM Proxy API](https://apis.io/collections/litellm/open-litellm/)
- [LiteLLM Proxy Assistants API](https://apis.io/collections/litellm/open-litellm-assistants-api/)
- [LiteLLM Proxy Assistants Audio API](https://apis.io/collections/litellm/open-litellm-audio-api/)
- [LiteLLM Proxy Assistants Batches API](https://apis.io/collections/litellm/open-litellm-batches-api/)
- [LiteLLM Proxy Assistants Chat API](https://apis.io/collections/litellm/open-litellm-chat-api/)
- [LiteLLM Proxy Assistants Completions API](https://apis.io/collections/litellm/open-litellm-completions-api/)
- [LiteLLM Proxy Assistants Embeddings API](https://apis.io/collections/litellm/open-litellm-embeddings-api/)
- [LiteLLM Proxy Assistants Fine Tuning API](https://apis.io/collections/litellm/open-litellm-fine-tuning-api/)
- [LiteLLM Proxy Assistants Images API](https://apis.io/collections/litellm/open-litellm-images-api/)
- [LiteLLM Proxy Assistants Messages API](https://apis.io/collections/litellm/open-litellm-messages-api/)
- [LiteLLM Proxy Assistants Moderations API](https://apis.io/collections/litellm/open-litellm-moderations-api/)
- [LiteLLM Proxy Assistants Ocr API](https://apis.io/collections/litellm/open-litellm-ocr-api/)
- [LiteLLM Proxy Assistants Rag API](https://apis.io/collections/litellm/open-litellm-rag-api/)
- [LiteLLM Proxy Assistants Rerank API](https://apis.io/collections/litellm/open-litellm-rerank-api/)
- [LiteLLM Proxy Assistants Vector Stores API](https://apis.io/collections/litellm/open-litellm-vector-stores-api/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Litellm Domain Security](https://apis.io/security/litellm/litellm-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Litellm Plans Pricing](https://apis.io/plans/litellm/litellm-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Litellm Rate Limits](https://apis.io/rate-limits/litellm/litellm-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Litellm Finops](https://apis.io/finops/litellm/litellm-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.litellm.ai/)
- [Documentation](https://docs.litellm.ai/docs/)
- [Getting started](https://docs.litellm.ai/docs/proxy/quick_start)
- [Pricing](https://docs.litellm.ai/docs/enterprise)
- [Support](https://www.litellm.ai/support)
- [Changelog](https://www.litellm.ai/changelog)
- [Blog](https://docs.litellm.ai/blog)
- [Status](https://status.litellm.ai/)

## API Evangelist rating

**Kin Score 32.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 51.8 |
| Contract quality | 33.7 |
| Contract governance | 0.0 |
| Operational transparency | 28.9 |
| Developer ergonomics | 50.0 |
| Access clarity | 31.6 |

**Agent readiness 17.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 11.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/litellm/](https://apis.io/providers/litellm/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for LiteLLM: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/litellm/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
