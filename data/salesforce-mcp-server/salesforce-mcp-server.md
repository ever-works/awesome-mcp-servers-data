## Overview

Model Context Protocol (MCP) in Salesforce is an open-source protocol that makes it easier for AI apps and agents to connect with tools and data sources. MCP acts as a universal translator between AI agents and business data, similar to how USB created a standard way for devices to connect to computers.

## Salesforce Hosted MCP Servers

Salesforce Hosted Model Context Protocol Servers enable AI agents to securely access your Salesforce data and help teams across your entire organization. Organizations can expose specific Salesforce APIs and data as tools without writing a single line of code.

## Availability

- **Beta**: Currently available (as of 2026)
- **General Availability**: Targeted for February 2026
- **Agentforce Integration**: Pilot phase with July 2025 release

## Key Features

- **Read/Write CRM Access**: Access to Accounts, Contacts, Cases, Opportunities
- **Commerce Cloud Integration**: Products and orders management
- **Zero Code Configuration**: Expose APIs without custom development
- **Secure Access**: Enterprise-grade security and permissions
- **Agentforce Native Client**: Built-in MCP client for agents
- **Natural Language Queries**: Interact with Salesforce data conversationally
- **RBAC Compliance**: Respects all Salesforce permission models

## Agentforce MCP Support

Agentforce will include a native MCP client enabling agents to:

- Connect to any MCP-compliant server securely
- No custom code required
- Seamless integration with Salesforce workflows
- AI-powered automation across systems

## Core Capabilities

**CRM Objects:**
- Accounts: Company and organization records
- Contacts: Individual contact information
- Leads: Potential customer tracking
- Opportunities: Sales pipeline management
- Cases: Customer support tickets
- Tasks: Activity and task management
- Events: Calendar and meeting scheduling

**Commerce Cloud:**
- Product catalog management
- Order processing
- Inventory tracking
- Price books
- Shopping cart operations

**Data Operations:**
- Create records
- Read record details
- Update existing records
- Delete records (with permissions)
- Bulk operations
- Query using SOQL

## Natural Language Interactions

The MCP server enables Claude and other AI tools to:

- Query Salesforce data using everyday language
- Modify records conversationally
- Manage Salesforce objects
- Generate reports and insights
- Automate workflows

## Use Cases

**Sales Automation:**
- Automated lead qualification
- Opportunity updates
- Pipeline reporting
- Follow-up task creation
- Meeting scheduling

**Customer Support:**
- Case creation from emails/chats
- Automated case routing
- Knowledge base searches
- SLA tracking
- Escalation management

**Data Management:**
- Record updates from natural language
- Bulk data operations
- Data quality checks
- Duplicate detection
- Field validation

**Analytics & Reporting:**
- Custom report generation
- Dashboard insights
- Trend analysis
- Forecasting
- Performance metrics

## Security & Compliance

**Enterprise Security:**
- OAuth 2.0 authentication
- Role-based access control
- Field-level security
- Record-level security
- Sharing rules enforcement

**Data Protection:**
- Encryption at rest and in transit
- Audit logging
- Data residency compliance
- GDPR compliance
- HIPAA compliance (Health Cloud)

## Integration Patterns

**AI-Powered CRM:**
1. User asks about customer
2. AI queries Salesforce via MCP
3. Returns comprehensive customer view
4. Suggests next actions

**Automated Data Entry:**
1. AI processes email/message
2. Extracts relevant information
3. Creates/updates Salesforce records
4. Notifies team members

## Configuration

Hosted MCP Server setup:

1. Access Salesforce Setup
2. Navigate to MCP Servers
3. Select APIs/objects to expose
4. Configure permissions
5. Generate access credentials
6. Connect AI tools

## Supported Objects

**Standard Objects:**
- Account, Contact, Lead
- Opportunity, Case, Task
- Event, Campaign, Product
- PriceBook, Order, Contract

**Custom Objects:**
- Any custom object in your org
- Custom fields on standard objects
- Custom metadata
- Custom settings

## Query Capabilities

**SOQL Support:**
- SELECT queries
- WHERE conditions
- ORDER BY sorting
- LIMIT results
- Relationship queries
- Aggregate functions

**SOSL Search:**
- Full-text search
- Multi-object searches
- Relevance ranking
- Field-specific searches

## Compatible MCP Clients

- Agentforce (native support)
- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Custom MCP implementations

## Community Implementation

tsmztech/mcp-server-salesforce provides:

- Natural language Salesforce integration
- Query, modify, and manage objects
- Conversational CRM access
- Claude-optimized

## API Access

Exposed Salesforce APIs:

- REST API
- SOAP API
- Bulk API
- Streaming API
- Metadata API
- Tooling API

## Workflow Automation

- Trigger flows from MCP
- Execute Apex code
- Call external services
- Update records automatically
- Send notifications

## Einstein AI Integration

- Einstein Prediction Builder
- Einstein Discovery insights
- Einstein Next Best Action
- Einstein Bots integration

## Mobile Support

- Salesforce Mobile App integration
- Mobile-optimized workflows
- Offline capabilities
- Push notifications

## Customization

- Custom MCP tools
- Apex integration
- Lightning components
- Custom UI extensions
- Process Builder integration

## Performance

- API rate limits based on edition
- Bulk API for large operations
- Query optimization
- Caching strategies
- Asynchronous processing

## Monitoring & Analytics

- API usage tracking
- Error monitoring
- Performance metrics
- Audit trail
- Usage dashboards

## Pricing

Included with Salesforce subscription:

- **Essentials**: Starting at $25/user/month
- **Professional**: $75/user/month
- **Enterprise**: $150/user/month
- **Unlimited**: $300/user/month

MCP server access included; API limits vary by edition.