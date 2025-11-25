🚀 LangGraph RAG & Tool-Augmented RAG Pipelines

This repository contains three Jupyter notebooks demonstrating how to build advanced Retrieval-Augmented Generation (RAG) systems using LangChain, LangGraph, FAISS, Ollama, and Tavily Web Search.

📘 Included Notebooks
1. Basic RAG Pipeline (LangChain)

Loads PDFs

Splits text into chunks

Generates embeddings

Stores vectors in FAISS

Uses a local LLM (Ollama) to answer queries using retrieved context

2. LangGraph RAG Pipeline

Converts the traditional RAG flow into a node-based graph

Adds visibility, orchestration, and traceability

Includes graph visualization (Mermaid + PNG)

3. Tool-Augmented LangGraph RAG

Adds tools to the RAG pipeline:

Internal document retrieval (FAISS)

External web search (Tavily)

Includes an intelligent router that decides whether to use:

Internal knowledge

Web search

Or both (hybrid)

Generates a complete graph diagram showing the flow

🧩 Key Features

Local PDF-based RAG

FAISS vector search

Sentence Transformer embeddings

Local LLM inference via Ollama

Tool calling inside LangGraph

Automatic decision-making through router LLM

Mermaid and PNG graph exports for visualization

📂 Project Structure

Notebook 1: Basic RAG

Notebook 2: LangGraph RAG

Notebook 3: Tool-Augmented LangGraph RAG

Graph exports (.png and .mmd)

all_doc/ folder for PDFs

📄 How It Works

PDFs are loaded and converted into text.

Text is chunked and embedded.

FAISS is used for semantic retrieval.

LangGraph builds a stateful pipeline.

Tools (internal retrieval + web search) are added.

Router decides which tool(s) to call.

Final answer is generated using the LLM with combined context.

📊 Outputs Generated

Workflow graph for LangGraph RAG

Workflow graph for Tool-Augmented RAG

Intermediate retrieval results

Final synthesized answers

🎯 Purpose of the Project

This project is designed to help you:

Understand RAG basics

Learn how LangGraph organizes pipelines

Add tool routing & external APIs

Build production-ready retrieval systems

Work with local LLMs on your machine

📝 Notes

Place all PDFs inside the all_doc/ folder.

Tavily API key must be added in .env if using web search.

Ollama must have the required model installed.
