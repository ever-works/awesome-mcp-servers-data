## Overview

Docker MCP Compose enables you to compose, manage, and run multiple MCP servers as Docker containers with a unified API gateway built in. This tool provides Docker Compose-style configuration for Model Context Protocol servers with automatic protocol translation and monitoring capabilities.

## Features

- **Docker Compose-Style YAML**: Familiar configuration format
- **HTTP Proxy**: Automatic protocol translation (STDIO → HTTP)
- **Native Support**: Works with both Docker and Podman
- **Session Management**: Connection pooling and session handling
- **Built-in Dashboard**: Monitoring and management interface
- **OpenAPI Spec Generation**: Automatic API documentation
- **Unified Gateway**: Single entry point for multiple MCP servers
- **Container Isolation**: Each server runs in isolated container

## Key Capabilities

- Deploy multiple MCP servers simultaneously
- Manage MCP server lifecycle (start, stop, restart)
- Monitor server health and status
- Automatic HTTP endpoint generation
- Session persistence and management
- Container log access and debugging
- Network isolation and security

## Benefits for Local Development

- **Isolation**: Each server runs in its own container
- **Preconfigured Tools**: Ready-to-run servers with one click
- **Reproducibility**: Consistent behavior across environments
- **Security**: Sandboxed isolation prevents host damage
- **No Filesystem Access**: LLM can't access host unless explicitly bound

## Use Cases

- Local MCP server development and testing
- Multi-server application development
- Secure AI agent testing environments
- Microservice-based MCP architectures
- Team development with consistent setups
- CI/CD pipeline integration
- Production deployment preparation

## Docker MCP Toolkit Integration

Works with Docker's MCP Toolkit which provides:
- Hundreds of curated MCP servers
- Secure defaults and isolation
- Profile-based server management
- Integration with LLM-based clients

## Configuration Example

Uses YAML configuration for defining:
- Server images and versions
- Environment variables
- Port mappings
- Volume mounts
- Network configuration

## Integration Benefits

- Simplified multi-server management
- Consistent development environments
- Enhanced security through isolation
- Reduced setup complexity
- Automated deployment workflows

## Compatibility

Works with Docker and Podman container runtimes. Supports any containerized MCP server.

## Pricing

Open-source tool. Docker Desktop licensing applies for commercial use.