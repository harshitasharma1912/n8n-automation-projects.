# ⏰ Cron Gmail Automation

## 📌 Project Overview

This project demonstrates how to automate email sending using a scheduled trigger in n8n.

The workflow uses a cron expression to run automatically at a configured time and sends an email through Gmail without requiring manual execution.

## ⚙️ Workflow

### Workflow Flow

Schedule Trigger → Gmail

The Schedule Trigger runs the workflow according to the configured cron schedule. Once triggered, the Gmail node automatically sends the configured email.

## 🛠️ Technologies Used

* n8n
* Gmail
* Cron Expression
* Google APIs

## ✨ Key Features

* Automatically triggers the workflow at a scheduled time
* Uses cron expressions for scheduling
* Sends emails automatically through Gmail
* Eliminates the need for manual workflow execution
* Demonstrates scheduled workflow automation using n8n

## 📂 Project Structure

```text
05-cron-gmail/
│
├── cron-gmail.json
├── README.md
└── screenshots/
    └── workflow.png
```
