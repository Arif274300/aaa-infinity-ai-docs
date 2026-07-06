# System Architecture

```mermaid
graph TD

User --> Ari

Ari --> Router

Router --> OpenRouter

Router --> HuggingFace

Router --> HuggingFaceSpaces

Router --> GoogleColab

GoogleColab --> ComfyUI

Router --> Cloudflare

Cloudflare --> Infisical

Ari --> Gallery

Ari --> Projects

Ari --> PromptStudio

Ari --> WorkflowEngine
