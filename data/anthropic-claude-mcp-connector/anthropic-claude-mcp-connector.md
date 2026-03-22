## Overview

Anthropic's Messages API supports MCP servers as remote tool sources through the official MCP connector. This integration enables the Claude API to access external tools via MCP servers, with the mcp_servers API parameter for remote servers accessible via URL.

## Features

- **Messages API Integration**: Direct MCP server support in Claude API
- **Remote Tool Access**: Connect to remote MCP servers via URL
- **TypeScript SDK Helpers**: Automatic type conversion between MCP and Claude types
- **OAuth Support**: Authorization token parameter for secure authentication
- **Agent SDK**: Automatic MCP connection management
- **Multiple Transport Options**: Local processes, HTTP, or direct SDK execution

## API Requirements

- Header: "anthropic-beta: mcp-client-2025-11-20"
- Currently accesses tools from MCP servers via list_tools endpoint
- Resources and prompts not currently supported in API integration

## Integration Methods

### 1. **Claude Desktop App**
All Claude.ai plans support MCP server connections with one-click installation via desktop extensions.

### 2. **Claude API Direct**
Use mcp_servers parameter with Messages API for remote servers with tool support.

### 3. **Agent SDK Integration**
Automatic MCP connection management with support for:
- Local process execution
- HTTP connections
- Direct SDK application execution

## TypeScript SDK Helpers

Helper functions convert between:
- MCP types → Claude API types
- Eliminates manual conversion code
- Available in TypeScript SDK only

## Authentication & Security

- OAuth flow handled by API consumers
- Authorization token passed in MCP server definition
- Secure access token management
- Pre-API-call token acquisition

## Use Cases

- Extending Claude with custom tools
- Integrating external data sources
- Building AI agents with specialized capabilities
- Enterprise tool integration
- API-driven MCP server access
- Multi-tool orchestration

## Integration Benefits

- Official Anthropic support
- Seamless API integration
- Type-safe development (TypeScript)
- Flexible deployment options
- Secure authentication
- Enterprise-ready architecture

## Compatibility

Works with:
- Claude Desktop
- Claude API (Messages API)
- Agent SDK applications
- Any remote MCP server via HTTP

## Pricing

Claude API pricing applies based on usage. MCP integration included with all API tiers.