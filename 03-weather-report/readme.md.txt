# 🌤️ Weather Report Automation

## 📌 Project Overview

This project automates the process of retrieving weather information for a selected city and sending a daily weather report through Gmail using n8n.

The workflow uses the OpenWeather API to fetch current weather data, processes the required information, and sends it as an email.

## ⚙️ Workflow

### Workflow Flow

Schedule Trigger → HTTP Request → Edit Fields → Gmail

The workflow runs automatically according to the configured schedule, retrieves weather data from the OpenWeather API, formats the required information, and sends the weather report through Gmail.

## 🛠️ Technologies Used

* n8n
* OpenWeather API
* Gmail
* REST API

## ✨ Key Features

* Automatically retrieves weather information
* Uses the OpenWeather API
* Processes temperature, pressure, and humidity data
* Generates a formatted weather report
* Sends the report through Gmail
* Demonstrates API integration and workflow automation

## 📂 Project Structure

```text
03-weather-report/
│
├── weather-report.json
├── README.md
└── screenshots/
    └── workflow.png
```
