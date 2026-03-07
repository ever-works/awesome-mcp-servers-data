## Overview

Pinecone has released three MCP servers: Pinecone Assistant MCP (remote), Pinecone Assistant MCP (local), and Pinecone Developer MCP (local). These servers enable integration between Pinecone's vector database capabilities and Model Context Protocol-compatible applications.

## Available MCP Servers

**1. Pinecone Assistant MCP (Remote)**
- Cloud-hosted server
- No local setup required
- Managed infrastructure
- Scalable operations

**2. Pinecone Assistant MCP (Local)**
- Self-hosted deployment
- Full control over configuration
- Custom optimization
- Development environment support

**3. Pinecone Developer MCP (Local)**
- Developer-focused tooling
- In-IDE documentation search
- Development workflow integration
- Testing and debugging capabilities

## Key Features

- **Structured Context for Agents**: Provide organized context to AI agents
- **In-IDE Documentation Search**: Search documentation directly within development environments
- **Vector Database Operations**: Perform CRUD operations on vector embeddings
- **Semantic Search**: Find similar vectors based on meaning
- **RAG Support**: Enable Retrieval-Augmented Generation workflows
- **Integrated Embeddings**: Built-in embedding generation for supported models
- **Namespace Management**: Organize vectors in logical namespaces
- **Metadata Filtering**: Filter searches based on metadata fields

## Embeddings Integration

The Pinecone MCP supports only indexes with integrated embedding, meaning:

- Indexes must use Pinecone's embedding models
- External embedding models are not supported for MCP integration
- Generate embeddings by specifying a supported model
- Provide input data and model-specific parameters
- Upsert vectors with integrated embeddings

## Supported Models

Pinecone offers various embedding models:

- text-embedding-ada-002 (OpenAI)
- text-embedding-3-small (OpenAI)
- text-embedding-3-large (OpenAI)
- Other supported embedding models

## Core Capabilities

**Vector Operations:**
- Upsert vectors (insert/update)
- Query vectors (similarity search)
- Fetch vectors by ID
- Delete vectors
- Update vector metadata

**Index Management:**
- List indexes
- Create indexes
- Delete indexes
- Describe index configuration

**Search & Retrieval:**
- K-nearest neighbor search
- Metadata filtering
- Namespace filtering
- Hybrid search (vector + metadata)
- Top-K results retrieval

**RAG Workflows:**
- Document chunking
- Embedding generation
- Vector storage
- Semantic retrieval
- Context assembly for LLMs

## Use Cases

**Semantic Search Applications:**
- Document search across knowledge bases
- Code search in repositories
- Product recommendation systems
- Similar content discovery

**RAG Implementations:**
- Question answering systems
- Chatbots with knowledge retrieval
- Documentation assistants
- Customer support automation

**Development Tooling:**
- In-IDE documentation lookup
- Code example search
- API reference navigation
- Framework documentation access

**Enterprise Applications:**
- Knowledge management systems
- Internal search engines
- Content recommendation
- Duplicate detection

## Installation

Via NPX:
```bash
npx @pinecone-database/mcp
```

Configuration requires:

- Pinecone API Key (PINECONE_API_KEY environment variable)
- Index name
- Embedding model selection

## Configuration Example

```json
{
  "mcpServers": {
    "pinecone": {
      "command": "npx",
      "args": ["-y", "@pinecone-database/mcp"],
      "env": {
        "PINECONE_API_KEY": "your-api-key-here"
      }
    }
  }
}
```

## Community Implementations

Several community-built servers extend Pinecone MCP functionality:

- **zx8086/pinecone-vector-db-mcp-server**: Additional vector operations
- **sirmews/pinecone**: Alternative implementation with custom features
- RAG-focused implementations for PDF and Confluence data

## Vector Index Requirements

**For MCP Compatibility:**
- Must use integrated embeddings
- Cannot use externally-generated vectors
- Embedding model must be specified at index creation
- Dimension must match embedding model output

## Metadata Support

Vectors can include metadata:

```json
{
  "id": "doc-123",
  "values": [0.1, 0.2, ...],
  "metadata": {
    "title": "Document Title",
    "category": "technology",
    "date": "2026-03-07"
  }
}
```

Filter searches using metadata:

```json
{
  "filter": {
    "category": {"$eq": "technology"},
    "date": {"$gte": "2026-01-01"}
  }
}
```

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Custom MCP implementations

## Performance Characteristics

- **Query Latency**: Sub-100ms for most queries
- **Throughput**: Thousands of queries per second
- **Scalability**: Billions of vectors supported
- **Availability**: 99.9% uptime SLA
- **Regions**: Multiple cloud regions available

## Namespaces

Organize vectors using namespaces:

- Logical separation of vector sets
- Independent scaling
- Isolated search scopes
- Multi-tenant support
- Access control per namespace

## Semantic Search Quality

- State-of-the-art embedding models
- Optimized retrieval algorithms
- Relevance ranking
- Result reranking options
- Query expansion support

## Integration Patterns

**RAG Pattern:**
1. User submits query
2. Generate query embedding
3. Search Pinecone for similar vectors
4. Retrieve source documents
5. Assemble context for LLM
6. Generate response with context

**Documentation Search:**
1. Developer types search query
2. MCP server generates embedding
3. Pinecone returns relevant docs
4. Results displayed in IDE

## Pricing

Pinecone pricing based on:

- Index size (number of vectors)
- Query volume
- Storage tier (standard, fast)
- Cloud region
- Free tier available for development