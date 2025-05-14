# GitHub MCP Server

**Source:** [github/github-mcp-server](https://github.com/github/github-mcp-server)

**Category:** Development Tools / MCP Servers  
**Tags:** mcp, github, repository-management, open-source

---

## Description

GitHub MCP Server is the official Model Context Protocol (MCP) server for GitHub, providing integration with GitHub APIs to enable advanced automation, repository management, pull requests, issues handling, and more. It is designed for developers and tool builders to automate workflows, extract and analyze repository data, and build AI-powered applications interacting with GitHub.

---

## Features

### General
- Open source (MIT License)
- Written in Go
- Can be run via Docker or built from source
- Supports configuration overrides and i18n for tool descriptions
- Can be used with VS Code, Claude Desktop, and other MCP-compatible tools
- Supports GitHub Enterprise Server via custom host configuration

### User Management
- `get_me`: Retrieve details of the authenticated user

### Issues
- `get_issue`: Get contents of a specific issue
- `create_issue`: Create a new issue
- `add_issue_comment`: Add a comment to an issue
- `list_issues`: List and filter repository issues
- `update_issue`: Update an existing issue
- `search_issues`: Search for issues and pull requests

### Pull Requests
- `get_pull_request`: Get details of a pull request
- `list_pull_requests`: List and filter pull requests
- `merge_pull_request`: Merge a pull request
- `get_pull_request_files`: List files changed in a pull request
- `get_pull_request_status`: Get combined status of all checks
- `update_pull_request_branch`: Update PR branch from base branch
- `get_pull_request_comments`: Get review comments on a PR
- `get_pull_request_reviews`: Get reviews on a PR
- `create_pull_request_review`: Create a review on a PR
- `create_pull_request`: Create a new pull request

### Repository Management
- `create_or_update_file`: Create or update a file
- `push_files`: Push multiple files in a single commit
- `search_repositories`: Search for repositories
- `create_repository`: Create a new repository
- `get_file_contents`: Get contents of a file or directory
- `fork_repository`: Fork a repository
- `create_branch`: Create a new branch
- `list_commits`: List commits on a branch

### Search
- `search_code`: Search for code across repositories
- `search_users`: Search for GitHub users

### Code Scanning
- `get_code_scanning_alert`: Get a code scanning alert
- `list_code_scanning_alerts`: List code scanning alerts for a repository

### Repository Content Retrieval
- Retrieve content by path, branch, tag, commit, or pull request number

---

## Installation & Usage
- Docker-based deployment (recommended)
- Binary build from source (requires Go)
- VS Code and Claude Desktop integration examples provided
- Requires a GitHub Personal Access Token with appropriate permissions

---

## License
MIT License

---

## Pricing
The GitHub MCP Server is open source and free to use under the MIT License.
