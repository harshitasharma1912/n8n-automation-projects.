# 🎂 Birthday Wisher Automation

## 📌 Project Overview

This project automates the process of sending birthday wishes through Gmail using n8n.

The workflow checks the birthday information stored in Google Sheets and sends a personalized birthday email when the birthday matches the current date.

## ⚙️ Workflow

### Workflow Flow

Schedule Trigger → Google Sheets → IF → Gmail

The workflow runs automatically according to the configured schedule, retrieves birthday information from Google Sheets, checks whether the birthday matches the current date, and sends a birthday email when the condition is satisfied.

## 🛠️ Technologies Used

* n8n
* Google Sheets
* Gmail
* Google APIs

## ✨ Key Features

* Automatically checks birthday information
* Retrieves data from Google Sheets
* Compares the stored birthday with the current date
* Sends birthday wishes automatically through Gmail
* Reduces manual effort
* Demonstrates conditional logic and workflow automation

## 📂 Project Structure

```text
04-birthday-wisher/
│
├── birthday-wisher.json
├── README.md
└── screenshots/
    └── workflow.png
```
