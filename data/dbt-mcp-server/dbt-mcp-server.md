## Overview

The dbt MCP (Model Context Protocol) server is an open-source, experimental server that connects dbt projects to AI-powered tools and workflows. MCP lets AI systems like Claude Desktop and Cursor access your dbt project's metadata, documentation, and semantic layer for AI-driven analytics engineering.

## Three Functional Areas

### 1. Discovery & Metadata
Methods like get_all_models, get_model_details, get_model_parents enable:
- Autonomous metadata ingestion
- Automatic exploration of project structure
- Relationship discovery
- Column-level lineage

### 2. Semantic Layer Integration
Provides governed analytics using:
- list_metrics: Access validated business metrics
- get_dimensions: Retrieve metric dimensions
- query_metrics: Query metrics like monthly revenue directly from source of truth
- Governed data access through semantic definitions

### 3. Execution Engine
Drives operational orchestration:
- dbt run commands in isolated sandboxes
- Model execution and testing
- Workflow automation
- CI/CD integration

## Remote vs Local Server

### Remote dbt MCP Server (Public Beta)
- No installation required
- No dependencies to manage
- Hosted infrastructure
- Available for dbt Starter, Enterprise, and Enterprise+ plans

### Local dbt MCP Server
- Self-hosted option
- Open-source and experimental
- Full control over infrastructure

## Use Cases

- **Conversational Analytics**: Query business metrics through natural language
- **Data Catalog Exploration**: Discover models and their relationships conversationally
- **dbt Project Refactoring**: AI agents identify and refactor models to align with best practices
- **Documentation Generation**: Automated documentation from model metadata
- **Impact Analysis**: Understand downstream impacts of model changes
- **Lineage Exploration**: Trace data lineage through conversations

## AI-Driven Analytics Engineering

dbt expects both Business Intelligence and Data Engineering to be driven by AI operating on top of the context defined in dbt projects. The dbt MCP Server enables advanced AI-driven development workflows.

## Integration Benefits

- Natural language access to dbt metadata
- AI-assisted model development
- Automated refactoring workflows
- Conversational data exploration
- Governed semantic layer access
- Reduced time to insights

## Compatibility

Works with Claude Desktop, Cursor, and any MCP-compatible AI assistant.

## Pricing

Open-source local server. Remote server included with dbt Starter, Enterprise, and Enterprise+ plans.