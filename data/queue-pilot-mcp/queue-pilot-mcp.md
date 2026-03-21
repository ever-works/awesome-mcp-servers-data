## Overview

Queue Pilot is an MCP server for message queue development that combines message inspection with JSON Schema validation. Designed for integration projects where multiple teams communicate via message brokers, it supports both RabbitMQ and Apache Kafka through a unified interface.

## Features

### Multi-Broker Support
- **RabbitMQ Integration**: Full support for RabbitMQ queues, exchanges, and bindings
- **Apache Kafka Integration**: Kafka topics, consumer groups, partitions, and offsets
- **Unified Interface**: Same tools work for both brokers where applicable
- **Broker-Specific Tools**: Specialized tools for platform-specific features

### Core Capabilities
- **Message Inspection**: View and analyze messages from queues and topics
- **JSON Schema Validation**: Validate message payloads against agreed-upon schemas
- **Queue Management**: List queues/topics and monitor their status
- **Message Publishing**: Send test messages to queues or topics

### Kafka-Specific Tools
- `list_consumer_groups`: View all consumer groups
- `describe_consumer_group`: Get detailed consumer group information
- `list_partitions`: View topic partition details
- `get_offsets`: Check consumer offsets and lag

## Use Cases

### Team Collaboration
- Validate message contracts between teams
- Ensure payload compliance with API specifications
- Debug integration issues across services

### Development Workflow
- Inspect messages during local development
- Test message schemas before deployment
- Validate transformations and routing logic

### Multi-Platform Operations
- Manage both RabbitMQ and Kafka from one interface
- Standardize message validation across platforms
- Reduce context switching between broker tools

## Tools Available

Provides access to 14+ tools for:
- Inspecting queues and topics
- Validating message payloads
- Publishing test messages
- Managing consumer groups (Kafka)
- Monitoring partitions and offsets (Kafka)

## Integration

Works with AI assistants supporting MCP, enabling natural language interaction with your message infrastructure. Ideal for teams using microservices architectures with multiple messaging systems.

## Pricing

Free and open-source. Works with both self-hosted and cloud-managed RabbitMQ and Kafka instances.