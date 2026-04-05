## Overview

The Model Context Protocol (MCP) is an open standard that provides AI models with a universal way to connect to external tools, data sources, and services. Anthropic introduced it in November 2024, and it has since become the de facto protocol for connecting AI to the real world, adopted by OpenAI, Google DeepMind, Microsoft, and thousands of development teams.

In December 2025, Anthropic donated MCP to the Agentic AI Foundation under the Linux Foundation, making it a vendor-neutral, community-governed standard.

## Architecture

MCP operates around three roles:

- **Host**: The AI application the user interacts with (Claude Desktop, Cursor, ChatGPT, custom apps)
- **Client**: Lives inside the host, manages connections to MCP servers in a one-to-one relationship with each server
- **Server**: Exposes capabilities to the AI through the protocol

A single host can run many clients simultaneously, each connected to a different server.

## Core Primitives

MCP servers present capabilities through three primitives:

- **Tools**: Actions the AI can take (send a message, create a record, run a query, trigger a deployment). The write side of MCP.
- **Resources**: Data the AI can read (files, database rows, API responses, documents). The read side of MCP.
- **Prompts**: Reusable templates that guide the AI's behavior for specific tasks.

## Transport Mechanisms

- **stdio**: Runs servers as local subprocesses of the host, communicating through standard input/output. Ideal for desktop applications and development tools.
- **Streamable HTTP**: Supports remote servers deployed anywhere on the internet, using standard HTTP and Server-Sent Events for real-time streaming. Compatible with existing load balancers, proxies, and CDNs.

Connections are stateful, allowing servers to remember context across multiple requests within a workflow.

The wire format is JSON-RPC 2.0.

## Key Features

### Async Tasks
Any request can return a task handle immediately while the real work continues in the background. Clients can poll or subscribe for progress updates. Tasks move through defined states: working, input_required, completed, failed, cancelled.

### Sampling
Servers can request completions from the AI model during execution, enabling intermediate reasoning, assumption validation, or content generation as part of multi-step processes. Users can review and edit sampled output before it goes back.

### Elicitation
- **URL-mode**: Redirects users to trusted external URLs for OAuth flows, credential entry, or payment setup
- **Form-mode**: Handles structured input when the server needs clarification before proceeding

### Server-side Agent Loops
Servers can include tool definitions in sampling requests, specify tool choice behavior, and implement multi-step reasoning internally.

### MCP Apps
Launched January 2026 as the first official MCP extension. Tools can return rich HTML interfaces that render in sandboxed iframes within the chat experience. Co-developed with OpenAI. Works in Claude, ChatGPT, Goose, and VS Code. Launch partners include Amplitude, Asana, Box, Canva, Clay, Figma, Hex, monday.com, Slack, and Salesforce.

## Authentication

- **Local servers (stdio)**: Auth handled by the host application's permissions; server inherits access from the running app
- **Remote servers**: OAuth 2.1 flow with PKCE, token scoping, and consent screens
- **Client ID Metadata Documents (CIMD)**: Default client registration mechanism where client identity is a URL pointing to a JSON document
- **Resource Indicators (RFC 8707)**: Prevents token issued for one server from accessing another

## Ecosystem

- **Clients**: Claude, ChatGPT, Gemini, Microsoft Copilot, GitHub Copilot, Cursor, Windsurf, VS Code, Zed
- **Servers**: Slack, GitHub, Google, Salesforce, Stripe, HubSpot, Shopify, Notion, Linear, Sentry, Figma, Webflow, Cloudflare, Postman, WooCommerce, and many others
- **Official SDKs**: TypeScript and Python
- **Community SDKs**: Java, Kotlin, C#, Go, Rust, Swift
- **MCP Registry**: Central index for discovering servers with nearly 2,000 entries
- **Python and TypeScript SDKs**: Approximately 97 million monthly downloads

## Governance

MCP is governed through the Agentic AI Foundation under the Linux Foundation. Organization includes Working Groups (Transports, Auth, Registry, and others) and Interest Groups, with changes proposed through Specification Enhancement Proposals (SEPs).

## 2026 Roadmap

Four priority areas:

- **Transport evolution**: Stateless Streamable HTTP across multiple server instances, session migration during scale-out, MCP Server Cards standardization
- **Agent communication**: Expanded server-model collaboration, multi-step reasoning, coordination patterns
- **Enterprise readiness**: Structured audit trails/observability, SSO-integrated auth flows, gateway/proxy patterns, configuration portability
- **Governance maturation**: Contributor ladder, delegation of authority to Working Groups, standardized charter templates

## Pricing

Free and open-source. Governed by the Agentic AI Foundation under the Linux Foundation (vendor-neutral, community-governed standard).

## History

- **November 2024**: Anthropic open-sources MCP
- **March 2025**: Spec v2 launches with Streamable HTTP and OAuth 2.1; OpenAI announces full MCP support
- **April 2025**: Google DeepMind confirms MCP support for Gemini
- **June 2025**: MCP servers formalized as OAuth Resource Servers with Resource Indicators mandate
- **September 2025**: MCP Registry launches
- **November 2025**: Largest spec update (async tasks, sampling, elicitation, extensions system)
- **December 2025**: Anthropic donates MCP to the Agentic AI Foundation under the Linux Foundation; OpenAI and Block join as co-founders
- **January 2026**: MCP Apps launches as first official extension
- **March 2026**: 2026 roadmap published with enterprise readiness as top priority