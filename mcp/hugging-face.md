# Hugging Face MCP

**Provider:** claude.ai  
**Status:** △ needs authentication  
**Type:** ML Models / Datasets / Hub

## Overview

Hugging Face MCP connects Claude to the Hugging Face Hub, enabling model search, dataset exploration, inference API calls, and repository management. Requires authentication with a Hugging Face account or token.

## Authentication

```
Step 1: Run authenticate tool → prompts for HF token or OAuth
Step 2: Complete sign-in / paste token
Step 3: Run complete_authentication tool → confirms connection
```

Get your token at: https://huggingface.co/settings/tokens

## Available Tools (post-auth)

| Tool | Description |
|------|-------------|
| `authenticate` | Initiate Hugging Face authentication |
| `complete_authentication` | Finalize the authentication handshake |

Once authenticated, Claude gains access to Hub operations including:
- Searching models, datasets, and Spaces by task/framework/license
- Reading model cards, dataset previews, and Space descriptions
- Running inference via the Inference API
- Managing repositories (create, push files, update README)
- Accessing private repos and gated models you have access to

## Usage Examples

```
Find the best open-source text-to-image model under 10GB

Run inference on mistralai/Mistral-7B-Instruct-v0.2 with my prompt

Show me the dataset card for HuggingFaceH4/ultrachat_200k

Create a new model repo called my-org/my-fine-tuned-llm
```

## Notes

- Free-tier Inference API has rate limits; Pro tier or dedicated endpoints remove them
- Gated models (e.g., Meta Llama) require prior access approval on HF
- Write access to repos requires a token with write scope
