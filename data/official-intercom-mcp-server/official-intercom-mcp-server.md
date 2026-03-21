## Overview

Intercom provides an official MCP server as one of only three customer support platforms with first-party MCP integration. The server exposes 6 tools using a different design philosophy than competitors—two universal tools (search and fetch) that work across multiple resource types, plus four direct tools. Currently limited to US-hosted Intercom workspaces.

## Features

### Universal Tools
- **search**: Universal search across conversations, contacts, companies, and articles
- **fetch**: Retrieve specific resources by ID across all resource types

### Direct Tools
- **get_conversation**: Access detailed conversation data
- **get_contact**: Retrieve contact information
- **get_company**: Fetch company records
- **search_articles**: Find help center articles

### Resource Types
- Conversations and messages
- Contacts and user profiles
- Company records
- Help center articles
- Team assignments

### Limitations
- **Geography**: Currently US-hosted workspaces only
- **Tool Count**: 6 tools (fewer than Plain's 30)
- **Access**: Primarily read-focused operations

## Use Cases

### Customer Support
- Search conversation history
- Look up customer information quickly
- Find relevant help articles
- Access company context for support

### Data Retrieval
- Query customer interaction history
- Retrieve contact details
- Search help center content
- Access conversation threads

### AI-Assisted Support
- Provide context for support agents
- Suggest relevant help articles
- Auto-populate customer information
- Surface previous interactions

## Platform Comparison

As of March 2026, Intercom is one of three platforms with official MCP servers:
- **Plain**: 30 tools, global availability, read/write access
- **Intercom**: 6 tools, US workspaces only, primarily read access
- **Pylon**: 6 tools, global availability, read/write access

## Integration

Works with MCP-compatible AI assistants like Claude and Cursor. Requires Intercom workspace (US-hosted) and API authentication. OAuth support for secure access.

## Pricing

Intercom offers tiered pricing based on features and seat count. MCP server access available on qualifying plans.