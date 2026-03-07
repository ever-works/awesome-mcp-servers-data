## Overview

Notion MCP is a hosted server that gives AI tools secure access to your Notion workspace, designed to work seamlessly with popular AI assistants like Claude Code, Cursor, VS Code, ChatGPT, and more. It provides a token-efficient, Markdown-based API optimized for AI consumption.

## Key Features

- **Easy OAuth Setup**: Simple OAuth sign-in process, no manual token management
- **Full Workspace Access**: AI tools can read and write to Notion pages and databases
- **Markdown Optimization**: Data formatted efficiently for AI token usage
- **Remote Hosted Server**: Available at https://mcp.notion.com/sse
- **Open-Source Option**: Self-hosted implementation available via notion-mcp-server package
- **Streaming Support**: Token-efficient streaming via Server-Sent Events (SSE)
- **Rate Limiting**: Built-in rate limit handling

## Connection Options

**1. Remote Hosted MCP Server (Recommended)**
- URL: https://mcp.notion.com/sse
- OAuth sign-in included
- Token-efficient streaming
- Optimized for AI usage
- No setup or maintenance required

**2. Self-Hosted Open Source**
- Full control over setup and behavior
- Great for teams with existing Notion integrations
- Ideal for custom infrastructure requirements
- Available via npm: `notion-mcp-server`

## Supported Operations

- **Page Operations**: Create, read, update, and delete Notion pages
- **Database Operations**: Query, filter, and modify database entries
- **Block Management**: Manipulate page content blocks
- **Search**: Search across workspace content
- **Comments**: Add and retrieve comments
- **User Management**: Access user information and permissions

## AI Tool Compatibility

- Claude Code
- Claude Desktop
- Cursor
- Visual Studio Code with Copilot
- ChatGPT
- Windsurf
- Other MCP-compatible AI assistants

## Use Cases

- AI-assisted documentation writing
- Knowledge base management
- Meeting notes automation
- Project documentation generation
- Content organization and tagging
- Cross-page content search
- Template-based page creation
- Database-driven workflows

## OAuth Integration

Notion MCP uses OAuth Dynamic Client Registration according to the MCP specification:

- Secure authentication flow
- No manual token creation needed
- Workspace-level permissions
- Automatic token refresh

## Markdown API Benefits

The Markdown-based API provides:

- Lower token usage compared to JSON
- Better AI comprehension
- Efficient data transmission
- Natural language alignment
- Reduced API call overhead

## Documentation Resources

- Main documentation: https://developers.notion.com/docs/mcp
- Getting started: https://developers.notion.com/docs/get-started-with-mcp
- Supported tools: https://developers.notion.com/docs/mcp-supported-tools
- Self-hosting guide: https://developers.notion.com/docs/hosting-open-source-mcp

## Rate Limits

Built-in rate limit handling ensures compliance with Notion API limits while maintaining optimal performance for AI operations.

## Security

- OAuth 2.0 authentication
- Workspace-level access control
- Integration permissions management
- Secure credential storage

## Pricing

Notion workspace subscription required. MCP server access included with Notion plans.