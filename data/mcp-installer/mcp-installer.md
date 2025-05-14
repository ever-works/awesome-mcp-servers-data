# MCP Installer

A command-line tool to automate the installation and configuration of MCP (Model Context Protocol) servers for Claude Desktop on macOS.

**Source:** [GitHub Gist](https://gist.github.com/sidpan1/16d7719903d64ab876ea76ea51af3117)

## Features

- **Automatic Installation:** Installs and configures various MCP servers for Claude Desktop with a single script.
- **Dependency Checks:** Verifies and installs required dependencies (jq, Node.js/npx, uv/uvx) as needed.
- **Directory Management:** Sets up necessary directories for code and data storage.
- **Configuration Backup:** Automatically backs up existing Claude Desktop configuration before making changes.
- **Selective Server Installation:** Allows users to choose which MCP servers to install, including:
  - YouTube Transcript
  - DuckDuckGo Search
  - Fetch (web content)
  - Filesystem access
  - Git integration
  - Memory storage
  - Shell command execution
  - Python REPL
  - Sequential Thinking
  - Playwright (browser automation)
  - Obsidian integration
  - ClickHouse database
  - Kubernetes
  - Figma
- **API Key Prompts:** Prompts for necessary API keys for certain integrations (e.g., Figma, Obsidian, ClickHouse).
- **Optional Claude Restart:** Offers to automatically restart Claude Desktop after configuration changes.
- **Configurable Paths:** Lets users specify the base directory for code and data.
- **Config Restoration:** Creates a backup of the original configuration file for easy restoration.

## Requirements

- macOS
- Claude Desktop installed
- Basic command-line tools
- Internet connection

## Pricing

This tool is open-source and available for free via the provided GitHub Gist.

## Tags

installer, deployment, mcp, open-source
