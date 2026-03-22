## Overview

The Vault MCP Server is HashiCorp's official Model Context Protocol server implementation that provides integration with Vault for managing secrets and mounts. This server enables AI models to securely interact with Vault through natural language commands.

## Features

- **Mount Management**: List, create, and delete mounts in Vault (KV v1, KV v2)
- **Secret Operations**: Read and write secrets securely
- **Dual Transport Support**: Both stdio and StreamableHTTP transports for MCP communication
- **AI Integration**: AI models use Vault tools automatically when asked about storing secrets
- **Enterprise Security**: Designed for secure secret management workflows

## Capabilities

When connected to an AI model, the Vault MCP server provides specialized tools that can:
- List all mounts and their configurations
- Create new KV v1 and KV v2 secret engines
- Delete existing mounts
- Read secret values from specified paths
- Write new secrets or update existing ones

## Security Considerations

- Intended for local use only at this stage
- Always configure MCP_ALLOWED_ORIGINS environment variable to restrict access to trusted origins
- The MCP server may expose Vault data including secrets to the MCP client and LLM
- Do not use with untrusted MCP clients or LLMs

## Available Implementations

- Official HashiCorp implementation (hashicorp/vault-mcp-server)
- Multiple community implementations available

## Compatibility

Compatible with Claude for Desktop and other MCP clients supporting stdio or StreamableHTTP transport.

## Pricing

Open-source implementation. Vault pricing applies separately based on HashiCorp Vault licensing.