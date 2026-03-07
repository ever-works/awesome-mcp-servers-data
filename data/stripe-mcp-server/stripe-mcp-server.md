## Overview

The Stripe Model Context Protocol (MCP) server provides a set of tools that AI agents can use to interact with the Stripe API and search the knowledge base (including documentation and support articles). It dramatically simplifies the integration of payment functionality into applications through natural language instructions.

## Key Features

- **23 Comprehensive Tools**: Complete payment and customer management capabilities
- **Customer Management**: Create, list, and manage customer records
- **Product Operations**: Create and manage products with descriptions
- **Payment Processing**: Handle payments, refunds, and transactions
- **Account Information**: Access Stripe account details and settings
- **Knowledge Base Search**: Search Stripe documentation and support articles
- **OAuth Authentication**: Uses OAuth Dynamic Client Registration per MCP spec
- **Remote Server**: Hosted at https://mcp.stripe.com via Streamable HTTP
- **Restricted API Keys**: Support for limited-scope API keys for enhanced security

## Available Tools

Key tools organized by category:

**Customer Management:**
- create_customer: Create new customers with name and email
- list_customers: Retrieve customer lists with filtering options
- update_customer: Modify existing customer information
- delete_customer: Remove customer records

**Product & Pricing:**
- create_product: Create new products with descriptions
- list_products: Browse product catalog
- create_price: Set up pricing for products
- list_prices: View all pricing configurations

**Payment Operations:**
- create_payment_intent: Initialize payment flows
- capture_payment: Complete authorized payments
- create_refund: Process refunds
- list_charges: View transaction history

**Account & Settings:**
- get_stripe_account_info: Access account information
- get_balance: Check account balance

## Platform Support

**Claude**: Install the Stripe connector for Claude to access Stripe skills

**Claude Code**: Install via `claude /plugin install stripe@claude-plugins-official`

**Cursor**: Install the Stripe plugin for Cursor to access Stripe skills

Compatible with other MCP clients supporting remote servers.

## Remote Server Access

Stripe hosts a Streamable HTTP MCP server at https://mcp.stripe.com. The server uses OAuth Dynamic Client Registration to connect MCP clients according to the MCP specification.

For agentic software, you can pass a Stripe API key as a bearer token to the MCP remote server. Stripe strongly recommends using restricted API keys to limit access to only the functionality your agent requires.

## Monetization Features

The collaboration between Stripe and Cloudflare brings together payment processing expertise and edge computing infrastructure to create a toolkit that makes it easy to implement paid tools and services that AI assistants can access.

## Use Cases

- E-commerce payment processing
- Subscription billing management
- Invoice generation and tracking
- Customer account management
- Refund processing
- Payment analytics and reporting
- Marketplace payment distribution
- Recurring billing automation

## Security

- OAuth 2.1 authentication
- Restricted API keys for granular permissions
- PCI DSS compliance
- Webhook signature verification
- Audit logging

## Pricing

Stripe transaction fees apply based on your Stripe pricing plan. MCP server access is included.