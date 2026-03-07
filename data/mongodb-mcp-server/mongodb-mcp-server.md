## Overview

The MongoDB MCP Server enables AI-powered development by connecting MongoDB deployments—whether on MongoDB Atlas, MongoDB Community Edition, or MongoDB Enterprise Advanced—to MCP-supported clients like Windsurf, Cursor, GitHub Copilot in Visual Studio Code, and Anthropic's Claude.

## Key Features (Winter 2026 Update)

- **Performance Advisor Integration**: Directly integrates with Performance Advisor tools in MongoDB Atlas, providing performance insights in your development environment
- **Automatic Embedding Generation**: The insert-many tool now supports automatic embedding generation for fields with vector search indexes using Voyage AI models
- **Local Cluster Management**: Create and manage local MongoDB clusters directly from the MCP server
- **Vector Search Index Support**: CreateIndexTool class now supports both vector search indexes and regular MongoDB indexes
- **Database Operations**: Full CRUD operations via natural language
- **Data Exploration**: Query and analyze data using conversational commands
- **Schema Design**: Design tables and generate migrations
- **Context-Aware Code Generation**: Generate MongoDB queries and application code with AI assistance

## Supported MongoDB Deployments

- MongoDB Atlas (cloud-hosted)
- MongoDB Community Edition
- MongoDB Enterprise Advanced
- Local MongoDB instances

## Compatible AI Tools

- Windsurf
- Cursor
- GitHub Copilot in Visual Studio Code
- Anthropic's Claude (Claude Desktop and Claude Code)
- Other MCP-compatible AI assistants

## Use Cases

- Natural language database queries
- Schema design and optimization
- Performance troubleshooting with AI assistance
- Automated data migration generation
- Vector search implementation for AI applications
- Database administration tasks
- Query optimization and analysis

## Technical Capabilities

- Supports aggregation pipelines
- Vector embeddings for semantic search
- Full-text search integration
- Index management (including vector search indexes)
- Performance monitoring and optimization
- Connection to multiple databases simultaneously

## Installation

Available via npm and pip, with detailed setup instructions in the official MongoDB documentation.

## Pricing

Free and open-source. MongoDB Atlas pricing applies for cloud deployments.