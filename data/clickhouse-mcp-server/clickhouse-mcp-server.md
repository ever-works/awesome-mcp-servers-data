## Overview

The ClickHouse MCP Server enables AI assistants to interact with ClickHouse analytics databases through the Model Context Protocol, providing comprehensive database management and query capabilities for the world's fastest analytical database.

## Features

- **Query execution**: Execute SQL queries on ClickHouse clusters with sub-second response times
- **Database listing**: Enumerate all databases on ClickHouse clusters
- **Table inspection**: List tables in databases with pagination support
- **Read-only mode**: Queries run in read-only mode by default for safety
- **Configurable write access**: Optional write access with additional safety controls
- **Destructive operation protection**: DROP, TRUNCATE, and other destructive operations require explicit opt-in
- **OAuth authentication**: Secure authentication via OAuth
- **Fully managed cloud**: No setup or maintenance required for ClickHouse Cloud deployments

## Safety Features

By default, queries run in read-only mode (`CLICKHOUSE_ALLOW_WRITE_ACCESS=false`). When write access is enabled, destructive operations including:

- DROP TABLE
- DROP DATABASE
- DROP VIEW
- DROP DICTIONARY
- TRUNCATE TABLE

require an additional opt-in flag for maximum safety.

## Deployment Options

Multiple implementations available:

- **Official clickhouse-mcp**: Main implementation from ClickHouse
- **Tinybird MCP Server**: Optimized for Tinybird deployments
- **Altinity MCP**: Enterprise-focused implementation
- **Remote MCP server**: Fully managed on ClickHouse Cloud with OAuth

## Why ClickHouse for AI Analytics

ClickHouse is built to be the world's fastest analytical database, where no bits, bytes, or milliseconds are wasted. This makes it particularly well-suited for AI-driven analytics workloads that may generate suboptimal queries, as ClickHouse can handle them efficiently.

## Use Cases

- Real-time analytics dashboards
- Log analysis and monitoring
- Time-series data analysis
- Business intelligence queries
- Data warehouse operations
- Event stream processing
- AI-driven data exploration

## Integration

Compatible with Claude Desktop, Cursor, Continue, Windsurf, and other MCP clients. Supports both local and cloud ClickHouse deployments.

## Technical Details

- Columnar storage for optimal query performance
- Distributed query execution
- Real-time data ingestion
- Compression for efficient storage
- Vectorized query execution

## Pricing

ClickHouse Cloud pricing applies. Free tier available for development and small-scale deployments. Open-source version free to use.