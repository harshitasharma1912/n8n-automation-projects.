# 🎓 AI Summarizer for Students

## 📌 Project Overview

This project is an AI-powered student morning assistant built using n8n.

The workflow collects a student's schedule, important emails, pending assignments, and a coding problem from different sources. It then combines this information and uses an AI Agent to generate a concise morning report, which is automatically sent to Telegram.

## ⚙️ Workflow

### Workflow Flow

Schedule Trigger → Calendar / Gmail / Google Sheets → Merge → AI Agent → Telegram

The workflow runs automatically at a scheduled time and collects:

* 📅 Events from Google Calendar
* 📧 Emails from Gmail
* 📝 Student tasks or assignments from Google Sheets
* 💻 A coding problem selected from a Google Sheets database

The collected information is merged and processed by the AI Agent to create a personalized student morning report.

## 🤖 AI-Generated Report

The AI Agent generates the report in the following format:

* 🌅 Good Morning
* 📅 Today's Schedule
* 📧 Important Emails
* 📝 Pending Assignments
* 💻 Coding Challenge
* 🎯 Today's Focus

## 🛠️ Technologies Used

* n8n
* Google Calendar
* Gmail
* Google Sheets
* Groq
* AI Agent
* Telegram
* JavaScript

## ✨ Key Features

* Automatically runs at a scheduled time
* Retrieves events from Google Calendar
* Collects recent emails from Gmail
* Retrieves student assignments from Google Sheets
* Selects a random coding problem
* Combines data from multiple sources
* Uses an AI Agent to generate a personalized morning summary
* Sends the final report through Telegram
* Demonstrates multi-source AI workflow automation

## 📂 Project Structure

```text
08-ai-summarizer-for-students/
│
├── ai-summarizer-for-students.json
├── README.md
└── screenshots/
    └── workflow.png
```

## 🔐 Setup

Before running the workflow, configure your own:

* Google Calendar credentials
* Gmail credentials
* Google Sheets credentials
* Groq API credentials
* Telegram credentials
* Google Sheet IDs
* Telegram Chat ID

Replace the placeholder values in the JSON file with your own credentials and configuration.
