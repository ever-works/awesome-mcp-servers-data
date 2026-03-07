## Overview

Jira MCP refers to the integration of Atlassian Jira with the Model Context Protocol, allowing large language models and AI agents to interact securely and efficiently with Jira. The official Atlassian Rovo MCP Server is a cloud-based bridge between your Atlassian Cloud site and compatible external tools.

## Key Features

- **Project Management**: List accessible projects, retrieve detailed project information, discover project statuses
- **Issue Management**: Search issues using JQL, view detailed issue data, filter by status or project
- **Development Insights**: Access related commits, pull requests, and branches for specific issues
- **Comment and Worklog Handling**: View, add, update, and delete comments and worklogs
- **Workflow Navigation**: Explore available issue statuses to facilitate workflow automation
- **JQL Search**: Powerful Jira Query Language support for complex searches
- **Secure Integration**: OAuth authentication and permission-based access
- **Cloud & Data Center Support**: Works with both Atlassian Cloud and Server/Data Center
- **Real-Time Data**: Interact with Jira data in real-time through the MCP bridge

## Available Implementations

**1. Official Atlassian Rovo MCP Server**
- Cloud-based managed service
- Covers Jira, Compass, and Confluence
- OAuth authentication built-in
- Enterprise-grade reliability
- No server maintenance required

**2. Community Implementations**

**sooperset/mcp-atlassian:**
- Supports both Confluence and Jira
- Works with Cloud and Server/Data Center deployments
- Self-hosted option
- Customizable configuration

**aashari/mcp-server-atlassian-jira:**
- Node.js/TypeScript implementation
- Comprehensive tool suite
- Development info integration (commits, PRs)
- JQL and ID-based search

**Composio Jira MCP:**
- Enterprise-focused integration
- Quick setup and deployment
- Advanced automation capabilities

## Core Capabilities

**Project Operations:**
- List all accessible projects
- Get project details and metadata
- View project statuses and workflows
- Explore project components
- Access project versions/releases

**Issue Operations:**
- Create new issues with fields
- Update issue details and status
- Search using JQL (Jira Query Language)
- Get issue by ID or key
- Transition issues through workflows
- Assign issues to users
- Set priority and labels

**Advanced Search:**
JQL (Jira Query Language) support enables complex queries:
- `project = ABC AND status = "In Progress"`
- `assignee = currentUser() AND created >= -7d`
- `priority = High AND resolution = Unresolved`
- Custom field filtering
- Boolean operators (AND, OR, NOT)

**Development Integration:**
- View commits linked to issues
- Access pull request information
- See branch details
- Track code changes
- Link code to issues

**Comments & Collaboration:**
- Add comments to issues
- Update existing comments
- Delete comments (with permissions)
- View comment history
- Mention users

**Time Tracking:**
- Log work on issues
- View worklog entries
- Update time estimates
- Track remaining time
- Generate time reports

## Use Cases

**Automated Issue Management:**
AI agents can automatically create, update, and manage Jira issues based on natural language commands, eliminating manual ticket creation.

**Intelligent Triage:**
Analyze and automatically categorize incoming issues, assign to appropriate teams, and set priorities based on content and context.

**Report Generation:**
Generate comprehensive reports on project status, sprint progress, and team performance through conversational queries.

**Workflow Automation:**
Automate issue transitions, status updates, and notifications based on conditions and triggers.

**Development Tracking:**
Connect code changes, commits, and pull requests to Jira issues for complete traceability.

**Sprint Planning:**
Assist with sprint planning by analyzing issue complexity, team capacity, and historical velocity.

**Customer Support:**
Automatically create and update Jira tickets from customer support interactions.

## Authentication & Security

**OAuth 2.0:**
- Secure authentication flow
- Token-based access
- Automatic token refresh
- Scoped permissions

**Permission Model:**
- Respects Jira's permission scheme
- User-level access control
- Project-level permissions
- Field-level security

**Secure Bridge:**
The Atlassian Rovo MCP Server acts as a secure, controlled bridge between AI agents and Jira instances, ensuring data security and compliance.

## Configuration

Typical configuration includes:

- **Jira URL**: Your Atlassian Cloud or Data Center URL
- **Authentication**: OAuth credentials or API token
- **Projects**: Accessible project list
- **Permissions**: User permission scope

## Natural Language Operations

Example AI interactions:

- "Create a high-priority bug for the login issue"
- "Show me all issues assigned to me that are in review"
- "What's the status of ticket ABC-123?"
- "List all open issues in the mobile project"
- "Add a comment to issue XYZ-456 saying we've deployed the fix"
- "How many hours did I log this week?"

## JQL Examples

Powerful queries via Jira Query Language:

```jql
project = PROJ AND assignee = currentUser() AND status != Done
```

```jql
created >= -30d AND priority in (High, Highest) AND resolution = Unresolved
```

```jql
project = ABC AND fixVersion = "2.0" ORDER BY priority DESC
```

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- IntelliJ IDEA with AI Assistant
- Continue
- Custom MCP implementations

## Integration Benefits

**Natural Language Interface:**
Interact with Jira using plain English instead of learning complex UI navigation.

**Automation:**
Reduce manual data entry and repetitive tasks through AI-powered automation.
**Cross-Platform:**
Access Jira functionality from any MCP-compatible AI assistant or IDE.

**Productivity:**
Create and update issues without context switching from your development environment.

**Insights:**
Generate insights and reports through conversational queries.

## Atlassian Rovo

The official Atlassian Rovo MCP Server is part of Atlassian's Rovo platform, which provides:

- Unified search across Atlassian products
- AI-powered insights
- Workflow automation
- Knowledge discovery
- Cross-product integration

## Pricing

Pricing varies by implementation:

- **Atlassian Rovo MCP**: Requires Atlassian Rovo subscription
- **Community Servers**: Free and open-source
- **Jira Subscription**: Required for all implementations

Jira pricing based on cloud or data center tier and user count.