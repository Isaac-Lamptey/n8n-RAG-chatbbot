RAG Chatbot Architecture
This repository contains a modular n8n workflow for a RAG-based knowledge base agent, built to ensure hallucination-free responses by scoping an LLM strictly to provided documentation.

Key Components
Orchestration: n8n

Vector Storage: mogoDB vector store

Logic: Custom RAG pipeline ensuring data integrity and restricted context retrieval.

How to Use
Import workflow.json into your n8n instance.

Configure your environment variables for Supabase and your chosen LLM.

Connect your vector store to the retrieval node.

4. Commit and Push
In your terminal, run:

Bash
git init
git add .
git commit -m "Initial commit: Modular RAG chatbot architecture for client evaluation"
git branch -M main
git remote add origin [YOUR_GITHUB_REPO_URL]
git push -u origin main
