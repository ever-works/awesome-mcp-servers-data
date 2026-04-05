## Overview

The Microsoft Learn Docs MCP Server is a cloud-hosted service that provides AI assistants with real-time access to official Microsoft documentation through the Model Context Protocol. It connects to `https://learn.microsoft.com/api/mcp` and enables semantic search across Microsoft Learn, Azure documentation, Microsoft 365 documentation, and other official Microsoft sources.

## Key Capabilities

- **Semantic Search**: Exposes the `microsoft_docs_search` tool that performs contextual semantic search against Microsoft's official technical documentation
- **Real-time Documentation**: Always accesses the latest Microsoft documentation as it is published, solving the problem of AI assistants being trained on outdated information
- **Context-Aware Results**: Understands context — searching for "containers" in an Azure context returns Azure Container Instances documentation, while the same term in a .NET context returns C# collection information
- **Comprehensive Coverage**: Covers Microsoft Learn, Azure docs, Microsoft 365 documentation, .NET/C# releases, ASP.NET Core, Entity Framework, and more
- **Structured Results**: Returns up to 10 high-quality content chunks with article titles and URLs

## Use Cases

- Query official Azure CLI command syntax
- Find Entity Framework dependency injection patterns in ASP.NET Core
- Look up the latest .NET Aspire features and implementation guidance
- Review code against Microsoft-validated performance recommendations
- Get authoritative JWT authentication implementation details

## Configuration

The server is cloud-hosted and requires no local deployment. It can be configured in VS Code settings.json and is accessible via the MCP protocol for any compatible AI assistant.

## Pricing

Free to use.