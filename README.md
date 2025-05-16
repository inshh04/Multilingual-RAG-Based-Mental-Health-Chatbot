# Multilingual Mental Health Chatbot — Embedding & Retrieval Pipeline

## 🧠 Overview

This project implements a Retrieval-Augmented Generation (RAG)-based chatbot for **mental health awareness** in **English and Urdu**. It leverages multilingual embeddings and vector similarity search to retrieve semantically relevant chunks from preprocessed documents.

## 🔧 Features

- 📚 Preprocessing and chunking of bilingual data
- 🌐 Embedding using Sentence-BERT and DistilBERT multilingual models
- 📦 Vector storage and similarity search with Pinecone
- 🧪 Scripts for similarity queries and manual evaluation

## 📂 Repository Contents

- `mentalhealth_multilingualchatbot.py` — Full implementation script
- `mental_health_en.pdf` — English source document (WHO)
- `mental_health_ur.pdf` — Urdu (manual translation of English)
- `README.md` — Project overview and usage guide

## 🚀 Setup Instructions

1. **Clone the repo:**
   ```bash
   git clone https://github.com/yourusername/mental-health-chatbot.git
   cd mental-health-chatbot

**▶️ Run the script:**
    Use Google Colab or any Python environment
    Edit your Pinecone API key and region in the script

**💬 Usage:**
  Loads and chunks mental health documents in two languages
  Embeds text using two different models
  Stores vectors in Pinecone for similarity-based retrieval
  Supports English and Urdu queries for semantic evaluation


**📊 Evaluation Summary:**
Manual similarity search results showed:
    ✅ DistilBERT performs better on Urdu queries
    ✅ SBERT is stronger for semantic search in English
    ✅ The Urdu document was manually translated from the English source to maintain semantic consistency
    ❗ SBERT returned lower similarity scores (~0.17) on English queries
    ✅ DistilBERT achieved high accuracy (up to 0.83) for Urdu semantic matching


