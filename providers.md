---
layout: default
title: Providers
nav_order: 5
permalink: /providers/
---

# Providers

Limitcode supports these providers:

- OpenAI
- DeepSeek
- Anthropic
- Gemini
- OpenRouter
- Moonshot AI (Kimi)
- Ollama
- LM Studio
- Llamafile

Cloud providers require an API key. Ollama, LM Studio, and Llamafile run locally without a cloud API key. Model lists are fetched from each provider's models endpoint and use a cached fallback when needed.

To configure a provider, run **Limitcode: Setup Provider API Key** from the Command Palette, then select a provider and model in the Limitcode chat.

## Local models

For local inference, start Ollama, LM Studio, or Llamafile before opening a chat. Configure the provider's base URL when the default endpoint does not match your local setup (Llamafile defaults to `http://127.0.0.1:8080`).

## Provider-specific settings

Use `provider_base_urls` for custom or self-hosted OpenAI-compatible endpoints:

```json
{
    "provider_base_urls": {
        "openai_compatible": "http://localhost:1234/v1"
    }
}
```
