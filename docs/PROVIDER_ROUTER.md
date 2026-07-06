# 🔀 Provider Router

> Automatically selects the best AI provider for each task.

## Purpose

The Provider Router is the decision engine of AAA Infinity AI.

Instead of asking users to manually choose an AI model, Ari AI sends the request to the most suitable provider.

## Supported Providers

### OpenRouter

Use Cases

- Chat
- Coding
- Vision
- Reasoning
- Long Context

---

### Hugging Face Spaces

Use Cases

- Image Generation
- Video Generation
- OCR
- Audio
- Custom AI Apps

---

### Hugging Face Inference

Use Cases

- Hosted Models
- Image Models
- Video Models
- Embeddings

---

### Google Colab

Use Cases

- ComfyUI
- Stable Diffusion
- SDXL
- LoRA
- ControlNet

---

### Cloudflare Workers

Responsibilities

- API Gateway
- Routing
- Rate Limiting
- Logging
- Security

---

### Infisical

Responsibilities

- API Keys
- Tokens
- Environment Variables
- Secret Rotation

---

## Routing Flow

User Request

↓

Ari AI

↓

Intent Detection

↓

Provider Selection

↓

Execution

↓

Response

↓

Gallery / History

---

## Provider Priority

### Chat

1. OpenRouter
2. Hugging Face (optional)

### Coding

1. OpenRouter

### Images

1. Google Colab
2. Hugging Face Spaces

### Videos

1. Hugging Face Spaces
2. Hugging Face Inference

---

## Error Handling

If a provider fails:

- Retry
- Switch Provider
- Notify User
- Log Error

---

## Future Features

- Automatic Benchmarking
- Cost Optimization
- Queue Management
- Parallel Execution
- Provider Health Monitor
