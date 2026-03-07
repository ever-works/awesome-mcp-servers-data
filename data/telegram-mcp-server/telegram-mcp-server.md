## Overview

Telegram MCP Server is a comprehensive Telegram integration for Claude, Cursor, and any MCP-compatible client, powered by Telethon and the Model Context Protocol. This server exposes extensive Telegram capabilities, making nearly every major Telegram/Telethon feature available as a tool.

## Key Features

- **Chat Management**: Read messages, send texts, manage conversations
- **Group Administration**: Create groups, manage members, configure settings
- **Media Handling**: Upload and send photos, videos, documents, and other media
- **Message Operations**: Send, modify, delete, forward messages
- **Contact Management**: Add, remove, and manage contacts
- **Settings Control**: Manage user and chat settings
- **Bot Integration**: Build and manage Telegram bots
- **Message Splitting**: Automatic handling of Telegram's 4096 character limit
- **Error Handling**: Comprehensive error management for reliable operations
- **MTProto Support**: Direct Telegram API access via MTProto protocol

## Available Implementations

**1. chigwell/telegram-mcp** (Full-featured, Telethon-based)
- Most comprehensive implementation
- Powered by Telethon for full Telegram API access
- Extensive feature set covering all major operations
- Production-ready with robust error handling

**2. sparfenyuk/mcp-telegram** (MTProto-based)
- Direct MTProto protocol integration
- Currently provides read-only access
- Lightweight and focused on message retrieval
- Secure connection management

**3. siavashdelkhosh81/telegram-bot-mcp-server** (Bot API)
- Built on Telegram Bot API
- Automatic message splitting for long texts
- NPX support for easy execution: `npx telegram-bot-mcp-server`
- Focused on bot operations

**4. Composio Telegram MCP**
- 18+ tools for communication and messaging automation
- Quick setup (minutes)
- Enterprise-grade integration
- Comprehensive automation capabilities

**5. IQAIcom/mcp-telegram**
- Bridges LLMs and Telegram messaging
- Direct interaction through AI context window
- Channel and group management
- Message automation

## Core Capabilities

**Messaging:**
- Send text messages to users, groups, channels
- Format messages with Markdown or HTML
- Reply to specific messages
- Forward messages between chats
- Edit and delete messages
- Pin important messages

**Chat Operations:**
- Create private chats
- Create and manage groups
- Create and manage channels
- Join and leave chats
- Mute and unmute conversations
- Archive and unarchive chats

**Media Management:**
- Send photos with captions
- Upload videos
- Share documents and files
- Send voice messages
- Share locations
- Send contacts

**Group Administration:**
- Add and remove members
- Promote and demote admins
- Configure group permissions
- Manage group settings
- Create polls
- Schedule messages

**Bot Functionality:**
- Create inline keyboards
- Handle callback queries
- Process commands
- Manage bot settings
- Set bot commands

## Use Cases

- **Customer Support**: Automate customer interactions on Telegram
- **Notifications**: Send automated alerts and updates
- **Community Management**: Manage Telegram groups and channels
- **Content Distribution**: Share content across channels
- **Data Collection**: Gather information through bot interactions
- **Integration Hub**: Connect Telegram with other services
- **Automated Responses**: Intelligent reply automation
- **Broadcasting**: Mass messaging to users or channels

## Authentication & Security

**API Credentials Required:**
- Telegram API ID
- Telegram API Hash
- Phone number (for user accounts)
- Bot token (for bot operations)

**Security Features:**
- Secure credential storage
- Two-factor authentication support
- Session management
- Encryption support
- Permission-based access control

## Message Splitting

Automatic handling of Telegram's 4096 character limit:

- Long messages automatically split into multiple parts
- Preserves message formatting
- Maintains message context
- Handles Unicode correctly

## Installation Examples

**NPX (for bot-based server):**
```bash
npx telegram-bot-mcp-server
```

**Via npm:**
```bash
npm install telegram-mcp
```

**Via pip (Python implementations):**
```bash
pip install mcp-telegram
```

## Configuration

Typical configuration requires:

- **API ID**: From Telegram's app registration
- **API Hash**: From Telegram's app registration
- **Phone Number**: For user account access (or bot token for bots)
- **Session Name**: For storing authentication session

## Natural Language Operations

Example AI interactions:

- "Send a message to the engineering group saying the deployment is complete"
- "What are the latest messages in my personal chat?"
- "Create a new channel called 'Product Updates'"
- "Upload this image to the marketing channel"
- "Add John to the project group"

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Custom MCP implementations

## Telegram API Access

**MTProto Protocol:**
- Direct Telegram server communication
- Lower-level API access
- Better performance
- Advanced features

**Bot API:**
- Simpler integration
- Bot-specific features
- Easier setup
- Good for automated tasks

## Error Handling

Comprehensive error management for:

- Network connectivity issues
- API rate limits
- Authentication failures
- Invalid operations
- Permission errors
- Malformed requests

## Rate Limiting

Respects Telegram's rate limits:

- Automatic retry with backoff
- Queue management for bulk operations
- Smart throttling

## Pricing

Free and open-source. Telegram API usage is free with rate limits. No Telegram subscription required for basic features.