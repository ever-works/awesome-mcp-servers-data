## Overview

Queue Pilot is an MCP server that combines message inspection with JSON Schema validation and supports both RabbitMQ and Kafka. Designed for integration projects where multiple teams communicate via message brokers, it allows you to inspect queues/topics, view messages, and validate payloads against agreed-upon schemas from your AI assistant.

## Features

- **Dual Broker Support**: Unified interface for both RabbitMQ and Kafka
- **Message Inspection**: View and analyze messages in queues and topics
- **JSON Schema Validation**: Validate message payloads against schemas
- **Consumer Group Management**: Kafka-specific consumer group operations
- **Partition Management**: List and inspect Kafka partitions
- **Offset Operations**: Get and manage consumer offsets
- **Cross-Team Integration**: Designed for multi-team integration projects

## RabbitMQ Tools

- List queues and view queue details
- Inspect messages in queues
- Validate message payloads
- Monitor queue depths and consumers

## Kafka-Specific Tools

- list_consumer_groups: List all consumer groups
- describe_consumer_group: Get detailed group information
- list_partitions: List topic partitions
- get_offsets: Retrieve consumer offsets

## Technical Implementation

Kafka adapter uses the Confluent JavaScript client and supports SASL authentication.

## Use Cases

- Integration testing across teams
- Message payload validation
- Queue and topic monitoring
- Schema compliance verification
- Multi-broker message infrastructure management
- Debugging integration issues

## Integration Benefits

- Single interface for multiple broker types
- AI-assisted message debugging
- Automated schema validation
- Reduced context switching between broker tools
- Natural language message inspection

## Authentication

Supports connection credentials for both RabbitMQ and Kafka with SASL authentication for Kafka.

## Compatibility

Compatible with Claude, Cursor, Windsurf, and any MCP-enabled AI assistant.

## Pricing

Open-source implementation. Broker service costs apply separately.