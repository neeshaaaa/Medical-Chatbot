# Medical-Chatbot
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
