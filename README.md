# PDF Answering Chatbot

## Problem Statement
Accessing information from lengthy PDF documents can be time-consuming and inefficient. This project aims to build an intelligent chatbot that can understand and answer questions based on the content of PDF files. It provides quick, relevant responses by extracting and processing the document's text, improving productivity and user experience.

## Tech Stack
- **Python** – Core programming language  
- **LangChain** – For document processing and chaining LLM calls  
- **FAISS** – Vector similarity search for efficient document retrieval  
- **CTransformers** – Lightweight large language model integration  
- **Streamlit** – Web-based user interface for easy interaction

Using LLaMA 2 7B Model from Hugging Face
This project uses the LLaMA 2 7B model to power the chatbot’s language understanding and response generation.

Steps to Download and Use LLaMA 2 7B:
Create a Hugging Face account (if you don’t have one):
https://huggingface.co/join

Accept the LLaMA 2 model license on Hugging Face:
Visit https://huggingface.co/meta-llama/Llama-2-7b-chat-hf and agree to the terms.

Install the huggingface_hub Python package (if not installed):

bash
Copy
Edit
pip install huggingface_hub
Login to Hugging Face from your terminal:

bash
Copy
Edit
huggingface-cli login
This will prompt you to enter your Hugging Face API token, which you can get from your Hugging Face account settings.

Download or load the model programmatically:

You can load the model using libraries like transformers or your specific LLM framework (e.g., CTransformers) by providing the model path "meta-llama/Llama-2-7b-chat-hf".

Example with transformers:

python
Copy
Edit
from transformers import AutoModelForCausalLM, AutoTokenizer

model_name = "meta-llama/Llama-2-7b-chat-hf"
tokenizer = AutoTokenizer.from_pretrained(model_name)
model = AutoModelForCausalLM.from_pretrained(model_name)
Ensure you have enough VRAM or use CPU fallback
LLaMA 2 7B requires a GPU with at least 12-16GB VRAM for efficient inference.  

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
