## Overview

DBHub is a zero-dependency, token-efficient MCP server implementing the Model Context Protocol interface. This lightweight gateway allows MCP-compatible clients to connect to and explore different databases through a single interface with just two tools, maximizing the available context window for AI operations.

## Supported Databases

- **PostgreSQL**: Full support for PostgreSQL databases
- **MySQL**: MySQL server integration
- **MariaDB**: MariaDB compatibility
- **SQL Server**: Microsoft SQL Server support
- **SQLite**: Embedded database access

## Features

### Two-Tool Design
- **Maximum Efficiency**: Just 2 MCP tools for all database operations
- **Token Optimization**: Minimal token usage preserves context window
- **Unified Interface**: Same tools work across all database types
- **Zero Dependencies**: Lightweight with no external dependencies

### Multi-Database Support
- Connect to multiple database types simultaneously
- Switch between databases seamlessly
- Consistent query interface regardless of backend
- Automatic schema discovery

### Database Operations
- Execute SELECT queries
- Explore database schemas
- View table structures and relationships
- Inspect column types and constraints

## Use Cases

### Local Development
- Query development databases quickly
- Explore database schemas conversationally
- Test SQL queries with AI assistance
- Debug database issues

### Multi-Database Projects
- Manage projects using different databases
- Compare data across database types
- Migrate between database platforms
- Learn different SQL dialects

### Data Exploration
- Discover what data exists in databases
- Understand table relationships
- Query data without writing SQL
- Generate insights from database content

### Schema Analysis
- Document database structures
- Find tables and columns
- Understand foreign key relationships
- Analyze database design

## Token Efficiency

DBHub's two-tool design is specifically optimized to:
- Minimize tool definition tokens
- Preserve context window for data
- Reduce API costs
- Improve response quality

This is crucial for AI applications where context window is limited and expensive.

## Security

- Local deployment only (no cloud connections)
- Direct database connections
- No data transmission to third parties
- Standard database authentication

## Integration

Works with AI assistants supporting MCP like Claude and Cursor. Requires database connection strings for the databases you want to access. Runs locally on your machine.

## Pricing

Free and open-source. Works with your existing database installations.