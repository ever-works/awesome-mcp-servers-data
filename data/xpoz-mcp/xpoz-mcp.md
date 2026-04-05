## Overview

Xpoz MCP is an MCP server that provides multi-platform social media intelligence through a single integration. It indexes over 1.5 billion posts across Twitter/X, Instagram, TikTok, and Reddit, enabling natural language queries via AI assistants like Claude and ChatGPT.

## Platforms Covered

- Twitter/X
- Instagram
- TikTok
- Reddit

## Key Features

- 1.5B+ indexed posts
- Natural language query support
- Historical data access
- User and engagement analysis
- Network and follower analysis
- CSV export capability
- No per-request rate limits
- No API keys required for setup

## Example Queries

- Find tweets about topics with specific engagement thresholds
- Identify influential accounts in a niche
- Track brand mentions over time
- Analyze competitor discussions across platforms

## Pricing

| Tier | Results/Month | Cost |
|------|---------------|------|
| Free | 100,000 | $0 |
| Pro | 1,000,000 | $20 |
| Max | 10,000,000 | $200 |

## Use Cases

- **Brand Monitoring**: Track mentions across Twitter, Instagram, Reddit, and TikTok simultaneously
- **Competitor Analysis**: Compare performance across platforms and analyze follower networks
- **Research**: Query historical and current social media data for trend analysis
- **Monitoring**: Regularly query for recent mentions and flag significant changes

## Setup

Compatible with Claude Desktop via MCP server configuration:

```json
{
  "mcpServers": {
    "xpoz": {
      "command": "npx",
      "args": ["-y", "@anthropic-ai/mcp-server-xpoz"],
      "env": {
        "XPOZ_API_KEY": "your-api-key"
      }
    }
  }
}
```

Also supports ChatGPT with MCP integration.