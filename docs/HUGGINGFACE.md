# 🤗 Hugging Face Integration

> Connect Hugging Face Inference API and Hugging Face Spaces to AAA Infinity AI.

## Purpose

Hugging Face provides access to thousands of open-source AI models.

Ari AI automatically uses Hugging Face when the requested task matches an available model or Space.

---

## Components

### Hugging Face Inference API

Used for

- Text Generation
- Image Generation
- Video Generation
- Audio Processing
- Embeddings

---

### Hugging Face Spaces

Used for

- Gradio Apps
- AI Demos
- Image Generation
- Video Generation
- OCR
- Speech
- Custom AI Applications

---

## Authentication

Stored securely using Infisical.

Environment Variable

HF_TOKEN

Never expose tokens in frontend code.

---

## Ari AI Integration

User

↓

Ari AI

↓

Intent Detection

↓

Hugging Face Connector

↓

Inference API or Spaces

↓

Result

---

## Supported Features

- Image Generation
- Video Generation
- Image-to-Image
- Text-to-Image
- Speech Recognition
- Text-to-Speech
- OCR
- Background Removal
- Upscaling
- Captioning

---

## Hugging Face Spaces Connector

The connector can

- Save favorite Spaces
- Connect using Space ID
- Detect Gradio APIs
- Monitor Space status
- Retry failed requests
- Switch between Spaces

---

## Example Space IDs

username/my-space

organization/video-generator

organization/image-generator

---

## Error Handling

If a Space is unavailable

- Retry request
- Suggest another configured Space
- Show status to the user

---

## Future

- Automatic Space Discovery
- Space Marketplace
- Workflow Integration
- Queue Monitoring
- Space Health Checks

