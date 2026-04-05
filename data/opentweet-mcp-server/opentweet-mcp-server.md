## Overview

OpenTweet's MCP server is purpose-built for Twitter/X. It is the most complete Twitter MCP server available, with 12 tools covering the full tweet lifecycle — from drafting to publishing to analytics. No Twitter developer account is needed, as OpenTweet handles the X API connection.

## Features

- Create and schedule tweets and threads (up to 25 tweets per thread)
- Batch schedule up to 50 tweets at once
- Upload images and videos
- Get detailed analytics (impressions, engagement, best posting times)
- Track follower growth
- Manage drafts
- Publish immediately or schedule for later
- AI-native workflow — Claude writes AND publishes tweets in one conversation
- MCP resources (scheduled posts, drafts, analytics summary)
- MCP prompt templates (weekly content plan, performance review)

## Setup

Install via npx:
```
npx @opentweet/mcp-server
```

MCP configuration:
```json
{
  "mcpServers": {
    "opentweet": {
      "command": "npx",
      "args": ["-y", "@opentweet/mcp-server"],
      "env": {
        "OPENTWEET_API_KEY": "ot_your_key_here"
      }
    }
  }
}
```

## Pricing

- The MCP server is free and open-source
- Requires an OpenTweet account starting at $11.99/month
- 7-day free trial available

## Best For

Developers, indie hackers, solopreneurs, and content creators who are focused on Twitter/X and want a complete AI-powered workflow.