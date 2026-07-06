# 🌐 API Guide

> API architecture for AAA Infinity AI.

## Overview

AAA Infinity AI exposes a unified API through Cloudflare Workers.

Clients never communicate directly with AI providers.

---

# Architecture

Mobile App

↓

Cloudflare Worker

↓

Ari AI

↓

Provider Router

↓

AI Provider

↓

Response

---

# Authentication

Supported Methods

- API Key
- JWT (Future)
- OAuth (Future)

---

# Standard Request

POST /api/v1/chat

POST /api/v1/image

POST /api/v1/video

POST /api/v1/ocr

POST /api/v1/pdf

POST /api/v1/speech

---

# Chat Endpoint

POST /api/v1/chat

Responsibilities

- Detect intent
- Select provider
- Generate response
- Save history

---

# Image Endpoint

POST /api/v1/image

Responsibilities

- Improve prompt
- Select workflow
- Generate image
- Save gallery

---

# Video Endpoint

POST /api/v1/video

Responsibilities

- Select video provider
- Submit job
- Monitor progress
- Return video

---

# OCR Endpoint

POST /api/v1/ocr

Extract text from images.

---

# PDF Endpoint

POST /api/v1/pdf

Analyze PDF documents.

---

# Speech Endpoint

POST /api/v1/speech

Supports

- Speech to Text
- Text to Speech

---

# Error Format

Status

Message

Code

Provider

Timestamp

---

# Ari AI Responsibilities

- Validate Request
- Authenticate User
- Select Provider
- Retry Failed Requests
- Format Responses

---

# Future

- Streaming API
- WebSocket Support
- Batch Requests
- GraphQL API
- API Versioning
- SDKs

