# BioMistral Medical RAG Chatbot

## Introduction
This repository contains code for building a Medical Chatbot using the BioMistral Large Language Model (LLM) and Heart Health PDF files. The chatbot is designed to provide accurate and relevant responses to medical queries based on the information extracted from the provided PDF documents.

## Installation Requirements
- Python 3.x
- Libraries: langchain_community, IPython

## Setup Environment
1. Install the required libraries and modules
2. Import necessary modules and libraries in your Python environment.
3. Update the paths and configurations in the code as per your requirements.

## Usage
1. Import the necessary document or PDF files using the provided document loaders.
2. Split the text into smaller passages for efficient processing.
3. Initialize embeddings for text
4. Initialize a vector store for retrieval purposes (FAISS or ChromaDB).
5. Initialize the BioMistral LLM model for generating responses.
6. Define a ChatPromptTemplate for interacting with the chatbot.
7. Run the code and input prompts to interact with the chatbot.

# Notes
Ensure that you have the necessary permissions to access and use the provided PDF documents. Adjust the configurations and parameters according to your specific use case and requirements. Monitor system resource usage, especially memory and GPU utilization, while running the code.

## Example
```python
# Import necessary libraries and modules
from langchain_community.document_loaders import PyPDFDirectoryLoader
from langchain.text_splitter import CharacterTextSplitter, RecursiveCharacterTextSplitter
from langchain_community.embeddings import HuggingFaceEmbeddings
from langchain.vectorstores import FAISS, Chroma
from langchain_community.llms import LlamaCpp
from langchain.chains import LLMChain
import pathlib
import textwrap
from IPython.display import display, Markdown

# Function to convert text to Markdown format
def to_markdown(text):
 text = text.replace('•', '  *')
 return Markdown(textwrap.indent(text, '> ', predicate=lambda _: True))

# Define ChatPromptTemplate
template = """
You are an AI assistant that follows instruction extremely well.
Please be truthful and give direct answers
</s>
{query}
</s>
"""

import sys

# User input loop
while True:
 user_input = input(f"Input Prompt: ")
 if user_input == 'exit':
     print('Exiting')
     sys.exit()
 if user_input == '':
     continue
 result = rag_chain.invoke(user_input)
 print("Answer: ", result)
