## Overview

The HubSpot MCP server securely connects MCP-compatible AI clients to your HubSpot CRM data. MCP (Model Context Protocol) is a standardized way for agents built with Large Language Models to securely request and receive specific information from external systems like HubSpot.

## Dual Server Types

**1. HubSpot MCP Server (Remote)**
MCP-compatible AI clients can fetch relevant, real-time CRM data (contacts, companies, deals) in a controlled and secure manner.

**2. Developer MCP Server (Local)**
CLI-based server enabling agentic development software to interact with the HubSpot Developer Platform for project scaffolding and management.

## Key Features

- **Read-Only CRM Access**: Secure access to 11 CRM object types
- **Natural Language Queries**: Interact with CRM data conversationally
- **Vector Storage**: Built-in caching to overcome HubSpot API limitations
- **10-Minute Setup**: Quick installation and configuration
- **Real-Time Data**: Live CRM data access
- **Property Access**: Complete access to object property data
- **API Bridge**: No need to understand complex API structures

## Supported CRM Objects

The HubSpot remote MCP server currently supports read-only access to:

- Contacts
- Companies
- Deals
- Tickets
- Carts
- Products
- Orders
- Line Items
- Invoices
- Quotes
- Subscriptions

## Use Cases

**Marketing:**
- Automated lead scoring
- Contact enrichment
- Campaign performance analysis
- Segmentation automation
- Email automation insights

**Sales:**
- Deal pipeline analysis
- Meeting preparation
- Contact research
- Revenue forecasting
- Opportunity tracking

**Service:**
- Ticket triage
- Customer history lookup
- Support analytics
- SLA monitoring
- Customer satisfaction tracking

## Quick Setup

Setup takes under 10 minutes:

1. Install npm package
2. Create HubSpot private app token
3. Configure Claude Desktop or Claude Code
4. Start querying CRM data immediately

## Vector Storage & Caching

Built-in features to improve performance:

- Vector storage for semantic search
- Intelligent caching mechanisms
- Overcome HubSpot API rate limitations
- Improved response times
- Reduced API calls

## Natural Language Interactions

"Show me all contacts from California with deals over $10,000"
"List open tickets assigned to the support team"
"Find companies in the technology sector"
"What deals are closing this month?"
"Show me products with low inventory"

## Authentication

- HubSpot private app tokens
- Secure OAuth flow
- Token-based access
- Permission scoping
- API key management

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Custom MCP implementations

## API Integration

Bridges to HubSpot APIs:

- CRM API
- Contacts API
- Companies API
- Deals API
- Tickets API
- Products API
- Marketing API

## Current Status

Publicly Available in Beta - Active development with ongoing improvements.

## Pricing

Free MCP server. HubSpot subscription pricing applies based on tier and features used.