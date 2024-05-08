# Fantasy Football Assistant

## Overview

This repository contains a Fantasy Football Assistant built using various natural language processing (NLP) techniques and models. The assistant provides insights, recommendations, and answers to questions related to fantasy football based on available articles and user queries. This README provides an overview of the components and functionalities of the Fantasy Football Assistant.

## Components and Functionality

The Fantasy Football Assistant comprises several components and functionalities:

1. **Model Loading and Configuration**:
   - Load pre-trained language models for text generation and processing.
   - Configure model quantization for optimized performance.

2. **Model Parameter Information**:
   - Print the number of trainable model parameters to provide insights into the model's complexity and resource requirements.

3. **Text Generation Pipeline**:
   - Create a text generation pipeline using the loaded language model for generating text based on prompts.

4. **Document Scraping and Processing**:
   - Scrape fantasy football articles from specified URLs.
   - Convert HTML documents to plain text for further processing.

5. **Text Chunking and Indexing**:
   - Chunk text into smaller segments for efficient indexing.
   - Index the chunked text segments using FAISS for fast retrieval.

6. **Question Answering**:
   - Generate prompts for answering questions based on fantasy football context and user queries.
   - Utilize the language model to provide answers to user questions.

## Usage

The Fantasy Football Assistant can be used to:
- Retrieve insights and recommendations from fantasy football articles.
- Answer specific questions related to fantasy football based on available articles and user input.

## Example

Here's an example use case of the Fantasy Football Assistant:

1. **User Query**: "Should I start Gibbs next week for fantasy?"
2. **Assistant Response**: The assistant provides an informed answer based on available context and knowledge about fantasy football.

## Dependencies

Ensure you have the following dependencies installed to run the Fantasy Football Assistant:
- Python 3.x
- PyTorch
- Hugging Face Transformers
- FAISS
- LangChain (Custom Library)

## Future Improvements

Possible future improvements for the Fantasy Football Assistant include:
- Enhancing the question-answering capabilities with more sophisticated models.
- Incorporating real-time data and player statistics for more accurate recommendations.
- Improving user interaction and interface for a smoother experience.



