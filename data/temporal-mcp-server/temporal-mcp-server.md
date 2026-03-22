## Overview

The Temporal MCP server acts as a bridge between AI assistants and Temporal workflow orchestration clusters. This integration turns complex backend orchestration into simple, chat-driven commands, allowing developers to interact with workflows entirely through natural language.

## Features

- **Workflow Lifecycle Management**: Start, check status, signal, cancel, and inspect workflows through natural language
- **Real-time Querying**: Query and signal running workflows in real-time
- **Batch Operations**: Execute operations across many workflows simultaneously
- **Schedule Management**: Complete schedule management via cron expressions
- **19 Tools**: Comprehensive toolset covering the full Temporal surface area
- **Config-Driven**: Define accessible workflows in a simple config.yml file

## How It Works

The server translates MCP tool calls into Temporal workflow executions. You define which workflows should be accessible in a configuration file, and the server makes them available as tools to any connected MCP client.

## Benefits

- Leverage existing workflow infrastructure without custom integration code
- Orchestrate complex, fault-tolerant processes through simple conversation
- Workflow state persists locally and workflows survive crashes
- Coordinate multi-step agent tasks with durable execution

## Use Cases

Production environments where companies rely on Temporal for orchestrating agents, multi-step processes, and fault-tolerant workflows.

## Supported Clients

GitHub Copilot, Claude, OpenCode, and any MCP-compatible AI assistant.