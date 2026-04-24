## Overview

Python MCP server to control a Minecraft server via RCON, using FastMCP.

## Features

- Exposes a set of commands (dictionary) to contextualize the LLM
- Executes commands on the Minecraft server via RCON
- Integration with Claude Desktop or any MCP client
- Simple structure: stdio (local development) or HTTP/SSE (production)
- Chat client (`mcp_chat_client.py`) that listens to @ai messages from Minecraft chat, sends to Gemini API, and executes commands

## Project Structure

```
mcp_server/
├── .env
├── commands.json
├── mcp_chat_client.py
├── server.py
├── requirements.txt
```

## Setup

- Enable RCON in `server.properties`: `enable-rcon=true`, set password and port
- Configure `.env` with Minecraft log path, server path, Gemini API key

## Running

- Install dependencies: `pip install -r requirements.txt`
- Run server: `python mcp_server/server.py`
- Run chat client: `python mcp_server/mcp_chat_client.py`

## Integration

Supports Claude Desktop via `claude_desktop_config.json` with stdio command.

## Local Testing

Use FastMCP Client to call `run_minecraft_command` tool and read `minecraft://commands` resource.

## Pricing

Free and open-source under the Apache 2.0 license.