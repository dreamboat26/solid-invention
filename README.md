# Mistral-7B LLM Indexing and Querying Demo

## Introduction
Welcome to the Mistral-7B LLM Indexing and Querying Demo! This repository demonstrates how to set up indexing and querying using the Mistral-7B Large Language Model (LLM) for semantic search. The demo includes instructions on installing dependencies, configuring the model and embeddings, indexing documents, and querying the index for relevant information.
## Set Up Model and Embeddings

1. **Import Libraries and Configure Logging**: 
   Import the required libraries and configure logging for better visibility.

2. **Initialize Mistral-7B LLM**:
   Initialize the Mistral-7B Large Language Model (LLM) using LLamaCPP with specific configurations such as temperature, max new tokens, and context window.

3. **Set Up Embedding Model**:
   Set up an embedding model using HuggingFaceEmbeddings for semantic representations.

## Indexing Documents

1. **Create Langchain Embedding and ServiceContext Objects**:
   Create Langchain embedding and ServiceContext objects.

2. **Create VectorStoreIndex**:
   Utilize these objects to create a VectorStoreIndex from documents.

## Querying the Index

1. **Create Query Engine**:
   Create a query engine from the index.

2. **Query Index**:
   Query the index with specific questions or queries to retrieve relevant information.

## Usage

You can modify the code example provided in the README and integrate it into your own projects for semantic search applications. Ensure that you have the necessary permissions to access the Mistral-7B model and embeddings.

## Acknowledgments

This demo utilizes the Mistral-7B Large Language Model provided by TheBloke on the Hugging Face model hub. We acknowledge the contributions of the LLamaCPP and LangchainEmbedding libraries in enabling semantic search functionality.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

   

