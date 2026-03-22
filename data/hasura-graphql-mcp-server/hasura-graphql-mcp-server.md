## Overview

The Hasura GraphQL MCP server enables AI agents to interact with Hasura GraphQL endpoints, allowing them to discover API structure, execute queries and mutations, preview data, and perform aggregations - all based on natural language requests. It acts as a specialized MCP bridge to any Hasura GraphQL endpoint.

## Features

- **Schema Introspection**: Provides the full GraphQL schema definition via introspection
- **Query Execution**: Executes read-only GraphQL queries
- **Mutation Execution**: Executes GraphQL mutations for data modifications
- **Table Listing**: Lists available data tables managed by Hasura
- **Natural Language Interface**: Convert natural language requests into GraphQL operations
- **Data Aggregations**: Perform aggregations and analytics on data

## Tools Provided

1. **Hasura GraphQL Schema**: Full schema definition through introspection
2. **run_graphql_query**: Execute read-only queries
3. **run_graphql_mutation**: Execute mutations for data changes
4. **list_tables**: List available tables in the Hasura instance

## Technical Implementation

Node.js server built on the Model Context Protocol that acts as a bridge between AI assistants and Hasura GraphQL endpoints.

## Use Cases

- Discover and explore GraphQL API structure
- Execute queries to retrieve data conversationally
- Perform mutations to create or update data
- Analyze data with aggregations
- Build AI-powered applications with GraphQL backends

## Integration with PromptQL

Can leverage external MCP servers through Hasura's connector architecture, allowing:
- Integration of existing MCP tools into a unified data graph
- Consistent authorization policies across all tools
- Composition of data from different sources in a single query

## Supported Clients

Compatible with any MCP-enabled AI assistant including Claude, Cursor, Windsurf, and ChatGPT.

## Pricing

Open-source community implementation. Hasura Cloud pricing applies separately for GraphQL API hosting.