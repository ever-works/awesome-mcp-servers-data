## Overview

The Azure MCP Server enables AI-powered development tools to interact with Azure cloud services through the Model Context Protocol. Azure offers many cloud services for building robust applications, and the Azure MCP Server exposes these powerful services for agentic usage, allowing AI systems to perform operations that are context-aware of your Azure resources.

## Key Features

- **MCP Protocol Implementation**: Compatible with MCP clients like GitHub Copilot, OpenAI Agents SDK, Semantic Kernel
- **Entra ID Authentication**: Azure Identity library integration following best practices
- **Azure Services Support**: Broad coverage of Azure resources and operations
- **CLI Integration**: Azure CLI and Azure Developer CLI (azd) support
- **Multi-Language**: Python and .NET SDK support
- **VS Code Extension**: Integrated development experience
- **Resource Management**: Query, create, update Azure resources
- **Data Access**: Read files from Storage, query databases, analyze logs

## Supported Azure Services

**Compute:**
- Azure Virtual Machines
- Azure Kubernetes Service (AKS)
- Azure Container Instances
- Azure Functions
- Azure App Service

**Data & Storage:**
- Azure Cosmos DB
- Azure SQL Database
- Azure Blob Storage
- Azure Table Storage
- Azure Queue Storage
- Azure Data Lake

**Analytics:**
- Azure Log Analytics
- Azure Monitor
- Application Insights
- Azure Data Explorer

**Networking:**
- Virtual Networks
- Load Balancers
- Application Gateway
- Azure DNS
- Traffic Manager

**Security:**
- Azure Key Vault
- Azure Active Directory
- Azure Security Center
- Microsoft Sentinel

## Use Cases

**Database Operations:**
- Query Azure Cosmos DB using natural language
- Execute SQL queries on Azure SQL Database
- Retrieve documents from NoSQL collections
- Perform data aggregations

**Storage Management:**
- Read files from Azure Storage
- Upload and download blobs
- List storage containers
- Manage file shares

**Log Analysis:**
- Query logs in Log Analytics workspace
- Run KQL (Kusto Query Language) queries
- Analyze application insights
- Troubleshoot issues from logs

**Resource Management:**
- List Azure storage accounts
- Get resource group information
- Monitor resource health
- Manage resource tags

## GitHub Copilot Integration

Developers can use GitHub Copilot agent mode with the Azure MCP Server to:

- List Azure storage accounts conversationally
- Run KQL queries on Azure databases
- Access Azure resources from IDE
- Deploy applications to Azure
- Monitor application performance

## Authentication

**Entra ID (Azure AD):**
- DefaultAzureCredential for seamless auth
- Managed Identity support
- Service Principal authentication
- Interactive browser login
- Device code flow
- Azure CLI credential

**Best Practices:**
- Follows Azure authentication patterns
- Secure credential management
- Token caching
- Automatic token refresh

## Azure CLI Integration

**Azure CLI:**
- Run az commands via MCP
- Resource provisioning
- Configuration management
- Script execution

**Azure Developer CLI (azd):**
- Initialize projects
- Deploy applications
- Manage environments
- Provision infrastructure

## Tools Available

**Azure Cloud Architect:**
- Design cloud solutions
- Best practice recommendations
- Architecture validation
- Cost optimization suggestions

**Azure Redis Tools:**
- Cache management
- Connection configuration
- Performance monitoring
- Data operations

**Resource Management Tools:**
- CRUD operations on resources
- Resource group management
- Subscription operations
- Tag management

## Natural Language Examples

"List all storage accounts in my Azure subscription"
"Query the application logs from the last 24 hours"
"Show me the contents of container 'data' in storage account 'mystore'"
"Run a KQL query on my Log Analytics workspace"
"Deploy this application to Azure App Service"

## Compatible MCP Clients

- GitHub Copilot (agent mode)
- VS Code with Azure extension
- OpenAI Agents SDK
- Semantic Kernel
- Claude Desktop
- Claude Code
- Cursor
- Custom MCP implementations

## Development Languages

**Python:**
- Azure SDK for Python
- FastAPI for MCP server
- Type hints and async support

**.NET:**
- Azure SDK for .NET
- C# implementation
- ASP.NET Core integration

## VS Code Extension

Available from Visual Studio Marketplace:

- Integrated Azure resource explorer
- IntelliSense for Azure APIs
- Authentication helpers
- Debug support
- Configuration management

## KQL (Kusto Query Language) Support

Query Azure logs and data:

```kql
AppRequests
| where TimeGenerated > ago(24h)
| summarize count() by ResultCode
```

- Log Analytics queries
- Application Insights queries
- Azure Data Explorer
- Advanced analytics

## Security Best Practices

- Use Managed Identities when possible
- Implement least privilege access
- Enable Azure AD authentication
- Use Key Vault for secrets
- Enable audit logging
- Follow Azure Well-Architected Framework

## Resource Provisioning

- ARM templates deployment
- Bicep file execution
- Terraform integration
- Azure Resource Manager API
- Infrastructure as Code

## Monitoring & Observability

- Application Insights integration
- Azure Monitor metrics
- Log Analytics queries
- Performance tracking
- Error monitoring
- Custom telemetry

## Cost Management

- Resource cost analysis
- Budget alerts
- Cost optimization recommendations
- Resource right-sizing
- Reserved instance analysis

## High Availability

- Multi-region deployment
- Availability zones
- Load balancing
- Traffic management
- Disaster recovery

## Compliance

- Azure Policy enforcement
- Regulatory compliance
- Security standards
- Data residency
- Compliance reporting

## Performance Optimization

- Caching strategies
- CDN integration
- Auto-scaling configuration
- Performance monitoring
- Query optimization

## Pricing

Free and open-source MCP server. Azure service pricing applies based on:

- Resource usage
- Data transfer
- API calls
- Storage consumption
- Compute hours

Azure free tier includes 12 months of free services and always-free services.