## Overview

An MCP server connected to Elasticsearch unlocks a powerful real-time retrieval architecture where AI agents can explore, query, and analyze Elasticsearch data on demand. The official Elasticsearch MCP server implementation enables connecting agents to your Elasticsearch data through natural language conversations.

## Key Features

- **List Indices**: Retrieve all available Elasticsearch indices with health status and document counts
- **Get Mappings**: Fetch field mappings for indices to understand data structure
- **Execute Searches**: Run Elasticsearch searches using Query DSL
- **Automatic Highlighting**: Text field highlighting in search results
- **Natural Language Interface**: Query data conversationally instead of complex Query DSL
- **Real-Time Retrieval**: Access current data from Elasticsearch in real-time
- **Multi-Index Search**: Query across multiple indices simultaneously
- **Aggregations**: Perform analytical aggregations on data

## Available MCP Servers

**1. Official Elastic MCP Server** (elasticsearch 9.2+)
For Elasticsearch 9.2+ and Serverless, the Agent Builder MCP server is recommended, offering:
- Full access to built-in tools
- Custom tool creation
- Comprehensive feature set

**2. elastic/mcp-server-elasticsearch** (Earlier versions)
For Elasticsearch versions before 9.2 without Agent Builder:
- Connects agents to Elasticsearch data
- Natural language conversations
- More limited tool set than Agent Builder

**3. Community Implementations**
- cr7258/elasticsearch-mcp-server: Elasticsearch and OpenSearch support
- da1y/mcp-server-elasticsearch: Alternative implementation

## Core Tools

**list_indices**
Retrieves all available Elasticsearch indices.

Response includes:
- Index name
- Health status (green, yellow, red)
- Document count
- Primary shards
- Replica shards
- Storage size

**get_mappings**
Fetches field mappings for specified indices.

Provides:
- Field names
- Field types
- Field properties
- Nested structure
- Analyzer information

**search**
Executes Elasticsearch searches using Query DSL.

Supports:
- Full-text queries
- Term queries
- Boolean queries
- Range queries
- Aggregations
- Sorting
- Pagination
- Automatic text highlighting

## Query DSL Support

Full Elasticsearch Query DSL capabilities:

**Match Queries:**
```json
{
  "query": {
    "match": {
      "title": "search query"
    }
  }
}
```

**Boolean Queries:**
```json
{
  "query": {
    "bool": {
      "must": [{"match": {"status": "active"}}],
      "filter": [{"range": {"date": {"gte": "2026-01-01"}}}]
    }
  }
}
```

**Aggregations:**
```json
{
  "aggs": {
    "categories": {
      "terms": {"field": "category"}
    }
  }
}
```

## Use Cases

**Log Analysis:**
- Search application logs
- Identify error patterns
- Track system metrics
- Troubleshoot issues

**Document Search:**
- Full-text search across documents
- Semantic search
- Content discovery
- Knowledge base queries

**Data Analytics:**
- Aggregate metrics
- Generate reports
- Trend analysis
- Business intelligence

**E-commerce:**
- Product search
- Inventory management
- Customer behavior analysis
- Recommendation engines

**Security:**
- SIEM (Security Information and Event Management)
- Threat detection
- Audit log analysis
- Compliance monitoring

## Natural Language Examples

"Search for all documents about machine learning"
"Show me error logs from the last 24 hours"
"Find products in the electronics category"
"List all indices in the cluster"
"What's the mapping for the users index?"
"Show documents where status is active and created after 2026-01-01"

## Enhanced Search with AI

Model Context Protocol enhances Elasticsearch interaction by:

- Enabling natural language queries
- Eliminating complex Query DSL knowledge requirement
- Bridging AI capabilities with search data
- Providing conversational data access
- Simplifying complex query construction

## Text Highlighting

Automatic highlighting shows where search terms appear:

- Highlights matched terms in results
- Customizable highlight tags
- Multiple field highlighting
- Fragment sizing
- Pre/post tags configuration

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Custom MCP implementations

## OpenSearch Support

Some implementations (like cr7258/elasticsearch-mcp-server) also support OpenSearch:

- Compatible API
- Similar query capabilities
- Shared features
- Migration path

## Configuration

Typical configuration:

- **Host**: Elasticsearch endpoint URL
- **Port**: API port (default 9200)
- **Authentication**: Username/password or API key
- **TLS/SSL**: Encrypted connections
- **Cloud ID**: For Elastic Cloud deployments
- **API Key**: Token-based authentication

## Security

- Basic authentication
- API key authentication
- Role-based access control (RBAC)
- TLS/SSL encryption
- IP filtering
- Field-level security
- Document-level security

## Performance Considerations

- Use filters for exact matches (faster than queries)
- Limit result size with pagination
- Use field filters to reduce payload
- Cache frequently used queries
- Optimize index mappings
- Use appropriate shard count

## Deployment Options

**Self-Hosted:**
- Full control over configuration
- Custom hardware optimization
- On-premises deployment

**Elastic Cloud:**
- Fully managed service
- Automatic scaling
- Built-in monitoring
- Multi-region deployment

**Cloud Providers:**
- AWS Elasticsearch Service
- Azure Elasticsearch
- Google Cloud Elasticsearch

## Monitoring & Observability

- Cluster health monitoring
- Query performance metrics
- Index statistics
- Node resource usage
- Search latency tracking

## Integration Patterns

**Search-First Pattern:**
1. AI receives user query
2. Convert to Elasticsearch query
3. Execute search
4. Return formatted results

**RAG Pattern:**
1. Search for relevant documents
2. Extract content
3. Provide as context to LLM
4. Generate informed response

## Pricing

Varies by deployment:

- **Open Source**: Free (self-hosted)
- **Elastic Cloud**: Based on memory, storage, and features
- **Cloud Providers**: Per-instance pricing
- **MCP Server**: Free and open-source implementations