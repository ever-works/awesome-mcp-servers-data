## Overview

The Linear MCP Server provides a standardized interface to interact with Linear's issue tracking system, enabling comprehensive project management, issue tracking, and automation through the Model Context Protocol.

## Key Features

- **Issue Management**: Create, update, and delete issues (including subissues) with self-assign capabilities
- **Advanced Search**: Search issues using text queries and filters with logical operators and relative date filtering
- **Project & Team Management**: Retrieve projects, create project updates with health status tracking
- **Label Management**: Organize and categorize issues with labels
- **Comment System**: List and create comments on issues
- **User Management**: List users and retrieve user details
- **Status Tracking**: Manage and view issue statuses
- **Type-Safe Operations**: Comprehensive error handling and input validation
- **Rate Limit Management**: Built-in rate limiting for API stability

## Available Tools (21 Total)

The Linear MCP server provides 21 specialized tools:

**Issue Operations:**
- list_issues: List all issues with optional filters
- get_issue: Get detailed issue information with relationships
- create_issue: Create new issues with full metadata
- update_issue: Modify existing issues
- list_my_issues: Get issues assigned to current user

**Project Management:**
- list_projects: Retrieve all projects
- get_project: Get detailed project information
- create_project: Create new projects
- update_project: Modify project details
- create_project_update: Add project updates with health status

**Team & User:**
- list_teams: List teams with filtering by name/key
- get_team: Get detailed team information
- list_users: List all users
- get_user: Get user details

**Additional:**
- list_comments: View issue comments
- create_comment: Add comments to issues
- list_issue_statuses: View available statuses
- get_issue_status: Get status details
- list_labels: Manage labels
- search_documentation: Search Linear documentation

## Search Capabilities

Advanced filtering supports:

- Assignee, creator, project filters
- Status and priority filtering
- Date range queries (created, updated, completed)
- Label-based filtering
- Logical operators for complex queries
- Relative date expressions

## Use Cases

- Automated bug tracking and triage
- AI-powered issue creation from error logs
- Project status reporting
- Sprint planning automation
- Issue dependency analysis
- Team workload management
- Custom workflow automation
- Release planning assistance

## Multiple Implementations

Several providers offer Linear MCP servers:

- @cosmix/linear-mcp
- Composio Linear MCP Integration
- Tacticlaunch Linear server
- Zalab Inc Linear Issue Tracker
- Official Linear MCP (latest)

Each offers similar core functionality with varying features and deployment options.

## Integration

Compatible with AI assistants including Claude Desktop, Cursor, Windsurf, VS Code with Copilot, and other MCP-compatible tools.

## Technical Quality

- Type-safe TypeScript/JavaScript implementation
- Comprehensive error handling
- Input validation
- Rate limit management
- Well-documented API

## Pricing

Linear subscription required. Pricing based on Linear plan tier.