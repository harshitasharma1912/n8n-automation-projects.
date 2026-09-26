# SQL Webhook Logger

## 📌 Project Overview

This project automates the process of capturing data received through a Webhook and storing it in a MySQL database using n8n.

The workflow receives student data through a POST request, stores the information in a MySQL table, and sends a confirmation email after the data is successfully inserted.

## ⚙️ Workflow

### Workflow Flow

Webhook → MySQL → Gmail

The workflow starts when a POST request is received through the Webhook node. The incoming data is then inserted into a MySQL table, after which a confirmation email containing the received student information is sent through Gmail.

## 🛠️ Technologies Used

- n8n
- Webhook
- MySQL
- Gmail
- REST API

## ✨ Key Features

- Receives data through a Webhook
- Supports POST requests
- Stores received data in a MySQL database
- Sends a confirmation email after successful insertion
- Automates data collection and notification
- Demonstrates Webhook, database, and email integration

## 📂 Project Structure

```text
13-sql-webhook-logger/
│
├── sql-webhook-logger.json
├── README.md
└── screenshots/
    └── workflow.png