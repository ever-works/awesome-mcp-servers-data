## Overview

The official MCP Server for Neo4j is a local MCP server downloadable as a binary and works with all types of Neo4j Deployments including Neo4j Aura, Self Managed, Docker, Neo4j Desktop, and Neo4j Sandbox. The Neo4j MCP ecosystem includes several specialized servers for different use cases.

## Specialized Servers

### 1. **Cypher Server (mcp-neo4j-cypher)**
Allows extracting the graph database schema to give the agent-LLM the ability to generate Cypher queries to query and update the database.

### 2. **Knowledge Graph Memory Server**
Stores and retrieves entities and relationships from your personal knowledge graph in a local or remote Neo4j instance, allowing access to that information over different sessions, conversations, and clients.

### 3. **Aura Management Server**
Manages Neo4j Aura instances directly from your AI assistant chat:
- Create and destroy instances
- Find instances by name
- Scale instances up and down
- Enable features

### 4. **Data Modeling Server**
Creates, validates, and visualizes Neo4j graph data models:
- Model creation and validation
- Visual modeling capabilities
- Model import/export from Arrows.app

## Key Features

- **Schema Extraction**: Automatic graph schema discovery
- **Cypher Generation**: AI-generated queries from natural language
- **Knowledge Graph Memory**: Persistent agent memory
- **Instance Management**: Cloud instance lifecycle management
- **Visual Modeling**: Interactive data model design
- **No-Code Approach**: Build knowledge graphs without coding

## Use Cases

- AI agent memory management
- Knowledge graph construction
- Graph database querying
- Data modeling and visualization
- Cloud instance management
- Entity and relationship tracking
- Cross-session information persistence

## No-Code Knowledge Graph Building

The combination of Claude, MCP, and Neo4j represents a significant step toward democratizing graph database technology by removing the coding barrier, opening up powerful knowledge graph capabilities to a wider audience.

## Integration Support

Agent Frameworks supporting MCP:
- LangChain
- CrewAI
- Pydantic.AI
- Agent Development Kit (ADK)

MCP Clients:
- Claude Desktop
- VS Code
- Cursor
- Windsurf
- Gemini CLI

## Deployment Options

- Neo4j Aura (cloud)
- Self-managed instances
- Docker containers
- Neo4j Desktop
- Neo4j Sandbox

## Integration Benefits

- Natural language graph queries
- Persistent AI agent memory
- Visual data modeling
- Simplified graph database access
- No Cypher knowledge required
- Cross-framework compatibility

## Compatibility

Works with all MCP-compatible AI assistants and agent frameworks. Supports all Neo4j deployment types.

## Pricing

Neo4j offers free tier (Neo4j Aura Free). Professional and Enterprise plans for production use.