## Overview

Model Context Protocol (MCP) is becoming the industry standard for extending AI models with additional tools and knowledge. OpenAI provides official support for building MCP servers to use with ChatGPT Apps, deep research, or API integrations.

## Features

- **ChatGPT Apps Integration**: Build MCP servers for ChatGPT applications
- **Deep Research**: Connect to knowledge bases and data sources
- **API Integration**: Use MCP servers with OpenAI API
- **Remote Server Support**: Connect models to Internet-accessible servers
- **OAuth Authorization**: Secure authentication with access tokens
- **UI Bundle Rendering**: Custom widgets inside ChatGPT iframe
- **Developer Mode**: Full MCP client support for read and write tools

## ChatGPT Developer Mode

Beta feature providing:
- Full Model Context Protocol (MCP) client support
- Access to all tools (read and write)
- Enhanced debugging capabilities
- Advanced tool integration

## Key Capabilities

### MCP Server Requirements
- Define tools with auth enforcement
- Return data to ChatGPT
- Point tools to UI bundles
- Widget rendering in iframe
- Communication via MCP Apps UI bridge

### Compatibility Schema
For ChatGPT deep research and company knowledge:
- Implement two read-only tools: search and fetch
- Use standardized compatibility schema
- Support vector stores and private data sources

## API Integration

Remote MCP servers work with OpenAI API:
- Any server on public Internet implementing MCP
- Use mcp built-in tool type
- Require server_url parameter
- Optional OAuth authorization parameter

## Use Cases

- Extending ChatGPT with custom tools
- Enterprise knowledge base integration
- Vector store connections
- Private data source access
- Custom research capabilities
- Specialized domain tools
- Company-specific integrations

## Integration Benefits

- Industry-standard protocol
- Flexible tool definition
- Secure OAuth authentication
- Custom UI rendering
- API and App integration
- Deep research capabilities

## Development Tools

- OpenAI Apps SDK
- MCP server templates
- UI bundle framework
- Authentication helpers
- Testing tools

## Compatibility

Works with:
- ChatGPT Apps
- ChatGPT deep research
- OpenAI API
- Remote MCP servers
- Docker-based deployments

## Pricing

OpenAI API pricing applies based on usage. MCP integration available across API tiers.