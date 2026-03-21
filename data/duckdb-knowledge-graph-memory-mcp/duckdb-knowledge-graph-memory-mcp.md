## Overview

DuckDB Knowledge Graph Memory MCP is an MCP server that implements knowledge graph-based persistent memory using DuckDB as the storage backend. This enables AI agents to store, query, and retrieve structured knowledge with graph relationships, providing enhanced context awareness and reasoning capabilities.

## Features

### Knowledge Graph Storage
- **Entity Management**: Store and manage entities with attributes
- **Relationship Modeling**: Define connections between entities
- **Graph Queries**: Navigate knowledge graphs efficiently
- **Semantic Search**: Find related information by meaning

### Memory Operations
- **Store Knowledge**: Save facts, entities, and relationships
- **Query Memory**: Retrieve relevant information on demand
- **Update Entities**: Modify existing knowledge
- **Delete Obsolete Data**: Remove outdated information

### DuckDB Backend
- **Fast Queries**: In-memory analytical performance
- **Persistent Storage**: Data survives between sessions
- **SQL Interface**: Powerful query capabilities
- **Efficient Storage**: Columnar compression

## Use Cases

### Conversational AI Memory
- Remember user preferences and context
- Track conversation history and topics
- Build user profiles over time
- Provide personalized responses

### Knowledge Base Building
- Extract and store information from documents
- Build domain-specific knowledge graphs
- Connect related concepts and entities
- Enable semantic search over knowledge

### RAG Enhancement
- Store structured facts alongside embeddings
- Combine vector search with graph traversal
- Improve retrieval accuracy
- Provide explainable answers

### Agent Memory Systems
- Long-term memory for AI agents
- Remember tasks and outcomes
- Learn from interactions
- Build contextual understanding

## Knowledge Graph Capabilities

### Entity Types
- People, organizations, locations
- Documents, concepts, topics
- Events and timestamps
- Custom domain entities

### Relationship Types
- Hierarchical (parent-child)
- Associative (related-to)
- Temporal (before-after)
- Causal (causes-effects)

### Query Patterns
- Find entities by attributes
- Navigate relationships
- Discover connected entities
- Pattern matching

## Integration

Works with AI assistants supporting MCP. Uses DuckDB for storage with automatic schema management. Compatible with vector databases for hybrid search approaches.

## Pricing

Free and open-source. DuckDB is also free and open-source.