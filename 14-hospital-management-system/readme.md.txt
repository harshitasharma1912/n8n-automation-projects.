# Hospital Management System

## 📌 Project Overview

This project automates hospital appointment management using n8n.

The workflow receives appointment requests through a Webhook, stores appointment details in Firebase Cloud Firestore, sends confirmation emails to patients and notifications to the admin, handles appointment status updates, and provides an AI-powered hospital assistant for hospital-related queries.

## ⚙️ Workflow

### Workflow Flow

Appointment Webhook → Firestore → Gmail Notifications

Status Webhook → Firestore → Google Gemini → Response

Chatbot Webhook → Google Gemini → Response

The workflow receives appointment requests through a Webhook, processes the submitted information, stores the appointment data in Firestore, and sends confirmation emails to the patient and admin.

It also handles appointment status updates and retrieves appointment information using the patient's email address.

A separate hospital assistant uses Google Gemini to answer hospital-related questions and returns the response through a Webhook.

## 🛠️ Technologies Used

- n8n
- Firebase Cloud Firestore
- Gmail
- Google Gemini
- Webhook
- JavaScript

## ✨ Key Features

- Receives appointment requests through a Webhook
- Stores appointment data in Firebase Firestore
- Sends confirmation emails to patients
- Sends appointment notifications to the admin
- Handles appointment approval and rejection
- Retrieves appointment information using email
- Provides an AI-powered hospital assistant
- Answers hospital-related queries using Google Gemini
- Demonstrates Webhook, database, email, and AI integration

## 🔐 Setup

Before running the workflow, configure the following in n8n:

- Firebase Cloud Firestore credentials
- Firebase project ID and `appointments` collection
- Gmail credentials
- Google Gemini credentials
- Webhook URLs for appointment and chatbot requests

Replace the placeholder values in the JSON file with your own configuration.

Import the JSON file into n8n, configure the required credentials and webhook settings, and activate the workflow.

## 📂 Project Structure

```text
14-hospital-management-system/
│
├── hospital-management-system.json
├── README.md
└── screenshots/
    └──appointment-workflow.png
    └── chatbot-workflow.png