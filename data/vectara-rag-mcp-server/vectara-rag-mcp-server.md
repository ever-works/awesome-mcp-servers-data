## Overview

Vectara-MCP provides agentic applications with access to fast, reliable RAG (Retrieval-Augmented Generation) through the Model Context Protocol, leveraging Vectara's Trusted RAG platform to reduce hallucinations and improve factual accuracy.

## Features

- **RAG queries**: Run RAG queries using Vectara, returning search results with generated responses
- **Semantic search**: Execute semantic search queries without generation for pure retrieval
- **Hallucination correction**: Identify and correct hallucinations using Vectara's VHC API
- **Fast retrieval**: Optimized for sub-second query response times
- **Grounded generation**: All generated responses grounded in retrieved documents
- **Enterprise-grade security**: Secure connections with API key authentication
- **Multi-corpus support**: Query across multiple document collections

## Available Tools

1. **ask_vectara**: Run a RAG query using Vectara, returning search results with a generated response that synthesizes the information

2. **search_vectara**: Run a semantic search query using Vectara without generation, returning only the most relevant documents

3. **correct_hallucinations**: Identify and correct hallucinations in generated text using Vectara's VHC (Vectara Hallucination Correction) API

## Use Cases

- Enterprise document search and question answering
- Customer support knowledge base integration
- Legal document analysis and retrieval
- Research paper search and summarization
- Technical documentation Q&A
- Compliance and regulatory document search

## Installation

Available via pip:
```bash
pip install vectara-mcp
```

## Configuration

Requires Vectara API key and corpus keys. Compatible with Claude Desktop and other MCP clients through standard configuration.

## Technical Details

- Built with Python MCP SDK
- Supports streaming responses
- Configurable relevance thresholds
- Citation and source tracking for all results

## Pricing

Vectara platform pricing applies. Free tier available for development and testing.