## Overview

A Model Context Protocol server implementation for RabbitMQ operation that wraps admin APIs of a RabbitMQ broker as MCP tools. Built by the Amazon MQ team, this server enables AI assistants to manage RabbitMQ message brokers through natural language commands.

## Features

- **Multi-Broker Support**: Connect to multiple RabbitMQ brokers within a single session
- **Queue Management**: Create, list, delete, and monitor queues
- **Exchange Management**: Manage exchanges and their configurations
- **Binding Operations**: Create and manage bindings between exchanges and queues
- **Message Operations**: Publish, consume, and inspect messages
- **Admin API Integration**: Full access to RabbitMQ admin API functionality
- **Cluster Management**: Manage multiple clusters simultaneously

## Capabilities

- List and inspect queues, exchanges, and bindings
- Create and configure message routing infrastructure
- Monitor queue depths and message rates
- Manage virtual hosts and permissions
- View cluster status and node health
- Execute administrative commands through natural language

## Use Cases

- Message broker infrastructure management
- Queue monitoring and troubleshooting
- Automated message routing configuration
- Integration testing with message queues
- Operational tasks for message-driven architectures
- Multi-cluster RabbitMQ administration

## Integration Benefits

- Simplified broker management through AI assistants
- Natural language interface for complex RabbitMQ operations
- Multi-broker support reduces context switching
- Automated operational workflows
- Reduced learning curve for RabbitMQ administration

## Authentication

Supports RabbitMQ admin credentials and connection configurations for secure broker access.

## Compatibility

Works with RabbitMQ 3.x and any MCP-compatible AI assistant including Claude, Cursor, and Windsurf.

## Pricing

Open-source MCP server. Amazon MQ for RabbitMQ pricing applies for managed service usage.