
# Weather RAG Chatbot

**Project Introduction**

Weather RAG Chatbot is an AI-powered Retrieval-Augmented Generation (RAG) project designed to answer weather-related queries using historical and forecast data. Instead of relying solely on a large language model’s memory, this project leverages a FAISS vector store to store and retrieve relevant weather records. By combining semantic search with natural language generation, the chatbot can provide accurate, context-aware responses to user questions such as temperature, humidity, and weather conditions for specific cities and dates.

**The project demonstrates how to:**

Convert raw weather data into embeddings for fast retrieval.

Store embeddings in a FAISS vectorstore for scalable similarity search.

Integrate retrieved documents with an LLM (OpenAI GPT-3.5) for natural language answers.

Handle queries about multiple cities and time periods efficiently.

**This project is ideal for:**

Learning RAG pipelines with Python and LangChain.

Building domain-specific AI assistants that use real-world datasets.

Exploring vector search and LLM integration in practical applications.


## Installation

**Clone the repository**

git clone https://github.com/yourusername/weather-rag-chatbot.git
cd weather-rag-chatbot

**Create and activate the virtual environment**

conda create -n rag_env python=3.10 -y

conda activate rag_env

**Install dependancies**

pip install -U langchain langchain-community sentence-transformers faiss-cpu openai


**Set up an openai API Key**




    
## Usage
Data preparation and converstion to text document.

Create embeddings and vectore store.

Querrying the vectorstore, eg.

* What is the highest temperature in Kisumu on 2026-01-19?

* What is the average humidity in Mombasa during March?

* Which city had the highest average temperature among Nairobi, Mombasa, and Kitale?

## Future Improvements

* Expand vectorstore with more cities and longer historical records.

* Integrate web interface for interactive querying.

* Use local LLMs to avoid API quota limitations.
