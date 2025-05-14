# ida-pro-mcp

**Category:** Code Execution Automation MCP Servers  
**Tags:** mcp, reverse-engineering, automation, ai-integration

## Description
The IDAPRO MCP Server is a middleware component that connects AI assistants with IDA Pro, a leading reverse engineering tool. It enables automation and remote control of IDA Pro operations through a RESTful HTTP API, facilitating tasks such as script execution, binary data retrieval, and advanced binary analysis.

## Features
- Acts as a bridge between AI assistants and IDA Pro
- Executes Python scripts within IDA Pro via remote API
- Retrieves binary data such as:
  - Strings
  - Functions
  - Exports and imports
- Supports searching for:
  - Immediate values
  - Text
  - Byte sequences
- Provides disassembly output for specified address ranges
- Automates repetitive IDA Pro operations through a REST API
- Includes:
  - IDA Pro plugin (`ida_remote_server.py`)
  - TypeScript client
  - Main server component
- Exposes HTTP endpoints for remote control (localhost by default)
- Supports automation in reverse engineering workflows
- Designed for integration with AI assistants and scripting tools
- Secure by default (localhost restriction for communication)
- Tested with IDA Pro 8.3 or later

## Applications
- Automated binary analysis and reverse engineering
- Integrating IDA Pro actions into AI-driven workflows
- Remote scripting of large-scale or repetitive IDA Pro tasks
- Vulnerability discovery and malware analysis

## Requirements
- IDA Pro version 8.3+
- Node.js 18+
- TypeScript

## Pricing
No pricing information is provided; likely open source or free to use based on available content.

## Source
[Visit IDAPRO MCP Server](https://creati.ai/mcp/mcp-server-idapro/)