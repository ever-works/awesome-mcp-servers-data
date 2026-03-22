## Overview

The Apache Airflow MCP Server acts as a bridge between AI assistants and Apache Airflow instances by wrapping Apache Airflow's REST API. This MCP server leverages the Model Context Protocol to transform Apache Airflow REST API operations into natural language tools, supporting both Airflow API v1 (2.x) and v2 (3.0+).

## Features

- **45 Tools for API v2**: Comprehensive toolset for Airflow 3.0+
- **43 Tools for API v1**: Full support for Airflow 2.x
- **Dynamic Version Selection**: Automatic API version detection via environment variable
- **DAG Management**: Schedule, trigger, pause, and unpause DAGs
- **Workflow Monitoring**: Query DAG run states and task statuses
- **Natural Language Operations**: Manage Airflow through conversational AI
- **Programmatic Access**: Standardized MCP interface for AI agents

## Key Capabilities

- Schedule and trigger Airflow workflows programmatically
- Monitor DAG runs and task executions
- Manage DAG lifecycle (pause, unpause, update)
- Query workflow states and failures
- Proactive monitoring and alerting
- Automated workflow management
- Complex pipeline lifecycle handling

## Use Cases

- AI-assisted workflow scheduling
- Automated DAG management
- Proactive pipeline monitoring
- Natural language workflow operations
- Failure detection and alerting
- Pipeline optimization assistance
- Reduced manual intervention in orchestration

## Platform Integration

Apache Airflow is a Python-based platform for running directed acyclic graphs (DAGs) of tasks, providing:
- Programmatic workflow authoring
- Scheduling and execution
- Rich UI for monitoring
- Extensible architecture
- Enterprise-scale orchestration

## Integration Benefits

- Natural language Airflow management
- Reduced context switching
- AI-powered troubleshooting
- Automated operational tasks
- Faster incident response
- Simplified DAG management

## Docker Support

Available as Docker image: acuvity/mcp-server-apache-airflow

## Compatibility

Works with Claude, Cursor, Windsurf, and any MCP-compatible AI assistant. Supports Airflow 2.x and 3.0+.

## Pricing

Open-source Apache Airflow. Managed services available through cloud providers.