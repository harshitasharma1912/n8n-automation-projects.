# 💼 Jobs Alert System

## 📌 Project Overview

This project automates the process of checking job listings and sending relevant job alerts through Telegram using n8n.

The workflow retrieves job data from Google Sheets, filters the listings based on the required role and location, uses Google Gemini to generate a short job summary, and sends the alert to Telegram.

## ⚙️ Workflow

### Workflow Flow

Schedule Trigger → Google Sheets → IF → Google Gemini → Telegram

The workflow runs automatically at a scheduled interval, retrieves job listings from Google Sheets, checks whether the job matches the required role and location, generates a concise summary using Google Gemini, and sends the job alert through Telegram.

## 🛠️ Technologies Used

* n8n
* Google Sheets
* Google Gemini
* Telegram
* Google APIs

## ✨ Key Features

* Automatically checks job listings on a scheduled basis
* Retrieves job data from Google Sheets
* Filters jobs based on role and location
* Uses Google Gemini for AI-based job summarization
* Sends job alerts directly to Telegram
* Reduces manual effort in monitoring job opportunities
* Demonstrates AI integration with workflow automation

## 📂 Project Structure

```text
06-jobs-alert-system/
│
├── jobs-alert-system.json
├── README.md
└── screenshots/
    └── workflow.png
```

## 🔐 Setup

Before running the workflow, configure your own:

* Google Sheets credentials
* Google Gemini credentials/API access
* Telegram credentials
* Google Sheet ID
* Telegram Chat ID

Replace the placeholder values in the JSON file with your own credentials and configuration.
