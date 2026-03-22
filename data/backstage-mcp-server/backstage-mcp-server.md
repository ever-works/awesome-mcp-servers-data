## Overview

Backstage's integration with the Model Context Protocol (MCP) represents a significant advancement in platform engineering, enabling AI agents to interact with developer platform functionality in a standardized, secure way. This integration allows developers to query and manage their software catalog through natural language conversations.

## Features

- **Actions Registry Integration**: New mcp-actions backend plugin surfaces plugin actions as tools in an MCP server
- **Catalog Access**: Query catalog entity data including ownership, relationships, and metadata
- **Template Management**: List and instantiate scaffolder templates
- **Tech Insights**: Access Tech Insights metrics and scorecards
- **API Documentation**: Query and interact with API documentation
- **Natural Language Queries**: Ask questions like "Do we have a microservice template in C#?" or "Who owns Order Management System?"

## Platform Engineering Benefits

- Standardized way to expose business logic across multiple interfaces
- Security and type safety maintained
- Reduced context switching for developers
- Access Backstage functionality without opening the UI
- Integration with popular AI tools

## Available Implementations

- Official Backstage mcp-actions plugin (v1.40+)
- Roadie MCP servers for enhanced catalog and template access
- Red Hat Developer Hub MCP integration

## Use Cases

- Query software catalog for service information
- Discover and instantiate project templates
- Find service owners and dependencies
- Access API documentation conversationally
- Retrieve Tech Insights metrics

## Supported AI Clients

Cursor, Claude, ChatGPT, Windsurf, and any MCP-compatible AI assistant.

## Status

Currently experimental but represents a significant shift in platform engineering workflows.

## Pricing

Open-source for Backstage. Roadie offers managed Backstage with MCP integration (contact for pricing).