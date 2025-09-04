# AI RAG Assistant 

A Gradio-based Question-Answering (QA) application that leverages **IBM Watsonx AI** LLMs and embeddings to answer questions from PDF documents.

## Features

- Upload a PDF document.
- Ask questions about the content.
- Uses IBM Watsonx **Mixtral-8x7b** model for text generation.
- Embeddings-based retrieval with **Slate-125m** model.
- Implements **RAG (Retrieval-Augmented Generation)** with LangChain.
- Chunks large documents for better semantic search.
- Simple web interface with Gradio.

## Installation

Install the required packages:

```bash
pip install ibm-watsonx-ai langchain langchain-community gradio chromadb PyPDF2

