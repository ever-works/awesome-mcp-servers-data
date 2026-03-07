## Overview

The GitHub MCP Server is an official Anthropic implementation providing comprehensive GitHub repository management, file operations, and GitHub API integration. It enables AI assistants to interact with GitHub repositories, manage issues, handle pull requests, and analyze code through the Model Context Protocol.

## Key Features

- **Repository Management**: Create, read, update, and manage GitHub repositories
- **File Operations**: Access, modify, and manage repository files
- **Issue Tracking**: Create, update, search, and manage GitHub issues
- **Pull Request Handling**: Create, review, merge, and manage pull requests
- **Code Analysis**: Analyze code structure, commits, and changes
- **File Structure Mapping**: Navigate and understand repository organization
- **GitHub API Integration**: Full access to GitHub's comprehensive API
- **Branch Management**: Create, switch, merge, and delete branches
- **Commit Operations**: View commit history, diffs, and metadata
- **Collaboration**: Comment on issues, PRs, and code reviews

## Usage Statistics

According to FastMCP analysis of 1,864+ MCP servers, GitHub ranks #7 with 3,100 views and 204 installs, reflecting the central role GitHub plays in modern development.

## Available Operations

**Repository Operations:**
- List repositories for user or organization
- Create new repositories
- Clone repositories
- Fork repositories
- Archive or delete repositories
- Configure repository settings

**File and Content:**
- Read file contents
- Create new files
- Update existing files
- Delete files
- Search code across repositories
- Navigate directory structures

**Issues Management:**
- Create issues with labels, assignees, milestones
- Update issue details
- Search issues with filters
- Add comments
- Close or reopen issues
- Manage labels and milestones

**Pull Requests:**
- Create pull requests
- Review code changes
- Add review comments
- Request changes or approve
- Merge pull requests
- Handle merge conflicts

**Code Analysis:**
- View commit history
- Generate diffs
- Analyze code quality
- Track changes over time
- Identify contributors

## Integration with Development Tools

Development tools companies including Zed, Replit, Codeium, and Sourcegraph are working with MCP to enhance their platforms—enabling AI agents to better retrieve relevant information to understand the context around coding tasks.

## Claude for Work Integration

All Claude.ai plans support connecting MCP servers to the Claude Desktop app, and Claude for Work customers can begin testing MCP servers locally, connecting Claude to internal GitHub systems and datasets.

## Use Cases

- **Automated Issue Management**: Create and triage issues through AI
- **Code Review Assistance**: AI-powered code review and feedback
- **Documentation Generation**: Auto-generate README and docs
- **Project Analysis**: Analyze repository structure and dependencies
- **Pull Request Automation**: Create and manage PRs conversationally
- **Repository Maintenance**: Automate routine maintenance tasks
- **Contribution Tracking**: Analyze contributor patterns
- **Release Management**: Assist with release notes and versioning

## Security and Authentication

- **Personal Access Tokens**: Secure authentication via GitHub PAT
- **OAuth Integration**: Full OAuth 2.0 support
- **Permission Scoping**: Granular control over API access
- **Repository Access**: Respects GitHub's permission model
- **Rate Limiting**: Handles GitHub API rate limits intelligently

## Natural Language Queries

Example interactions:

- "Create a new issue for the bug I just described"
- "Show me the last 5 pull requests"
- "What files changed in the latest commit?"
- "Create a PR with these changes"
- "Find all open issues labeled 'bug'"
- "Who are the top contributors to this repository?"

## Technical Details

- Part of official modelcontextprotocol/servers repository
- TypeScript/JavaScript implementation
- Full GitHub REST API v3 support
- GraphQL API support for complex queries
- Webhook integration capabilities

## Installation

Available via npm:
```bash
npx @modelcontextprotocol/server-github
```

Requires GitHub Personal Access Token with appropriate scopes.

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Zed
- Replit
- Codeium
- Sourcegraph
- Other MCP-compatible AI assistants

## API Coverage

Provides access to:

- Repositories API
- Issues API
- Pull Requests API
- Commits API
- Contents API
- Search API
- Users API
- Organizations API
- Teams API
- Actions API (GitHub Actions)
- Packages API

## Pricing

Free and open-source under the MIT License. GitHub API usage subject to GitHub's rate limits and terms of service.