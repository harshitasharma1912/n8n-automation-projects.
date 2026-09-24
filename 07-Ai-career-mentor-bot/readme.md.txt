# 🤖 AI Career Mentor Bot

## 📌 Project Overview

This project is an AI-powered career mentor chatbot built using n8n.

The workflow allows users to interact with an AI Career Mentor through Telegram. It uses a skills database stored in Google Sheets and an AI Agent powered by a Groq language model to provide guidance on career roadmaps, skill gap analysis, learning plans, and interview preparation.

## ⚙️ Workflow

### Workflow Flow

Telegram Trigger → Google Sheets → AI Agent → Telegram

The workflow receives a user's message through Telegram, retrieves information from the skills database, processes the request using the AI Agent, and sends the generated response back to the user through Telegram.

The AI Agent also uses Simple Memory to maintain conversational context during the interaction.

## 🛠️ Technologies Used

* n8n
* Telegram
* Google Sheets
* Groq
* AI Agent
* Simple Memory

## ✨ Key Features

* AI-powered career guidance
* Telegram-based chatbot interaction
* Career roadmap assistance
* Skill gap analysis
* Personalized learning plans
* Interview preparation support
* Skills database integration using Google Sheets
* Conversational memory using Simple Memory
* Automated response generation using an AI Agent

## 📂 Project Structure

```text
07-ai-career-mentor-bot/
│
├── ai-career-mentor-bot.json
├── README.md
└── screenshots/
    └── workflow.png
```

## 🔐 Setup

Before running the workflow, configure your own:

* Telegram credentials
* Groq API credentials
* Google Sheets credentials
* Google Sheets ID
* Skills database

Replace the placeholder values in the JSON file with your own credentials and configuration.
