## Overview

The AWS Core MCP Server is a key component in the AWS MCP ecosystem, recommended as the starting point for every new project in custom instructions for tools like Cline.

## Installation

Install using uv:
- macOS/Linux: `uvx awslabs.core-mcp-server@latest`
- Windows: `uv tool run --from awslabs.core-mcp-server@latest awslabs.core-mcp-server.exe`

## Configuration

Example for ~/.kiro/settings/mcp.json (macOS/Linux):
```json
{
  "mcpServers": {
    "awslabs-core-mcp-server": {
      "command": "uvx",
      "args": ["awslabs.core-mcp-server@latest"],
      "env": {
        "FASTMCP_LOG_LEVEL": "ERROR"
      }
    }
  }
}
```
Similar configurations apply to Cline, Cursor, Windsurf, VS Code with platform-specific variations.

## License

Apache 2.0