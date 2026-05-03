# Medical-Chatbot

🩺 Medical AI Chatbot (RAG-Based System)

An AI-powered medical chatbot that uses Retrieval-Augmented Generation (RAG) to answer questions based on a curated medical knowledge base.

🚀 Features
PDF-based medical knowledge ingestion
Text preprocessing and chunking
Semantic embeddings using HuggingFace
Vector storage using Pinecone
Context-aware response generation using Llama 3 (Ollama)
Flask-based web interface
Fast similarity search for relevant medical context
🧠 How It Works
Medical PDF documents are loaded using LangChain loaders
Text is cleaned and split into chunks
Each chunk is converted into embeddings
Embeddings are stored in Pinecone vector database
User asks a question
Query is embedded and matched with relevant chunks
Retrieved context is passed to LLM
LLM generates final response


# steps

git clone https://github.com/neeshaaaa/Medical-Chatbot.git


Step-1 
python -m venv medibot

medibot\Scripts\activate


step-2
pip install -r requirements.txt


# Create a .env file in the root directory and add your Pinecone & openai credentials as follows:

PINECONE_API_KEY = ".................................."


# run the following command to store embeddings to pinecone
python store_index.py


# Finally run the following command
python app.py


Now,  open up localhost: localhost:8080



# Techstack Used:
Python
LangChain
Flask
llama 3
Pinecone
