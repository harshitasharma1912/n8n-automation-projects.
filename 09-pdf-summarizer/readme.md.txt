# 📄 PDF Summarizer

## 📌 Project Overview

This project automates the process of summarizing a PDF document using n8n and an AI language model.

The workflow retrieves a PDF from a provided URL, processes it using an LLM, generates a summarized version with bullet points and proper spacing, and sends the final summary through Gmail.

## ⚙️ Workflow

### Workflow Flow

Manual Trigger → HTTP Request → Basic LLM Chain → Gmail

The workflow starts manually, retrieves the PDF using an HTTP Request, sends the document to the AI language model for summarization, and delivers the generated summary through Gmail.

## 🤖 AI Summarization

The AI is instructed to:

* Summarize the document
* Present the summary using bullet points
* Maintain clear spacing for readability

## 🛠️ Technologies Used

* n8n
* HTTP Request
* Groq
* LLM Chain
* Gmail
* PDF

## ✨ Key Features

* Retrieves a PDF from a URL
* Uses an AI language model for summarization
* Generates a structured summary
* Uses bullet points for better readability
* Automatically sends the summary through Gmail
* Demonstrates AI-powered document processing and workflow automation

## 📂 Project Structure

```text
09-pdf-summarizer/
│
├── pdf-summarizer.json
├── README.md
└── screenshots/
    └── workflow.png
```

## 🔐 Setup

Before running the workflow, configure your own:

* Groq API credentials
* Gmail credentials
* PDF source URL
* Recipient Gmail address

Replace the placeholder values in the JSON file with your own credentials and configuration.
