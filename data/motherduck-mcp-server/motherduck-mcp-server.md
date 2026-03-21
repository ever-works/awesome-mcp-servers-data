## Overview

Connect AI assistants to your data using DuckDB's powerful analytical SQL engine through the MotherDuck MCP Server. This server supports connecting to local DuckDB files, in-memory databases, S3-hosted databases, and MotherDuck cloud analytics platform. Runs in read-only mode by default for safety.

## Features

### Multiple Connection Types
- **Local DuckDB Files**: Query .duckdb files on your filesystem
- **In-Memory Databases**: Temporary analytical workloads
- **S3-Hosted Databases**: Query data directly from object storage
- **MotherDuck Cloud**: Connect to serverless DuckDB in the cloud

### Query Capabilities
- **Analytical SQL**: Full DuckDB SQL dialect support
- **Parquet Files**: Direct queries on columnar data
- **CSV/JSON**: Read structured and semi-structured data
- **External Tables**: Query data without importing

### Safety Features
- **Read-Only Default**: Prevents accidental data modification
- **Write Mode Available**: Add --read-write flag when needed
- **Transaction Support**: ACID guarantees for data integrity
- **Query Validation**: Syntax checking before execution

## DuckDB Capabilities

### Performance
- In-process analytical database
- Columnar storage for fast aggregations
- Parallel query execution
- Efficient compression

### Integrations
- Direct S3/GCS/Azure Blob queries
- Parquet, CSV, JSON support
- Arrow integration
- PostgreSQL wire protocol

### Advanced Features
- Window functions and CTEs
- Full-text search
- Geospatial queries (PostGIS extension)
- Machine learning extensions

## Use Cases

### Data Exploration
- Analyze CSV and Parquet files without importing
- Query S3 data lakes directly
- Perform ad-hoc analysis on local data
- Join data from multiple sources

### Business Intelligence
- Generate reports from analytical queries
- Calculate aggregations and metrics
- Analyze time-series data
- Create data visualizations

### Data Pipelines
- Transform data with SQL
- Validate data quality
- Test ETL transformations locally
- Debug data processing issues

### RAG Applications
- Vector similarity search with HNSW indexing
- Semantic search over embeddings
- Hybrid search combining text and vectors
- High-performance retrieval for AI applications

## MotherDuck Cloud Benefits

- Serverless DuckDB with zero infrastructure
- Share databases across team members
- Scale compute automatically
- Persistent storage in the cloud
- Collaborate on analytical workflows

## Integration

Works with Claude, Cursor, and other MCP-compatible AI tools. Requires DuckDB installed locally or MotherDuck account for cloud analytics.

## Pricing

DuckDB is free and open-source. MotherDuck offers free tier with generous limits and usage-based pricing for cloud analytics.