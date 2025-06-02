# PDF Answering Chatbot

## Problem Statement
Accessing information from lengthy PDF documents can be time-consuming and inefficient. This project aims to build an intelligent chatbot that can understand and answer questions based on the content of PDF files. It provides quick, relevant responses by extracting and processing the document's text, improving productivity and user experience.

## Tech Stack
- **Python** – Core programming language  
- **LangChain** – For document processing and chaining LLM calls  
- **FAISS** – Vector similarity search for efficient document retrieval  
- **CTransformers** – Lightweight large language model integration  
- **Streamlit** – Web-based user interface for easy interaction

## Using LLaMA 2 7B Model from Hugging Face
This project uses the LLaMA 2 7B model to power the chatbot’s language understanding and response generation.

## Steps to Download and Use LLaMA 2 7B:
## 1. Create a Hugging Face account (if you don’t have one):
   https://huggingface.co/join

## 2.Accept the LLaMA 2 model license on Hugging Face:
Visit https://huggingface.co/meta-llama/Llama-2-7b-chat-hf and agree to the terms.

## 3. Install the huggingface_hub Python package (if not installed):
pip install huggingface_hub


## 4. Login to Hugging Face from your terminal:
huggingface-cli login
(Enter your API token from your Hugging Face account settings.)

## 5.Load the model in your Python code:
from transformers import AutoModelForCausalLM, AutoTokenizer
model_name = "meta-llama/Llama-2-7b-chat-hf"
tokenizer = AutoTokenizer.from_pretrained(model_name)
model = AutoModelForCausalLM.from_pretrained(model_name)
Ensure you have enough VRAM or use CPU fallback
LLaMA 2 7B requires a GPU with at least 12-16GB VRAM for efficient inference.  

## 6.Ensure your hardware meets the VRAM requirements (12-16GB GPU) or use CPU fallback with slower inference.

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

## For any questions or collaboration, feel free to contact:
Sri Tarunika
Email: sritarunikagunasekaran@gmail.com
GitHub: https://github.com/SriTarunika10
