# PDF Answering Chatbot

## Problem Statement
Accessing information from lengthy PDF documents can be time-consuming and inefficient. This project aims to build an intelligent chatbot that can understand and answer questions based on the content of PDF files. It provides quick, relevant responses by extracting and processing the document's text, improving productivity and user experience.

## Tech Stack
- **Python** – Core programming language  
- **LangChain** – For document processing and chaining LLM calls  
- **FAISS** – Vector similarity search for efficient document retrieval  
- **CTransformers** – Lightweight large language model integration  
- **Streamlit** – Web-based user interface for easy interaction  

## Features
- Upload PDF documents and extract text content automatically  
- Split large documents into manageable chunks for better processing  
- Create semantic embeddings for each chunk using sentence transformers  
- Store embeddings in a FAISS vector store for fast similarity search  
- Interactive chatbot UI to ask questions and get accurate answers  
- Conversation memory to maintain context during a chat session  

## How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/SriTarunika10/PDF-answering-chatbot.git
   cd PDF-answering-chatbot
