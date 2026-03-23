## Overview

The HubSpot MCP server is the official integration from HubSpot, now in public beta, that securely connects MCP-compatible AI clients to HubSpot CRM data. It enables AI assistants to interact with CRM information through natural language.

## Server Types

HubSpot offers two MCP server implementations:

1. **Remote MCP Server**: Cloud-based bridge for authorized LLMs to access real-time CRM data
2. **Developer MCP Server**: CLI-based local server for HubSpot Developer Platform interaction

## Features

- **CRM Object Access**: Read contacts, companies, deals, tickets, carts, products, orders, line items, invoices, quotes, subscriptions
- **Natural Language Interface**: Query CRM data conversationally
- **Real-Time Data**: Access current CRM information
- **Secure Authentication**: Private app access token based security
- **Read-Only Mode**: Currently supports read operations (public beta)
- **Easy Configuration**: NPM package with simple JSON configuration

## Supported CRM Objects

- Contacts and Companies
- Deals and Pipelines
- Tickets and Support Cases
- E-commerce: Carts, Products, Orders, Line Items
- Financial: Invoices, Quotes, Subscriptions

## Use Cases

- AI-assisted CRM data analysis
- Account research and enrichment
- Sales pipeline insights
- Customer support automation
- CRM data quality checks
- Competitive intelligence gathering
- Automated reporting and analytics

## Integration

Compatible with AI clients including Cursor, Claude Desktop, and other MCP-enabled applications.

## Setup

Available as NPM package with configuration via access token from HubSpot private app.

## Pricing

Free MCP server. HubSpot CRM pricing applies based on your subscription tier.