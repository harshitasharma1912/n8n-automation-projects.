# AI Content & Image Generation

## 📌 Project Overview

This project automates the process of generating LinkedIn content and an AI-generated image using n8n.

The workflow takes a topic, target audience, and platform as input, uses Groq to generate a LinkedIn caption, hashtags, and an image prompt, then uses Hugging Face to generate an image and sends the final image with the generated caption to Telegram.

## ⚙️ Workflow

### Workflow Flow

Schedule Trigger → Edit Fields → Groq → Code in JavaScript → Hugging Face → Telegram

The workflow runs automatically according to the configured schedule, prepares the content details, generates LinkedIn content and an image prompt using Groq, processes the AI response using JavaScript, generates an image using Hugging Face, and sends the generated image with the caption to Telegram.

## 🛠️ Technologies Used

- n8n
- Groq
- Hugging Face
- Telegram
- JavaScript
- REST API

## ✨ Key Features

- Automatically generates LinkedIn content
- Uses AI to generate captions and hashtags
- Generates an AI image prompt
- Creates an image using Hugging Face
- Sends the generated image and caption to Telegram
- Uses scheduled workflow automation
- Demonstrates AI content generation and image generation

## 📂 Project Structure

```text
11-ai-content-image-generation/
│
├── ai-content-image-generation.json
├── README.md
└── screenshots/
    └── workflow.png