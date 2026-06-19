

# RAG Knowledge Base Chatbot with n8n
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/2a0212f8-a95c-4d9b-ba07-916a8926802f" />

## Overview

This project demonstrates a modular Retrieval-Augmented Generation (RAG) support agent built with **n8n** and **MongoDB Vector Search**.

The goal is to enable AI assistants to answer questions using only approved business documentation, reducing unsupported responses by grounding every answer in retrieved context from the knowledge base.

The architecture is designed to be modular, extensible, and suitable for customer support, internal knowledge bases, and document-driven AI assistants.

---

## Features

* Retrieval-Augmented Generation (RAG)
* Modular n8n workflow architecture
* MongoDB Vector Store integration
* Semantic document retrieval
* Context-aware response generation
* Restricts responses to retrieved knowledge
* Easily adaptable to PDF and document-based support systems
* Compatible with OpenAI-compatible language models

---

## Architecture

```
                User Query
                     │
                     ▼
             n8n Orchestration
                     │
         ┌───────────┴───────────┐
         │                       │
         ▼                       ▼
Generate Embedding      Workflow Logic
         │
         ▼
MongoDB Vector Store
         │
         ▼
Relevant Context Retrieval
         │
         ▼
      Language Model
         │
         ▼
 Grounded AI Response
```

---

## Technology Stack

* n8n
* MongoDB Vector Store
* OpenAI-compatible LLM
* Vector Embeddings
* REST APIs
* Retrieval-Augmented Generation (RAG)

---

## Workflow Design Goals

The workflow is designed to:

* Retrieve only relevant knowledge before generation
* Improve factual consistency by grounding responses in stored documents
* Maintain a modular architecture for easy customization
* Support scalable automation pipelines and future integrations

---

## Setup

1. Import `Sanitized_workflow.json` into your n8n instance.
2. Configure your MongoDB credentials.
3. Configure your preferred LLM provider.
4. Connect your vector store.
5. Execute the workflow.

---

## Repository Contents

* `Sanitized_workflow.json` — Sanitized n8n workflow
* `README.md` — Project documentation

---

## Future Enhancements

* Multi-document support
* Source citation display
* Metadata filtering
* Hybrid retrieval
* Reranking
* Role-based document access
* Conversation memory
* Advanced analytics

---

## Author

**Isaac Lamptey**

AI Automation Developer specializing in **n8n**, **OpenAI integrations**, and **Retrieval-Augmented Generation (RAG)** systems.
