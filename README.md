# LiteLLM (litellm)

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
