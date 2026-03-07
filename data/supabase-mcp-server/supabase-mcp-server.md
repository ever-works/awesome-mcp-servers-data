## Overview

The Supabase MCP server connects Supabase projects to AI assistants like Cursor, Claude, and Windsurf using the Model Context Protocol. It standardizes how Large Language Models talk to Supabase, allowing them to perform tasks like managing tables, fetching config, and querying data.

## Key Features

- **Project Management**: Create and manage Supabase projects directly from AI tools
- **Database Design**: Design tables and generate migrations using natural language
- **Data Querying**: Query data and run reports using SQL through conversational commands
- **Branch Management**: Manage branches, configurations, and TypeScript types
- **Over 20 Tools**: Comprehensive toolset for database design, data querying, and project administration
- **Project Scoping**: Limit access to specific projects for enhanced security
- **Read-Only Mode**: Execute SQL as a read-only PostgreSQL user to prevent write operations
- **Branching Support**: Create development branches to test changes before merging to production

## Security Features (2026)

The server includes several important security capabilities:

**Project Scoping**: Scope your MCP server to a specific project, limiting access to only that project's resources and preventing LLMs from accessing data from other projects in your Supabase account.

**Read-Only Flag**: Set a `--read-only` flag on the CLI command to prevent write operations on databases by executing SQL as a read-only Postgres user.

**Safe Branching**: Use Supabase's branching feature to create a development branch for your database, allowing you to test changes in a safe environment before merging them to production.

## Authentication

By default, the hosted Supabase MCP server uses dynamic client registration to authenticate with your Supabase org, meaning you don't need to manually create a personal access token (PAT) or OAuth app to use the server.

## Supported AI Tools

- Cursor
- Claude (Claude Desktop and Claude Code)
- Windsurf
- Visual Studio Code (Copilot)
- Cline
- More tools expected as they adopt the MCP standard

## Use Cases

- Natural language database schema design
- AI-assisted query writing and optimization
- Database migration generation
- Project configuration management
- Data exploration and analysis
- Development branch testing
- TypeScript type generation

## Technical Details

- Built on PostgreSQL
- RESTful API via PostgREST
- Real-time subscriptions
- Row-level security
- Authentication and authorization
- Storage and file management

## Pricing

Free tier available. Paid plans based on Supabase project usage.