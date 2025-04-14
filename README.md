# RAG Evaluation App (Gemini-powered)

This repository contains a portfolio project demonstrating a Retrieval-Augmented Generation (RAG) system built using Google Gemini, FAISS, and Sentence Transformers. The application compares different RAG strategies—including module-based methods (hybrid retrieval, reranker, metadata filtering) and prompt-based techniques (chain-of-thought, role-based prompting)—and evaluates their performance using simulated metrics. An optional LLM-based evaluation provides qualitative feedback on the responses.

## Features

- **Google Gemini Integration:** Uses Google Gemini (model: `models/gemini-2.0-flash`) for generating responses.
- **Vector-Based Retrieval:** Leverages FAISS in combination with Sentence Transformers for efficient context retrieval.
- **Data Set:** Uses a static context text about the **American Revolution** (covering its causes, key figures, battles, and outcomes) to simulate historical information retrieval.
- **Multiple RAG Techniques:**  
  - **Module-based:** Options include hybrid retrieval, reranker enhancement, and metadata filtering (filters based on keywords like "American" and "Revolution").
  - **Prompt-based:** Techniques such as chain-of-thought (CoT) prompting and role-based prompting (e.g., "Imagine you are a historian specializing in the American Revolution.") are supported.
- **Simulated Evaluation Metrics:** The system reports simulated metrics:
  - *Faithfulness* – How closely the generated answer matches the retrieved context.
  - *Relevance* – How directly the answer addresses the input question.
  - *Context Precision* – How focused or on-target the retrieved context is.
- **Optional LLM Evaluation:** An experimental feature that optionally provides a qualitative review of the generated answers.
- **User-Friendly Interface:** Built with Streamlit for an interactive web-based demonstration.

## Installation

### 1. Clone or Download the Repository
Clone this repository via Git:
```bash
git clone https://github.com/your-username/your-repo-name.git

2. Navigate to the Project Directory
cd TEG_RAG_Gemini_Portfolio

3. Create a Virtual Environment
python -m venv rag_env
Activate the Virtual Environment
.\rag_env\Scripts\Activate.ps1

#Install the Dependencies
#Install the required Python packages with:
pip install -r requirements.txt

Set Up Your Gemini API Key
GOOGLE_API_KEY="your_google_gemini_api_key_here"

Usage
streamlit run app_advanced_en.py

