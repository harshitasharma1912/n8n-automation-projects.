# PDF Translation in Slack

## 📌 Project Overview

This project automates the process of translating a PDF document using n8n.

The workflow retrieves a PDF from a given URL, uses Google Gemini to translate the content into Punjabi and Hindi, generates a concise Punjabi summary, converts the processed content into a PDF, and uploads the final PDF to a Slack channel.

## ⚙️ Workflow

### Workflow Flow

Manual Trigger → HTTP Request → Google Gemini → Code in JavaScript → PDFShift API → Slack

The workflow starts manually, retrieves the PDF using an HTTP Request, processes the content using Google Gemini, formats the translated content using JavaScript, converts it into a PDF using PDFShift, and uploads the generated PDF to Slack.

## 🛠️ Technologies Used

- n8n
- Google Gemini
- Slack
- PDFShift API
- HTTP Request
- JavaScript
- REST API

## ✨ Key Features

- Retrieves a PDF from a URL
- Translates PDF content into Punjabi and Hindi
- Generates a concise Punjabi summary
- Uses Google Gemini for AI-powered translation
- Converts the processed content into a PDF
- Automatically uploads the generated PDF to Slack
- Demonstrates AI, API, PDF processing, and Slack integration

## 📂 Project Structure

```text
11-pdf-translation-slack/
│
├── pdf-translation-slack.json
├── README.md
└── screenshots/
    └── workflow.png