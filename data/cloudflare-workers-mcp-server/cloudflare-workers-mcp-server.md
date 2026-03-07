## Overview

Cloudflare has built robust integration between the Model Context Protocol and Cloudflare Workers, allowing developers to build and deploy MCP servers on their edge computing platform. The official Cloudflare API MCP server provides access to the entire Cloudflare API—over 2,500 endpoints—through an innovative approach.

## Key Features

- **2,500+ API Endpoints**: Complete access to Cloudflare's API across all products
- **Codemode Technique**: Model writes JavaScript against a typed OpenAPI spec rather than loading individual tool definitions
- **Dynamic Worker Sandboxes**: Generated code runs in isolated sandboxes for security
- **Two Core Tools**: search() and execute() handle all 2,500+ endpoints efficiently
- **Workers Bindings**: Access D1 databases, R2 object storage, and KV stores on-the-fly
- **OAuth Integration**: Built-in OAuth Provider Library for MCP server authorization
- **Edge Deployment**: Deploy MCP servers to Cloudflare's global edge network
- **Streamable HTTP Transport**: Supports current MCP specification standard

## Cloudflare MCP Ecosystem

**1. Cloudflare API MCP Server**
Provides access to DNS management, Workers deployment, R2 storage, Zero Trust security, CDN configuration, and all other Cloudflare products through two intelligent tools.

**2. Workers MCP Package**
CLI tooling and in-Worker logic to connect Claude Desktop (or any MCP Client) to a Cloudflare Worker on your account using the `workers-mcp` package.

**3. MCP Gateway**
Cloudflare's open-source solution for orchestrating Model Context Protocol servers, managing configuration, credentials, and access control.

**4. Workers Bindings MCP Server**
Leverage application development primitives like D1 databases, R2 object storage, and Key Value stores as you build Workers applications.

## How Codemode Works

Instead of defining 2,500+ individual tools, the MCP server uses Codemode where:

1. The AI searches for relevant endpoints using search()
2. The AI writes JavaScript code against the typed Cloudflare API client
3. Code executes in an isolated Dynamic Worker sandbox
4. Results return to the AI assistant

This approach is more scalable and maintainable than traditional tool-per-endpoint models.

## Deployment with Wrangler

Use the Wrangler CLI to:

- Create new MCP servers locally
- Test MCP servers in development
- Deploy to Cloudflare's edge network
- Manage server configurations and secrets

## Security Features

- Isolated execution in Dynamic Worker sandboxes
- OAuth 2.1 protocol support via OAuth Provider Library
- API key authentication
- Fine-grained access controls
- Audit logging

## Use Cases

- Managing Cloudflare DNS records
- Deploying and configuring Workers
- Managing R2 object storage
- Configuring Zero Trust security policies
- CDN cache management
- Analytics and reporting
- Automated incident response

## Integration

Compatible with Claude Desktop, Cursor, and other MCP clients through one-click setup.

## Pricing

Cloudflare Workers pricing applies. Free tier includes 100,000 requests per day.