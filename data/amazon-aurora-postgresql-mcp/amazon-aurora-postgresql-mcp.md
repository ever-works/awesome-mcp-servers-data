## Overview

Amazon Aurora PostgreSQL MCP is an AWS-optimized Model Context Protocol server designed specifically for Amazon Aurora PostgreSQL databases. It provides natural language query capabilities, schema inspection, and seamless integration with AWS RDS PostgreSQL-compatible databases including Aurora Serverless.

## Features

- **Aurora Optimization**: Optimized for Amazon Aurora PostgreSQL
- **Natural Language Queries**: Convert conversational queries to SQL
- **Schema Discovery**: Automatic database schema inspection
- **Query Execution**: Direct SQL query execution
- **Read-Only Mode**: Safe read-only access option
- **AWS Integration**: Native AWS credentials and IAM support
- **Connection Pooling**: Efficient connection management
- **Multi-Database**: Support for multiple Aurora instances

## Aurora-Specific Features

- **Serverless v2 Support**: Connect to Aurora Serverless databases
- **Global Database**: Query global Aurora clusters
- **Read Replicas**: Distribute reads across replicas
- **Fast Cloning**: Work with Aurora fast clones
- **Backtrack**: Query point-in-time data (where available)
- **Performance Insights**: Integration with Aurora monitoring
- **Auto-scaling**: Works with Aurora auto-scaling

## Query Capabilities

- Natural language to SQL conversion
- Complex JOIN operations
- Aggregate functions
- Subqueries and CTEs
- Full-text search
- JSON/JSONB queries
- Array operations
- Window functions

## Schema Operations

- List all databases
- Inspect table structures
- View column types and constraints
- Explore relationships and foreign keys
- Index information
- View definitions
- Function and procedure listings

## AWS Integration

- IAM database authentication
- AWS Secrets Manager integration
- VPC endpoint support
- CloudWatch logging
- AWS Systems Manager Parameter Store
- RDS proxy support
- Multi-AZ deployment awareness

## Security Features

- Read-only mode for safety
- IAM role-based access
- SSL/TLS encryption
- Secrets Manager credential rotation
- VPC isolation
- Security group integration
- Query logging and auditing

## Use Cases

- Query Aurora databases through natural language
- Build AI-powered database tools
- Automate database reporting
- Explore database schemas conversationally
- Generate insights from Aurora data
- Create database documentation
- Perform ad-hoc data analysis

## Connection Options

- Direct connection string
- AWS Secrets Manager secret ARN
- Systems Manager parameter
- Environment variables
- IAM authentication
- RDS Proxy endpoint

## Performance

- Connection pooling for efficiency
- Query result caching
- Pagination for large result sets
- Timeout configuration
- Read replica routing

## Pricing

Free and open-source from AWS Labs. Aurora database usage follows AWS pricing:
- **Aurora Serverless v2**: ACU-based pricing
- **Aurora Provisioned**: Instance-based pricing
- **I/O Operations**: Pay per request
- **Storage**: Per GB-month pricing