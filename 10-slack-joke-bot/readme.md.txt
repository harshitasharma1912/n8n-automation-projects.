# Slack Joke Bot

## 📌 Project Overview

This workflow automates the process of retrieving information from an external API and sending the processed data as a message to a Slack channel.

A Manual Trigger starts the workflow whenever it is executed. The HTTP Request node fetches the required data from the API, after which the Edit Fields node extracts and formats only the relevant information. Finally, the processed data is posted automatically to the configured Slack channel using the Slack (Send a Message) node.

## ⚙️ Workflow

### Workflow Flow

Manual Trigger → HTTP Request → Edit Fields → Slack (Send a Message)

The workflow demonstrates how an external API can be integrated with Slack to automate notifications and information sharing.

## 🛠️ Technologies Used

* n8n
* Slack
* JokeAPI
* HTTP Request
* REST API

## ✨ Key Features

* Retrieves data from an external API
* Processes the API response using the Edit Fields node
* Automatically sends the processed data to a Slack channel
* Demonstrates REST API integration
* Demonstrates Slack integration
* Reduces manual effort in information sharing

## 📂 Project Structure

```text
10-slack-joke-bot/
│
├── slack-joke-bot.json
├── README.md
└── screenshots/
    └── workflow.png
```

## 🔐 Setup

Before running the workflow, configure your own Slack credentials and select the required Slack channel.

The JokeAPI used in this workflow does not require an API key for the configured request.
