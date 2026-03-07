## Overview

The Git MCP server is an official Anthropic implementation providing comprehensive tools to read, search, and manipulate Git repositories. It enables AI assistants to interact with local Git repositories for version control tasks, code analysis, and repository management.

## Key Features

- **Repository Reading**: Access commit history, branches, and tags
- **Code Search**: Search through repository contents and history
- **Branch Management**: Create, switch, and manage branches
- **Commit Operations**: View commit details, diffs, and metadata
- **Status Checking**: Check working directory and staging area status
- **Log Analysis**: Analyze commit history and patterns
- **Diff Generation**: Generate diffs between commits, branches, or files
- **Repository Manipulation**: Perform Git operations through AI commands

## Security

Anthtropic has fixed three bugs in the official Git MCP server that researchers found could be chained with other MCP tools to remotely execute malicious code or overwrite files via prompt injection. The flaws affect default deployments of mcp-server-git prior to version 2025.12.18.

**Important**: Users should ensure they're using version 2025.12.18 or later for secure deployments.

## Use Cases

- **Code Analysis**: Analyze repository history and code patterns
- **Branch Strategy**: Manage branching workflows and merges
- **Commit History**: Explore and understand project evolution
- **Code Review**: Review changes and diffs between versions
- **Repository Insights**: Generate insights from Git history
- **Automated Git Operations**: Perform Git tasks via natural language
- **Project Documentation**: Extract information from commit messages
- **Contributor Analysis**: Analyze contributor patterns and activity

## Available Operations

**Reading:**
- Read commit history
- View file contents at specific commits
- List branches and tags
- Show repository status
- Display commit details

**Searching:**
- Search commit messages
- Search code across history
- Find commits by author
- Filter by date ranges

**Analysis:**
- Generate diffs
- Compare branches
- Analyze commit patterns
- Track file changes over time

**Management:**
- Create branches
- Switch branches
- View repository configuration

## Integration with Development Tools

Development tools companies including Zed, Replit, Codeium, and Sourcegraph are working with MCP to enhance their platforms—enabling AI agents to better retrieve relevant information to understand the context around coding tasks.

## Claude Desktop Integration

The setup allows Claude to analyze and interact with Git repositories directly, providing powerful code analysis and version control capabilities through conversational commands.

## Technical Details

- Part of official modelcontextprotocol/servers repository
- TypeScript implementation
- Works with local Git repositories
- Supports all major Git operations
- Cross-platform compatibility

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Zed
- Replit
- Other MCP-compatible AI assistants

## Configuration

Typically configured to work with local repositories. Can be scoped to specific repository paths for security.

## Pricing

Free and open-source under the MIT License.