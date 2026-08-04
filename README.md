# LiteLLM (litellm)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

LiteLLM is an open-source Python SDK and proxy server providing a unified OpenAI-compatible interface to 100+ LLM providers.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/master/apis.yml](https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/master/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Gateways

## Timestamps

- **Created:** 2026-03-03
- **Modified:** 2026-05-19

## APIs

### LiteLLM Chat Completions API

Provides an OpenAI-compatible /chat/completions endpoint that routes requests to 100+ LLM providers with unified request and response formatting, streaming support, cost tracking, and load balancing.

- **Human URL:** [https://docs.litellm.ai/docs/completion](https://docs.litellm.ai/docs/completion)

#### Tags

- AI
- Chat
- Completions
- LLM

#### Properties

- [Documentation](https://docs.litellm.ai/docs/completion)
- [Getting Started](https://docs.litellm.ai/docs/proxy/quick_start)
- [OpenAPI](openapi/litellm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Completions API

Provides an OpenAI-compatible /completions endpoint for text completion requests routed through the LiteLLM proxy to supported LLM providers.

- **Human URL:** [https://docs.litellm.ai/docs/text_completion](https://docs.litellm.ai/docs/text_completion)

#### Tags

- Completions
- LLM
- Text

#### Properties

- [Documentation](https://docs.litellm.ai/docs/text_completion)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Responses API

Provides an OpenAI-compatible /responses endpoint supporting the Responses API specification, including conversation history compression via /responses/compact.

- **Human URL:** [https://docs.litellm.ai/docs/response_api](https://docs.litellm.ai/docs/response_api)

#### Tags

- AI
- LLM
- Responses

#### Properties

- [Documentation](https://docs.litellm.ai/docs/response_api)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Embeddings API

Provides an OpenAI-compatible /embeddings endpoint for generating text embeddings across multiple providers including OpenAI, Cohere, HuggingFace, and Bedrock with unified formatting.

- **Human URL:** [https://docs.litellm.ai/docs/embedding/supported_embedding](https://docs.litellm.ai/docs/embedding/supported_embedding)

#### Tags

- AI
- Embeddings
- Vectors

#### Properties

- [Documentation](https://docs.litellm.ai/docs/embedding/supported_embedding)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Image Generation API

Provides OpenAI-compatible /images/generations, /images/edits, and /images/variations endpoints for image generation and manipulation routed through the LiteLLM proxy.

- **Human URL:** [https://docs.litellm.ai/docs/image_generation](https://docs.litellm.ai/docs/image_generation)

#### Tags

- AI
- Generation
- Images

#### Properties

- [Documentation](https://docs.litellm.ai/docs/image_generation)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Audio API

Provides OpenAI-compatible /audio/transcriptions and /audio/speech endpoints for audio transcription and text-to-speech conversion across supported providers.

- **Human URL:** [https://docs.litellm.ai/docs/audio_transcription](https://docs.litellm.ai/docs/audio_transcription)

#### Tags

- AI
- Audio
- Speech
- Transcription

#### Properties

- [Documentation](https://docs.litellm.ai/docs/audio_transcription)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Moderations API

Provides an OpenAI-compatible /moderations endpoint for content moderation across supported providers through the LiteLLM proxy.

- **Human URL:** [https://docs.litellm.ai/docs/moderation](https://docs.litellm.ai/docs/moderation)

#### Tags

- Content
- Moderation
- Safety

#### Properties

- [Documentation](https://docs.litellm.ai/docs/moderation)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Batches API

Provides an OpenAI-compatible /batches endpoint for batch processing operations, enabling bulk request handling across LLM providers.

- **Human URL:** [https://docs.litellm.ai/docs/batches](https://docs.litellm.ai/docs/batches)

#### Tags

- Batches
- Bulk
- Processing

#### Properties

- [Documentation](https://docs.litellm.ai/docs/batches)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Files API

Provides an OpenAI-compatible /files endpoint for file management operations used in conjunction with fine-tuning and batch processing.

- **Human URL:** [https://docs.litellm.ai/docs/files_endpoints](https://docs.litellm.ai/docs/files_endpoints)

#### Tags

- Files
- Management

#### Properties

- [Documentation](https://docs.litellm.ai/docs/files_endpoints)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Fine-Tuning API

Provides an OpenAI-compatible /fine_tuning endpoint for model fine-tuning operations across supported providers through the LiteLLM proxy.

- **Human URL:** [https://docs.litellm.ai/docs/fine_tuning](https://docs.litellm.ai/docs/fine_tuning)

#### Tags

- Fine-Tuning
- Models
- Training

#### Properties

- [Documentation](https://docs.litellm.ai/docs/fine_tuning)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Rerank API

Provides a /rerank endpoint for document reranking operations, supporting providers like Cohere through the LiteLLM proxy with a unified interface.

- **Human URL:** [https://docs.litellm.ai/docs/rerank](https://docs.litellm.ai/docs/rerank)

#### Tags

- Relevance
- Rerank
- Search

#### Properties

- [Documentation](https://docs.litellm.ai/docs/rerank)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Vector Stores API

Provides /vector_stores endpoints for creating and managing vector stores, file operations within vector stores, and search functionality for retrieval-augmented generation (RAG) use cases.

- **Human URL:** [https://docs.litellm.ai/docs/vector_stores/create](https://docs.litellm.ai/docs/vector_stores/create)

#### Tags

- RAG
- Search
- Storage
- Vectors

#### Properties

- [Documentation](https://docs.litellm.ai/docs/vector_stores/create)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Anthropic Messages API

Provides Anthropic-compatible /v1/messages and /v1/messages/count_tokens endpoints for native Anthropic API format support through the LiteLLM proxy.

- **Human URL:** [https://docs.litellm.ai/docs/anthropic_unified/](https://docs.litellm.ai/docs/anthropic_unified/)

#### Tags

- AI
- Anthropic
- Messages

#### Properties

- [Documentation](https://docs.litellm.ai/docs/anthropic_unified/)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Realtime API

Provides /realtime WebSocket endpoints for real-time model interactions with load balancing and guardrails support across providers.

- **Human URL:** [https://docs.litellm.ai/docs/realtime](https://docs.litellm.ai/docs/realtime)

#### Tags

- Realtime
- Streaming
- WebSocket

#### Properties

- [Documentation](https://docs.litellm.ai/docs/realtime)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM MCP API

Provides /mcp endpoints for Model Context Protocol (MCP) integration, enabling LLMs to interact with external tools and APIs through OpenAPI specifications.

- **Human URL:** [https://docs.litellm.ai/docs/mcp](https://docs.litellm.ai/docs/mcp)

#### Tags

- MCP
- Protocols
- Tools

#### Properties

- [Documentation](https://docs.litellm.ai/docs/mcp)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM OCR API

Provides an /ocr endpoint for optical character recognition, enabling text extraction from images through supported providers via the LiteLLM proxy.

- **Human URL:** [https://docs.litellm.ai/docs/ocr](https://docs.litellm.ai/docs/ocr)

#### Tags

- Images
- OCR
- Text Extraction

#### Properties

- [Documentation](https://docs.litellm.ai/docs/ocr)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Guardrails API

Provides /guardrails/apply_guardrail endpoint for applying configured content filtering and safety guardrails to LLM requests and responses.

- **Human URL:** [https://docs.litellm.ai/docs/apply_guardrail](https://docs.litellm.ai/docs/apply_guardrail)

#### Tags

- Content Filtering
- Guardrails
- Safety

#### Properties

- [Documentation](https://docs.litellm.ai/docs/apply_guardrail)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Evals API

Provides /evals endpoints for the Evaluations API, enabling measurement and benchmarking of model performance through the LiteLLM proxy.

- **Human URL:** [https://docs.litellm.ai/docs/evals_api](https://docs.litellm.ai/docs/evals_api)

#### Tags

- Benchmarks
- Evaluations
- Performance

#### Properties

- [Documentation](https://docs.litellm.ai/docs/evals_api)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM A2A Agent Gateway API

Provides /a2a endpoints for the Agent-to-Agent (A2A) gateway, enabling agent registration, publishing, and inter-agent communication.

- **Human URL:** [https://docs.litellm.ai/docs/a2a](https://docs.litellm.ai/docs/a2a)

#### Tags

- A2A
- Agents
- Gateway

#### Properties

- [Documentation](https://docs.litellm.ai/docs/a2a)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LiteLLM Videos API

Provides /videos endpoints for video generation and handling through supported providers like RunwayML via the LiteLLM proxy.

- **Human URL:** [https://docs.litellm.ai/docs/videos](https://docs.litellm.ai/docs/videos)

#### Tags

- AI
- Generation
- Videos

#### Properties

- [Documentation](https://docs.litellm.ai/docs/videos)
- [Postman Collection](collections/litellm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/litellm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/litellm)
- [Portal](https://www.litellm.ai/)
- [Documentation](https://docs.litellm.ai/docs/)
- [Getting Started](https://docs.litellm.ai/docs/proxy/quick_start)
- [Git Hub Org](https://github.com/BerriAI/litellm)
- [Blog](https://docs.litellm.ai/blog)
- [Changelog](https://www.litellm.ai/changelog)
- [Release Notes](https://docs.litellm.ai/release_notes)
- [Status Page](https://status.litellm.ai/)
- [Support](https://www.litellm.ai/support)
- [Pricing](https://docs.litellm.ai/docs/enterprise)
- [Dashboard](https://admin.litellm.ai/)
- [Providers](https://docs.litellm.ai/docs/providers)
- [Models](https://models.litellm.ai/)
- [Configuration](https://docs.litellm.ai/docs/proxy/configs)
- [Authentication](https://docs.litellm.ai/docs/set_keys)
- [Guardrails](https://docs.litellm.ai/docs/apply_guardrail)
- [Enterprise](https://docs.litellm.ai/docs/proxy/enterprise)
- [Release Cycle](https://docs.litellm.ai/docs/proxy/release_cycle)
- [S S O](https://docs.litellm.ai/docs/proxy/admin_ui_sso)
- [Docker](https://docs.litellm.ai/docs/proxy/docker_quick_start)
- [Py P I](https://pypi.org/project/litellm/)
- [L L Ms Txt](https://docs.litellm.ai/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
