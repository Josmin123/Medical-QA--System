# Medical-QA System: AI-Powered Medical Chatbot
## Overview
Medical-QA System is an AI-powered chatbot designed to answer medical queries efficiently using Llama 2, Pinecone, and LangChain. This chatbot transforms static PDF-based medical knowledge into an interactive experience, enabling users to get reliable health-related answers instantly—all while running on a CPU-friendly setup.

### Features
✅ Powered by Llama 2 – Utilizes Meta’s open-source language model for advanced language understanding.

✅ PDF to Chatbot – Converts static medical documents (e.g., Gale Encyclopedia of Medicine) into a searchable AI assistant.

✅ Embeddings with Pinecone – Uses Pinecone as a cloud-based vector database for scalable and fast document retrieval.

✅ CPU-Friendly – Runs without requiring expensive GPUs.

✅ User-Friendly Interface – Built with Chainlit for seamless interactions.


### How It Works
Extracting Knowledge from PDFs 📄

Medical documents are converted into text using pymupdf.

The text is split into smaller chunks using LangChain.

Creating and Storing Embeddings 🔍

Text chunks are embedded using all-MiniLM-L6-v2 from sentence-transformers.

Embeddings are stored in Pinecone, a scalable, cloud-based vector database optimized for similarity search.

Retrieving Answers Using Llama 2 🤖

When a user asks a medical question, the system retrieves the most relevant embeddings from Pinecone.

Llama 2 processes the retrieved data to generate a structured response.

Interactive Chatbot Interface 💬

Built with Chainlit, allowing users to interact with the chatbot smoothly.


Future Improvements 🚀

🔹 Enhancing Accuracy – Reducing AI hallucinations for better reliability.

🔹 Improving Security – Implementing guardrails to ensure privacy in medical queries.

🔹 Expanding Knowledge Base – Adding more medical sources to improve responses.
