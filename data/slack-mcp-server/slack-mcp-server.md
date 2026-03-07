## Overview

The Slack MCP server enables integrated apps to search channels, send messages, and perform other Slack actions through MCP clients. Model Context Protocol is a specification for exchanging context, capabilities, and structured actions between clients and servers.

## Key Features

- **Message Search**: Search for messages and files with filtering by date, user, and content type
- **User Search**: Find users in workspace by name (partial matching), email, and user ID with detailed profiles
- **Message Sending**: Send messages to any conversation type in Slack
- **Message Threading**: Grab complete message thread conversations
- **Canvas Management**: Create and share rich, formatted documents
- **Canvas Export**: Export canvases as markdown files
- **Message Drafting**: Format and preview messages within AI clients
- **No Permission Requirements**: Powerful server with minimal permission needs
- **Apps Support**: Full Slack Apps API integration
- **GovSlack**: Support for government Slack instances
- **DMs & Group DMs**: Direct message and group direct message support
- **Smart History Fetch**: Intelligent message history retrieval logic

## Search Capabilities

**Message & File Search:**
- Filter by date ranges
- Filter by user/author
- Filter by content type (messages, files, or both)
- Retrieve metadata and content
- Support for attachments and file previews

**User Search:**
- Partial name matching
- Email-based lookup
- User ID search
- Retrieve user details, status, and presence

## Messaging Features

- Send to channels, DMs, and group conversations
- Draft and preview before sending
- Rich text formatting support
- Attachment handling
- Emoji and reaction support
- Thread participation

## Canvas Capabilities

Canvases are Slack's rich document format:

- Create formatted documents
- Share across workspace
- Export as markdown
- Collaborative editing support
- Structured content organization

## Setup Requirements

To use Slack MCP:

1. Create a Slack app in your workspace
2. Configure necessary bot token scopes
3. Install the app to your workspace
4. Configure MCP client with bot token

## Available Commands

- Channel management
- Message posting and threading
- User information retrieval
- File and content search
- Canvas creation and management
- Workspace metadata access

## Multiple Implementations

Several Slack MCP implementations available:

- Official Slack documentation server
- korotovsky/slack-mcp-server (most powerful)
- Composio Slack MCP Integration
- Workato enterprise integration

## Use Cases

- Automated message responses
- Team activity monitoring
- Cross-channel content search
- Meeting notes and documentation
- Incident response automation
- Onboarding automation
- Status update aggregation
- Knowledge base integration

## Integration

Compatible with Claude Desktop, Cursor, VS Code, Windsurf, and other MCP clients.

## Security

- OAuth 2.0 authentication
- Bot token scopes for granular permissions
- Workspace-level access controls
- Audit logging

## Pricing

Slack workspace subscription required. Pricing based on Slack plan tier.