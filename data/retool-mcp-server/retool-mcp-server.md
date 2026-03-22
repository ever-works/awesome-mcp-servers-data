## Overview

Retool has announced an official MCP server (currently in beta) that allows AI agents to inspect and query Retool organizations - apps, automations, resources, users, and more. This integration enables AI-powered management of internal tools and low-code applications through natural language.

## Features

- **Organization Inspection**: Query Retool organization structure and metadata
- **App Management**: Access and manage Retool applications
- **Automation Workflows**: Inspect and control automation workflows
- **Resource Querying**: Query database connections and API resources
- **User Management**: Access user and permission information
- **Agent Integration**: Configure MCP servers as resources for Retool agents
- **Remote MCP Support**: Connect to remote-hosted MCP servers

## Two Setup Options

### 1. Official Retool MCP Server (Beta)
- Hosted by Retool
- Query Retool organization data
- App and workflow management
- User and resource inspection

### 2. Community MCP Server
- For self-hosted Retool instances
- Create apps and manage workflows
- Full Retool instance control
- Available at TechnicalRhino/retool-mcp

## Use Cases

- AI-assisted app development in Retool
- Automated workflow management
- Resource configuration and monitoring
- User and permission auditing
- App usage analytics
- Query performance analysis
- Workflow execution monitoring

## Integration with Retool Agents

If you have a public URL for an MCP server, you can configure that MCP server as a resource and then give your Retool agent access to all the tools that server provides.

## Third-Party Integration

Retool MCP integration via Improvado connects Retool data to AI agents, allowing teams to:
- Query app usage metrics
- Analyze query performance
- Monitor workflow execution
- Use plain-language prompts for data access

## Current Limitations

Retool currently only supports remote-hosted MCPs. Local MCP servers need to be exposed via public URLs.

## Compatibility

Works with Claude, Cursor, Windsurf, and any MCP-compatible AI assistant.

## Pricing

Retool offers a free tier for up to 5 users. Professional and Enterprise plans available for larger teams and advanced features.