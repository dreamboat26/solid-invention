# Using RAG with LLaMa 13B

In this notebook, we explore how to utilize the open-source Llama-13b-chat model in both Hugging Face Transformers and LangChain. Please note that access to Llama 2 models must be requested via the provided form and is typically granted within a few hours.

🚨 Note: Running this notebook on CPU may be slow. To speed up processing, you can select a GPU accelerator in Google Colab by going to Runtime > Change runtime type > Hardware accelerator > GPU > GPU type > T4.

## Installation and Setup

We start by installing the required libraries via pip. Ensure all necessary dependencies are installed.

## Initializing the Hugging Face Embedding Pipeline

We initialize the embedding pipeline to transform our documents into vector embeddings. For this purpose, we use the sentence-transformers/all-MiniLM-L6-v2 model.

## Building the Vector Index

Next, we utilize the embedding pipeline to build embeddings and store them in a Pinecone vector index. To begin, initialize the index using a free Pinecone API key.

## Initializing the Hugging Face Pipeline

To initialize the text-generation pipeline with Hugging Face Transformers, we require:
- A LLM (e.g., meta-llama/Llama-2-13b-chat-hf).
- The respective tokenizer for the model.

We download and initialize the model, which may take a few minutes.

## Initializing a RetrievalQA Chain

For Retrieval Augmented Generation (RAG) in LangChain, we initialize either a RetrievalQA or RetrievalQAWithSourcesChain object. Both require an LLM and a Pinecone index initialized within a LangChain vector store object.
