# Neurotech Chatbot with Retrieval-Augmented Generation (RAG)

This project implements a Neurotech-focused chatbot using Retrieval-Augmented Generation (RAG). It leverages FAISS for vector search, OpenAI embeddings for document representation, and the OpenAI API for generating responses. The chatbot is designed to retrieve and process information from a curated set of Brain-Computer Interface (BCI) articles.

## Features

- **Document Parsing**: Uses `fitz` (PyMuPDF) to extract text from neurotech-related PDFs.
- **Vector Search**: Implements FAISS for efficient similarity search.
- **Embeddings**: Uses OpenAI's text embedding model to encode document segments.
- **Chatbot Integration**: Accepts user queries, retrieves relevant information, and generates responses using OpenAI's GPT model.

## Installation

Ensure you have Python 3.8+ installed. Then, install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

1. **Prepare Data**: Place your BCI-related PDFs in the `articles/raw/` folder.
2. **Index Documents**: Run the notebook to extract text, create embeddings, and build the FAISS index.
3. **Query the Chatbot**: Using OpenAI's API, you can query the model with context retreived from the vector search

## Future Improvements

- Modularize the code into .py scripts instead of a notebook
- Implement a web-based UI for interaction.
- Enhance document processing with improved chunking strategies.
- Expand dataset support.
- Purchase more credits from OpenAI to move up in the usage tiers (lol)
