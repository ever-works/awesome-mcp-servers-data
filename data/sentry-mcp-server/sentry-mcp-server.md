## Overview

The Sentry MCP Server provides comprehensive error monitoring and AI observability for Model Context Protocol implementations. It serves two main purposes: enabling LLM clients to interact with Sentry for error analysis, and monitoring your own MCP servers in production.

## Dual Functionality

**1. Sentry as an MCP Server**
Connects your LLM client to Sentry using the Model Context Protocol, giving your AI tools direct access to issues, errors, projects, and Seer AI-powered analysis.

**2. Monitoring Your MCP Servers**
Monitor your own MCP server implementations using Sentry for errors, traces, and logs with automatic instrumentation and observability.

## Key Features for Error Analysis

- **Error Search**: Search errors across files and projects
- **Issue Investigation**: Detailed analysis of specific issues
- **Seer Integration**: AI-powered root cause analysis
- **Release Management**: Track errors across releases
- **Performance Monitoring**: Monitor application performance
- **Custom Queries**: Advanced filtering and search capabilities
- **Project Access**: Multi-project error tracking
- **Team Collaboration**: Share insights across teams

## Production Monitoring (Launched August 2025)

Sentry's MCP Server Monitoring gives anyone building on MCP a clearer view into what's working (and what's not) behind the scenes. With just a few lines of code, teams can answer:

- Which clients are experiencing errors?
- Which tools are getting called the most?
- Which tools are slow or failing?
- Which inputs are causing breakage?
- Are clients using outdated transports?
- What's the traffic load on MCP servers?

## What Gets Monitored

Sentry automatically collects information about:

- MCP server connections
- Resource access patterns
- Tool execution metrics
- Error rates and types
- Performance metrics
- Client usage analytics
- Transport protocol versions

## Continuous AI for Error Monitoring

The Sentry Mission Control Integration enables Continuous AI where AI agents autonomously detect, analyze, and fix production errors:

1. Sentry detects an issue
2. AI agent automatically analyzes the error
3. Agent generates a fix
4. Creates pull request automatically
5. Validates the solution
6. No manual intervention required

## Integration Setup

**JavaScript/TypeScript:**
Integrates with MCP JavaScript SDK, automatically instrumenting tools, prompts, and resources.

**Python:**
Connects with MCP Python SDK, supporting both:
- High-level FastMCP API
- Low-level mcp.server.lowlevel.Server API

Both implementations provide automatic instrumentation of tools, prompts, and resources.

## Deployment Options

**Hosted Service:**
- Available at https://mcp.sentry.dev
- OAuth authentication included
- Nothing to install
- Fully managed by Sentry

**Self-Hosted:**
- Available via GitHub (github.com/getsentry/sentry-mcp)
- Full control over deployment
- Custom configuration options

## Observability Features

**Real-Time Alerts:**
- Immediate notification of errors
- Threshold-based alerting
- Custom alert rules

**Distributed Tracing:**
- Full request/response tracing
- Performance bottleneck identification
- Cross-service visibility

**Error Grouping:**
- Intelligent error aggregation
- Fingerprinting for duplicate detection
- Stack trace analysis

**Performance Insights:**
- Response time tracking
- Throughput metrics
- Resource utilization

## Seer AI-Powered Analysis

Seer provides:

- Automatic root cause identification
- Pattern recognition across errors
- Suggested fixes based on similar issues
- Impact analysis
- Trend detection

## Use Cases

- **Production Debugging**: Investigate and fix errors in real-time
- **MCP Server Monitoring**: Track health of your MCP implementations
- **Performance Optimization**: Identify and resolve bottlenecks
- **Client Analytics**: Understand how AI clients use your servers
- **Autonomous Error Resolution**: Let AI agents fix issues automatically
- **Release Validation**: Monitor errors across deployments
- **Team Collaboration**: Share error insights and solutions

## Security

- OAuth 2.0 authentication
- Project-level access controls
- API key management
- Audit logging
- PII data scrubbing
- GDPR compliance

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Custom MCP implementations

## Why Monitor MCP Servers?

"MCP is the fastest-growing protocol of the AI era, but when an MCP server breaks it can be tough to figure out what went wrong," says Sentry CEO Milin Desai.

Development teams needed visibility into:
- Traffic load and AI client usage
- Which tools are called most frequently
- Tool performance and failure rates
- Input patterns causing errors
- Client version adoption

All of this without relying on users to report issues.

## Dashboard & Analytics

- Visual error trends
- Performance graphs
- Client usage statistics
- Tool execution metrics
- Custom dashboards
- Export capabilities

## Pricing

Sentry subscription required. Pricing based on event volume and features. Free tier available for development.