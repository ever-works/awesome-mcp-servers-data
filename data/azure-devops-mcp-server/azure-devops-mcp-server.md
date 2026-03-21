## Overview

The official Azure DevOps Model Context Protocol Server provides your AI assistant with secure access to work items, pull requests, builds, test plans, and documentation from your Azure DevOps organization. This TypeScript project enables you to perform a wide range of Azure DevOps tasks directly from your code editor.

## Available Domains

### Core
- Organization and project management
- Team operations
- Process templates

### Work Items
- Create, update, and query work items
- Manage work item states and transitions
- Handle backlogs and sprints
- Track bugs, tasks, and user stories

### Repositories
- Browse code repositories
- View and create pull requests
- Access commit history
- Manage branches

### Pipelines
- View build and release pipelines
- Trigger pipeline runs
- Monitor build status
- Access build artifacts

### Test Plans
- Create and manage test plans
- Execute test cases
- Track test results
- Generate test reports

### Wiki
- Search and browse wiki pages
- Create and update documentation
- Manage wiki content

### Advanced Security
- Security scanning results
- Vulnerability management
- Code security alerts
- Compliance reporting

## Key Features

### Natural Language Operations
- Query work items conversationally
- Create pull requests with descriptions
- Trigger builds using plain English
- Search code and documentation

### Team Collaboration
- Manage team boards and backlogs
- Assign work items to team members
- Review and approve pull requests
- Comment on work items and PRs

### DevOps Automation
- Automate routine DevOps tasks
- Trigger CI/CD pipelines
- Generate status reports
- Update work item states

## Use Cases

### Work Item Management
- Create bugs and tasks from code editor
- Update work item status conversationally
- Query work items by various criteria
- Link work items to commits and PRs

### Code Review Workflow
- Create pull requests with AI assistance
- Review PR comments and discussions
- Check build status before merging
- Approve or request changes on PRs

### Pipeline Operations
- Trigger builds for specific branches
- Monitor pipeline execution status
- Retrieve build logs for debugging
- Manage release deployments

### Documentation Management
- Search wiki for information
- Create and update wiki pages
- Link documentation to work items
- Maintain project knowledge base

## Integration

Works with AI assistants supporting MCP including Claude Desktop, Cursor, Windsurf, and other compatible tools. Requires Azure DevOps account and personal access token (PAT) with appropriate permissions.

## Pricing

Azure DevOps offers free tier for up to 5 users with unlimited private Git repositories. Basic plan starts at $6/user/month. MCP server is free to use with Azure DevOps.