# RAG College Study Assistant

## 📌 Project Overview

This project is a Retrieval-Augmented Generation (RAG) based college study assistant built using n8n.

The system allows college study material in PDF format to be processed and stored as vector embeddings. Students can then ask academic questions through a chatbot, which retrieves relevant information from the uploaded study material before generating a response.

The project consists of two workflows: one for ingesting and embedding the study material, and another for retrieving the relevant information and answering student queries.

## ⚙️ Workflow

### 1. RAG Ingestion Workflow

### Workflow Flow

Google Drive → PDF Filter → Download PDF → Extract Text → Data Loader → Gemini Embeddings → Simple Vector Store

The ingestion workflow searches for files in a specified Google Drive folder and filters the files to process only PDF documents.

The selected PDF is downloaded and its text is extracted. The extracted content is then processed using a data loader, converted into vector embeddings using Google Gemini Embeddings, and stored in the n8n Simple Vector Store.

Source information is also stored as metadata so that the chatbot can identify the study material used for generating an answer.

### 2. RAG Chatbot Workflow

### Workflow Flow

Chat Trigger → AI Agent → Simple Vector Store → Google Gemini

The chatbot receives the student's question through the Chat Trigger.

The AI Agent uses the Simple Vector Store as a retrieval tool to search for relevant information from the uploaded study material. The retrieved information is then used by the Google Gemini model to generate the response.

Simple Memory is also used to maintain conversational context during the interaction.

## 🛠️ Technologies Used

- n8n
- Retrieval-Augmented Generation (RAG)
- Google Drive
- Google Gemini
- Gemini Embeddings
- Simple Vector Store
- AI Agent
- Simple Memory
- PDF Processing

## ✨ Key Features

- Processes college study material in PDF format
- Retrieves PDF files from Google Drive
- Extracts text from PDF documents
- Generates vector embeddings using Google Gemini
- Stores embeddings in n8n Simple Vector Store
- Uses an AI Agent for question answering
- Retrieves relevant information before generating answers
- Uses source metadata for identifying the study material
- Maintains conversational context using Simple Memory
- Reduces unsupported answers by restricting responses to the uploaded study material

## 🔐 Setup

Before running the workflows, configure the following in n8n:

- Google Drive credentials
- Google Gemini credentials
- Google Drive folder containing the study material
- Required PDF documents
- Simple Vector Store configuration

### Ingestion Workflow

1. Configure your Google Drive credentials.
2. Replace the Google Drive folder ID with your own folder ID.
3. Place the required college study material PDFs inside the folder.
4. Import `rag-ingestion.json` into n8n.
5. Execute the ingestion workflow to process the PDFs and generate embeddings.

### Chatbot Workflow

1. Configure your Google Gemini credentials.
2. Import `rag-chatbot.json` into n8n.
3. Ensure the chatbot is connected to the same Simple Vector Store used during ingestion.
4. Open the chat interface and ask questions related to the uploaded study material.

Replace any placeholder values in the JSON files with your own configuration before running the workflows.

## 📂 Project Structure

```text
15-rag-college-study-assistant/
│
├── rag-ingestion.json
├── rag-chatbot.json
├── README.md
│
└── screenshots/
    ├── rag-ingestion.png
    └── rag-chatbot.png