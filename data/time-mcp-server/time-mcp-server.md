## Overview

The Time MCP Server is an official Anthropic implementation that provides time and timezone conversion tools for AI assistants to handle localized time data and calculations. It addresses Claude's lack of native timestamp awareness.

## Why It's Needed

One of Anthropic's design decisions was to deprive Claude of built-in timestamps. The Time MCP server solves this limitation by providing reliable time information and timezone conversion capabilities.

## Key Features

- **Current Time Access**: Get current time for any IANA timezone
- **Timezone Conversion**: Convert time between specified timezones
- **UTC Offset Information**: Provides UTC offset for any timezone
- **DST Status**: Reports Daylight Saving Time status
- **Automatic Detection**: Auto-detects system timezone
- **IANA Timezone Support**: Works with all IANA timezone identifiers
- **Date Information**: Returns complete date and time data

## Available Tools

**1. Get Current Time**
- Returns current time for specified timezone
- Includes date, time, UTC offset, and DST status
- Defaults to system timezone if not specified
- Supports all IANA timezone names (e.g., America/New_York, Europe/London, Asia/Tokyo)

**2. Convert Time**
- Converts time between specified source and target timezones
- Handles DST transitions automatically
- Maintains accuracy across timezone boundaries
- Supports historical and future date conversions

## IANA Timezone Support

Supports all standard IANA timezone identifiers including:

- **Americas**: America/New_York, America/Los_Angeles, America/Chicago, etc.
- **Europe**: Europe/London, Europe/Paris, Europe/Berlin, etc.
- **Asia**: Asia/Tokyo, Asia/Shanghai, Asia/Kolkata, etc.
- **Pacific**: Pacific/Auckland, Pacific/Fiji, etc.
- **UTC**: UTC and all UTC offset variants

## Use Cases

- **Scheduling**: Schedule meetings across timezones
- **Event Planning**: Plan events for global audiences
- **Time Tracking**: Log activities with accurate timestamps
- **Deadline Management**: Handle deadlines in different timezones
- **Global Coordination**: Coordinate activities across time zones
- **Time-Based Logic**: Implement time-dependent features
- **Logging**: Add timestamps to AI-generated logs
- **Compliance**: Meet timezone-specific regulatory requirements

## Remote Access

For remote sessions like Claude Code /cowork, local MCP servers aren't accessible. Remote hosted versions of the Time MCP server solve this problem, allowing access from any environment.

## Installation

Multiple installation methods:

**Via pip:**
```bash
pip install mcp-server-time
```

**Direct execution:**
```bash
uvx mcp-server-time
```

**Via npm:**
```bash
npx @modelcontextprotocol/server-time
```

## Community Alternatives

Several community implementations provide additional features:

- **MCP Time Server** by 501336North
- **DateTime MCP Server** by odgrim
- **Simple Time MCP Server** by katomato65
- **Remote MCP Time Server** on Cloudflare by iamajeesh

Each offers specific enhancements for different use cases.

## Integration

Compatible with all MCP clients:

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Other MCP-compatible assistants

## Example Queries

- "What time is it in Tokyo right now?"
- "Convert 3 PM EST to London time"
- "What's the UTC offset for Sydney?"
- "Is New York currently observing DST?"
- "What's the time difference between Paris and San Francisco?"

## Technical Details

- Supports all IANA timezone database identifiers
- Handles DST transitions automatically
- Provides historical timezone data
- Accurate to the second
- Cross-platform compatibility

## Response Format

Typical response includes:

- Current date and time
- Timezone identifier
- UTC offset
- DST status (active/inactive)
- Formatted time string

## Pricing

Free and open-source under the MIT License.