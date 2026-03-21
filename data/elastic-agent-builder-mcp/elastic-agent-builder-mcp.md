## Overview

The Elastic Agent Builder MCP server is the recommended approach for Elasticsearch 9.2+ deployments and Serverless projects. It offers full access to built-in and custom tools, enabling AI agents to connect to Elasticsearch data through natural language conversations with advanced retrieval and analysis capabilities.

## Features

### Agent Builder Capabilities
- **Built-in Tools**: Pre-configured tools for common operations
- **Custom Tools**: Create specialized tools for your use cases
- **Full Tool Access**: Complete access to Elasticsearch functionality
- **Natural Language**: Conversational interface to your data

### Search Operations
- **Lexical Search**: Traditional keyword-based search
- **Semantic Search**: Vector-based similarity search
- **Hybrid Search**: Combine lexical and semantic for best results
- **Complex Queries**: Multi-field, nested, and aggregated searches

### Data Analysis
- **Aggregations**: Analyze data patterns and trends
- **Time Series**: Work with time-based data
- **Geospatial**: Location-based queries and analysis
- **Machine Learning**: Access Elasticsearch ML features

### Advanced RAG
- **Hybrid Retrieval**: Lexical + semantic search
- **Reranking**: Improve result relevance
- **Context Enhancement**: Enrich results with metadata
- **Citation Tracking**: Link answers to source documents

## Elasticsearch Platform

### Search Engine
- Distributed search and analytics
- Real-time indexing and search
- Full-text search capabilities
- RESTful API

### Data Platform
- JSON document storage
- Schema-free flexibility
- Automatic field mapping
- Nested and complex data types

### Analytics
- Aggregation framework
- Time-series analytics
- Geospatial analytics
- Machine learning integrations

## Use Cases

### Enterprise Search
- Search across documents and databases
- Semantic understanding of queries
- Personalized search results
- Real-time index updates

### Log Analytics
- Centralized log aggregation
- Real-time log search
- Pattern detection and alerts
- Performance monitoring

### RAG Applications
- Build knowledge bases for AI
- Retrieve relevant context for LLMs
- Combine structured and unstructured data
- Explainable AI with source citations

### Business Intelligence
- Real-time dashboards
- Data exploration and discovery
- Trend analysis and forecasting
- Custom analytics workflows

## Version Compatibility

### Elasticsearch 9.2+
- Agent Builder MCP (recommended)
- Full feature set
- Best performance and support

### Earlier Versions
- elastic/mcp-server-elasticsearch
- Limited tool set
- Basic functionality

## Integration

Works with AI assistants supporting MCP. Requires Elasticsearch 9.2+ or Elasticsearch Serverless. Configure with Elasticsearch credentials and endpoint URL.

## Pricing

Elasticsearch offers various deployment options:
- **Elastic Cloud**: Managed service with usage-based pricing
- **Self-Managed**: Free basic license, paid for advanced features
- **Serverless**: Pay per search and storage

MCP server included with all Elasticsearch deployments.