## Overview

APIAgent is Agoda's open-source universal MCP proxy that automatically converts REST and GraphQL APIs into Model Context Protocol servers without writing any code or managing deployments. Launched in January 2026, it addresses the 'integration tax' problem for organizations with thousands of internal APIs.

## Features

- **Zero Code Conversion**: Automatically converts REST/GraphQL APIs to MCP servers
- **Zero Deployment**: No infrastructure setup or deployment required
- **Automatic Schema Introspection**: Discovers endpoints and fields from OpenAPI specs or GraphQL endpoints
- **DuckDB SQL Post-Processing**: Filters, sorts, and aggregates data locally using embedded SQL engine
- **Recipe System**: Captures repeated queries as parameterized recipes to reduce latency
- **Direct Return Options**: Filtered data can bypass LLM summarization for efficiency

## Technical Architecture

- **FastMCP**: Powers the MCP server layer
- **OpenAI Agents SDK**: Handles language model orchestration
- **DuckDB**: In-process SQL engine for data post-processing
- **Automatic Tool Mapping**: Exposes API endpoints as functional tools to LLMs

## Use Cases

- Enterprise API integration without manual MCP server development
- Legacy API modernization for AI workflows
- Rapid prototyping with existing APIs
- Reducing integration overhead in large organizations

## Pricing

Free and open-source.