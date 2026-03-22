# LiteLLM (litellm)
LiteLLM is an open-source Python SDK and proxy server providing a unified OpenAI-compatible interface to 100+ LLM providers.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/apis.yml)

## Scope

- **Type:** Index 
- **Position:** Consuming 
- **Access:** 3rd-Party 

## Tags:

 - Gateways

## Timestamps

- **Created:** 2026-03-03 
- **Modified:** 2026-03-16 

## APIs

### LiteLLM Chat Completions API
Provides an OpenAI-compatible /chat/completions endpoint that routes requests to 100+ LLM providers with unified request and response formatting, streaming support, cost tracking, and load balancing.

**Human URL:** [https://docs.litellm.ai/docs/completion](https://docs.litellm.ai/docs/completion)


#### Tags:

 - Chat, Completions, LLM, AI

#### Properties

- [Documentation](https://docs.litellm.ai/docs/completion)
- [GettingStarted](https://docs.litellm.ai/docs/proxy/quick_start)

### LiteLLM Completions API
Provides an OpenAI-compatible /completions endpoint for text completion requests routed through the LiteLLM proxy to supported LLM providers.

**Human URL:** [https://docs.litellm.ai/docs/text_completion](https://docs.litellm.ai/docs/text_completion)


#### Tags:

 - Completions, Text, LLM

#### Properties

- [Documentation](https://docs.litellm.ai/docs/text_completion)

### LiteLLM Responses API
Provides an OpenAI-compatible /responses endpoint supporting the Responses API specification, including conversation history compression via /responses/compact.

**Human URL:** [https://docs.litellm.ai/docs/response_api](https://docs.litellm.ai/docs/response_api)


#### Tags:

 - Responses, AI, LLM

#### Properties

- [Documentation](https://docs.litellm.ai/docs/response_api)

### LiteLLM Embeddings API
Provides an OpenAI-compatible /embeddings endpoint for generating text embeddings across multiple providers including OpenAI, Cohere, HuggingFace, and Bedrock with unified formatting.

**Human URL:** [https://docs.litellm.ai/docs/embedding/supported_embedding](https://docs.litellm.ai/docs/embedding/supported_embedding)


#### Tags:

 - Embeddings, Vectors, AI

#### Properties

- [Documentation](https://docs.litellm.ai/docs/embedding/supported_embedding)

### LiteLLM Image Generation API
Provides OpenAI-compatible /images/generations, /images/edits, and /images/variations endpoints for image generation and manipulation routed through the LiteLLM proxy.

**Human URL:** [https://docs.litellm.ai/docs/image_generation](https://docs.litellm.ai/docs/image_generation)


#### Tags:

 - Images, Generation, AI

#### Properties

- [Documentation](https://docs.litellm.ai/docs/image_generation)

### LiteLLM Audio API
Provides OpenAI-compatible /audio/transcriptions and /audio/speech endpoints for audio transcription and text-to-speech conversion across supported providers.

**Human URL:** [https://docs.litellm.ai/docs/audio_transcription](https://docs.litellm.ai/docs/audio_transcription)


#### Tags:

 - Audio, Transcription, Speech, AI

#### Properties

- [Documentation](https://docs.litellm.ai/docs/audio_transcription)

### LiteLLM Moderations API
Provides an OpenAI-compatible /moderations endpoint for content moderation across supported providers through the LiteLLM proxy.

**Human URL:** [https://docs.litellm.ai/docs/moderation](https://docs.litellm.ai/docs/moderation)


#### Tags:

 - Moderation, Content, Safety

#### Properties

- [Documentation](https://docs.litellm.ai/docs/moderation)

### LiteLLM Batches API
Provides an OpenAI-compatible /batches endpoint for batch processing operations, enabling bulk request handling across LLM providers.

**Human URL:** [https://docs.litellm.ai/docs/batches](https://docs.litellm.ai/docs/batches)


#### Tags:

 - Batches, Bulk, Processing

#### Properties

- [Documentation](https://docs.litellm.ai/docs/batches)

### LiteLLM Files API
Provides an OpenAI-compatible /files endpoint for file management operations used in conjunction with fine-tuning and batch processing.

**Human URL:** [https://docs.litellm.ai/docs/files_endpoints](https://docs.litellm.ai/docs/files_endpoints)


#### Tags:

 - Files, Management

#### Properties

- [Documentation](https://docs.litellm.ai/docs/files_endpoints)

### LiteLLM Fine-Tuning API
Provides an OpenAI-compatible /fine_tuning endpoint for model fine-tuning operations across supported providers through the LiteLLM proxy.

**Human URL:** [https://docs.litellm.ai/docs/fine_tuning](https://docs.litellm.ai/docs/fine_tuning)


#### Tags:

 - Fine-Tuning, Models, Training

#### Properties

- [Documentation](https://docs.litellm.ai/docs/fine_tuning)

### LiteLLM Rerank API
Provides a /rerank endpoint for document reranking operations, supporting providers like Cohere through the LiteLLM proxy with a unified interface.

**Human URL:** [https://docs.litellm.ai/docs/rerank](https://docs.litellm.ai/docs/rerank)


#### Tags:

 - Rerank, Search, Relevance

#### Properties

- [Documentation](https://docs.litellm.ai/docs/rerank)

### LiteLLM Vector Stores API
Provides /vector_stores endpoints for creating and managing vector stores, file operations within vector stores, and search functionality for retrieval-augmented generation (RAG) use cases.

**Human URL:** [https://docs.litellm.ai/docs/vector_stores/create](https://docs.litellm.ai/docs/vector_stores/create)


#### Tags:

 - Vectors, Storage, RAG, Search

#### Properties

- [Documentation](https://docs.litellm.ai/docs/vector_stores/create)

### LiteLLM Anthropic Messages API
Provides Anthropic-compatible /v1/messages and /v1/messages/count_tokens endpoints for native Anthropic API format support through the LiteLLM proxy.

**Human URL:** [https://docs.litellm.ai/docs/anthropic_unified/](https://docs.litellm.ai/docs/anthropic_unified/)


#### Tags:

 - Anthropic, Messages, AI

#### Properties

- [Documentation](https://docs.litellm.ai/docs/anthropic_unified/)

### LiteLLM Realtime API
Provides /realtime WebSocket endpoints for real-time model interactions with load balancing and guardrails support across providers.

**Human URL:** [https://docs.litellm.ai/docs/realtime](https://docs.litellm.ai/docs/realtime)


#### Tags:

 - Realtime, WebSocket, Streaming

#### Properties

- [Documentation](https://docs.litellm.ai/docs/realtime)

### LiteLLM MCP API
Provides /mcp endpoints for Model Context Protocol (MCP) integration, enabling LLMs to interact with external tools and APIs through OpenAPI specifications.

**Human URL:** [https://docs.litellm.ai/docs/mcp](https://docs.litellm.ai/docs/mcp)


#### Tags:

 - MCP, Tools, Protocols

#### Properties

- [Documentation](https://docs.litellm.ai/docs/mcp)

### LiteLLM OCR API
Provides an /ocr endpoint for optical character recognition, enabling text extraction from images through supported providers via the LiteLLM proxy.

**Human URL:** [https://docs.litellm.ai/docs/ocr](https://docs.litellm.ai/docs/ocr)


#### Tags:

 - OCR, Images, Text Extraction

#### Properties

- [Documentation](https://docs.litellm.ai/docs/ocr)

### LiteLLM Guardrails API
Provides /guardrails/apply_guardrail endpoint for applying configured content filtering and safety guardrails to LLM requests and responses.

**Human URL:** [https://docs.litellm.ai/docs/apply_guardrail](https://docs.litellm.ai/docs/apply_guardrail)


#### Tags:

 - Guardrails, Safety, Content Filtering

#### Properties

- [Documentation](https://docs.litellm.ai/docs/apply_guardrail)

### LiteLLM Evals API
Provides /evals endpoints for the Evaluations API, enabling measurement and benchmarking of model performance through the LiteLLM proxy.

**Human URL:** [https://docs.litellm.ai/docs/evals_api](https://docs.litellm.ai/docs/evals_api)


#### Tags:

 - Evaluations, Benchmarks, Performance

#### Properties

- [Documentation](https://docs.litellm.ai/docs/evals_api)

### LiteLLM A2A Agent Gateway API
Provides /a2a endpoints for the Agent-to-Agent (A2A) gateway, enabling agent registration, publishing, and inter-agent communication.

**Human URL:** [https://docs.litellm.ai/docs/a2a](https://docs.litellm.ai/docs/a2a)


#### Tags:

 - Agents, A2A, Gateway

#### Properties

- [Documentation](https://docs.litellm.ai/docs/a2a)

### LiteLLM Videos API
Provides /videos endpoints for video generation and handling through supported providers like RunwayML via the LiteLLM proxy.

**Human URL:** [https://docs.litellm.ai/docs/videos](https://docs.litellm.ai/docs/videos)


#### Tags:

 - Videos, Generation, AI

#### Properties

- [Documentation](https://docs.litellm.ai/docs/videos)

## Common Properties

- [Portal](https://www.litellm.ai/)
- [Documentation](https://docs.litellm.ai/docs/)
- [GettingStarted](https://docs.litellm.ai/docs/proxy/quick_start)
- [GitHubOrg](https://github.com/BerriAI/litellm)
- [Blog](https://docs.litellm.ai/blog)
- [ChangeLog](https://www.litellm.ai/changelog)
- [ReleaseNotes](https://docs.litellm.ai/release_notes)
- [Status](https://status.litellm.ai/)
- [Support](https://www.litellm.ai/support)
- [Pricing](https://docs.litellm.ai/docs/enterprise)
- [Dashboard](https://admin.litellm.ai/)
- [Providers](https://docs.litellm.ai/docs/providers)
- [Models](https://models.litellm.ai/)
- [Configuration](https://docs.litellm.ai/docs/proxy/configs)
- [Authentication](https://docs.litellm.ai/docs/set_keys)
- [Guardrails](https://docs.litellm.ai/docs/apply_guardrail)
- [Enterprise](https://docs.litellm.ai/docs/proxy/enterprise)
- [ReleaseCycle](https://docs.litellm.ai/docs/proxy/release_cycle)
- [SSO](https://docs.litellm.ai/docs/proxy/admin_ui_sso)
- [Docker](https://docs.litellm.ai/docs/proxy/docker_quick_start)
- [PyPI](https://pypi.org/project/litellm/)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
