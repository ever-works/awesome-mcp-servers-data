## Overview

Discord MCP servers provide integration capabilities to MCP clients like Claude Desktop, enabling LLMs to interact with Discord channels, send and read messages, manage communities, and perform administrative operations through Discord's API.

## Key Features

- **Message Management**: Send, read, edit, delete messages
- **Channel Operations**: Create, configure, manage channels
- **Role Management**: Assign, modify, remove user roles
- **Moderation Tools**: Ban, kick, timeout, moderate content
- **Event Management**: Create and manage server events
- **Reaction Handling**: Add and manage message reactions
- **Thread Management**: Create and participate in threads
- **Server Administration**: Full server configuration control
- **Slash Commands**: Bot interaction via slash commands
- **Direct Messages**: Private messaging capabilities

## Available Implementations

**1. hanweg/mcp-discord**
- List servers and get server info
- Get channels and send messages
- Read messages and add reactions
- Moderate messages
- Create channels
- Manage user roles

**2. SaseQ/discord-mcp**
- Discord API (JDA) integration
- Seamless MCP application integration
- Claude Desktop compatible

**3. glittercowboy/discord-mcp**
- 128 operations for full control
- Messages, moderation, channels, roles, events
- Comprehensive community management

**4. Mastra AI Discord Bot**
- Intelligent assistance via slash commands
- Direct message support
- Threaded conversations
- Message chunking for long responses

## Deployment Options

**Quick Setup:**
```bash
npx discord-mcp-server
```

**Docker:**
```bash
docker run discord-mcp-server
```

**Local Development:**
```bash
git clone [repository]
npm install
npm start
```

**Transport Methods:**
- STDIO (standard input/output)
- HTTP (web-based communication)

## Core Capabilities

**Message Operations:**
- Send text messages
- Send embeds (rich messages)
- Upload attachments
- Edit messages
- Delete messages
- Pin/unpin messages
- React to messages
- Quote messages

**Channel Management:**
- Create text channels
- Create voice channels
- Create forum channels
- Set channel permissions
- Configure slow mode
- Set channel topics
- Archive/unarchive channels

**Role Management:**
- Create roles
- Assign roles to users
- Remove roles from users
- Set role permissions
- Set role colors
- Role hierarchy management

**Moderation:**
- Ban users
- Kick users
- Timeout users
- Delete messages
- Bulk delete messages
- Manage warnings
- View audit logs

**Event Management:**
- Create scheduled events
- Modify events
- Delete events
- Get event details
- Manage RSVPs

## Use Cases

**Community Management:**
- Automated moderation
- Welcome messages
- Role assignment based on criteria
- Server statistics tracking

**Support Systems:**
- Ticket creation
- Support queue management
- FAQ automation
- Response templates

**Engagement:**
- Polls and surveys
- Giveaways
- Event announcements
- Achievement notifications

**Gaming:**
- LFG (Looking for Group) systems
- Tournament management
- Score tracking
- Team coordination

**Education:**
- Study groups
- Assignment reminders
- Resource sharing
- Q&A sessions

## Slash Commands

Bot interactions through Discord's slash command system:

- Command registration
- Option parameters
- Autocomplete support
- Ephemeral responses
- Deferred responses for long operations

## Threaded Conversations

- Create threads from messages
- Manage thread participants
- Archive threads automatically
- Thread-specific permissions
- Search within threads

## Embed Messages

Rich message formatting:

- Title and description
- Custom colors
- Fields and inline fields
- Images and thumbnails
- Footer text
- Timestamp
- Author information

## Permission System

**Server Permissions:**
- Administrator
- Manage server
- Manage roles
- Manage channels
- Kick/ban members
- Manage messages

**Channel Permissions:**
- View channel
- Send messages
- Embed links
- Attach files
- Add reactions
- Manage messages

## Webhooks

Webhook integration for:

- External service notifications
- Custom avatars per message
- Username overrides
- Formatted messages
- Attachment support

## Voice Channels

- Create voice channels
- Set user limits
- Set bitrate
- Video support
- Go live streaming
- Stage channels

## Server Features

- **Verification**: Verification levels and requirements
- **Boosting**: Server boost status and perks
- **Discovery**: Server discovery settings
- **Analytics**: Member growth, engagement metrics
- **Integrations**: Third-party service connections

## Natural Language Examples

"Send a message to #general channel"
"Ban user @spammer for violating rules"
"Create a new role called 'Moderator'"
"Delete the last 50 messages in this channel"
"Schedule an event for Friday at 7 PM"
"Add a reaction to the latest announcement"

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Custom MCP implementations

## Authentication

- Bot token authentication
- OAuth2 for user actions
- Permissions verification
- Rate limit handling
- Token rotation support

## Rate Limits

Discord API rate limits:

- Global rate limit: 50 requests per second
- Per-route limits: Varies by endpoint
- Bucket-based limiting
- Automatic retry with backoff

## Message Chunking

Automatic handling of long messages:

- 2000 character limit per message
- Smart splitting at newlines
- Continuation indicators
- Thread creation for lengthy responses

## Error Handling

- API error codes
- Permission errors
- Rate limit handling
- Invalid parameters
- Network errors
- Graceful degradation

## Logging & Monitoring

- Command usage tracking
- Error logging
- Performance metrics
- User activity logs
- Moderation actions

## Compliance

- Discord Terms of Service
- Community Guidelines
- Data protection
- Bot verification process
- Privacy policy requirements

## Pricing

Free to use. Discord API access is free with rate limits. Discord Nitro and Server Boosting are optional paid features for enhanced capabilities.