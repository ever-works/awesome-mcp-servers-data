## Overview

Xquik MCP Server provides remote MCP access to X/Twitter data and automation workflows through Xquik. It is designed for agents that need live X data without managing a local scraper process.

## Capabilities

- Search tweets with X query operators and filters
- Look up tweets, users, trends, lists, and communities
- Fetch user timelines, followers, and follow relationships
- Download tweet media and read long-form X articles
- Create account monitors and receive webhook events
- Use write workflows such as posting, replies, likes, follows, and DMs when enabled

## Integration

The remote MCP endpoint is available at:

```text
https://xquik.com/mcp
```

Authentication uses an Xquik API key. The REST API schema is also published as OpenAPI at:

```text
https://xquik.com/openapi.json
```

## Use Cases

- Social media research and OSINT workflows
- Brand, account, and keyword monitoring
- Agentic X/Twitter search and profile enrichment
- Media extraction and webhook-driven automation
- Developer workflows that need the same X data surface through REST, SDKs, and MCP

