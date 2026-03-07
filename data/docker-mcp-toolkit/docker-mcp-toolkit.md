## Overview

Docker MCP Toolkit is a comprehensive platform providing 300+ verified MCP servers packaged as container images with versioning, provenance, and security updates. It includes an integrated management interface in Docker Desktop for effortless setup and AI agent connections.

## Key Components

**1. Docker MCP Catalog**
The Docker MCP Catalog is a curated collection of verified MCP servers, packaged as Docker images and distributed through Docker Hub. It provides 300+ verified servers packaged as container images with built-in versioning, provenance tracking, and security updates.

**2. Docker MCP Toolkit**
The Docker MCP Toolkit is a management interface integrated into Docker Desktop that lets you set up, manage, and run containerized MCP servers in profiles and connect them to AI agents.

**3. MCP Gateway**
Docker's open-source solution for orchestrating Model Context Protocol servers, managing configuration, credentials, and access control as a centralized proxy between clients and servers.

## Features

- **300+ Verified Servers**: Curated, containerized registry of MCP servers
- **Digital Signatures**: All images under mcp/ are built by Docker and digitally signed to verify source and integrity
- **Software Bill of Materials (SBOM)**: Full transparency with SBOM included in each image
- **Profile Management**: Organize servers into named collections with configurations for different projects or environments
- **Client Compatibility**: Connects to Docker AI Agent, Claude, Cursor, VS Code, Windsurf, continue.dev, and Goose
- **Container Isolation**: Each server runs as an isolated container for portability and consistency
- **Custom Catalogs**: Create focused collections for teams or organizations
- **One-Click Setup**: Integrated interface in Docker Desktop for easy configuration

## What is MCP?

Model Context Protocol (MCP) is an open protocol that standardizes how AI applications access external tools and data sources, connecting LLMs to local development tools, databases, APIs, and other resources to extend their capabilities beyond their base training.

## MCP Gateway Architecture

The MCP Gateway manages the server's entire lifecycle:

1. AI application sends request to Gateway
2. Gateway identifies which server handles the tool
3. If server isn't running, Gateway starts it as a Docker container
4. Gateway injects required credentials
5. Applies security restrictions
6. Forwards request to server
7. Returns results to AI application

## Security Features

**Containerized Isolation**: Docker standardizes development, packaging, and distribution of applications. By packaging MCP servers as containers, Docker eliminates issues related to isolation and environment differences.

**Restricted Privileges**: MCP Gateway runs servers in isolated Docker containers with restricted privileges, network access, and resource usage.

**Built-in Logging**: Full visibility and governance of AI tool activity through logging and call-tracing capabilities.

**Secrets Management**: Secure credential injection and management.

## Benefits

**Eliminates Runtime Complexity**: No dependency conflicts or environment setup issues

**Solves N×N Integration Problem**: Centralized gateway eliminates need to connect each client to each server individually

**Easy Client Integration**: Connect instantly to clients with one-click setup

**Consistent Environments**: Containers ensure servers run identically everywhere

## Custom Catalogs

Custom catalogs let you curate focused collections of servers for your team or organization:

- Define exactly which servers are available
- Control versioning and updates
- Maintain organizational standards
- Share across teams

Instead of exposing all 300+ servers, organizations can create targeted catalogs for specific use cases.

## Supported AI Clients

- Docker AI Agent
- Claude (Claude Desktop and Claude Code)
- Cursor
- Visual Studio Code with Copilot
- Windsurf
- continue.dev
- Goose
- Other MCP-compatible clients

## Use Cases

- **Development Environments**: Consistent tooling across development teams
- **CI/CD Integration**: Automated testing and deployment with AI assistance
- **Multi-Project Management**: Different server profiles for different projects
- **Enterprise Governance**: Centralized control over available tools and services
- **Team Collaboration**: Shared configurations and server collections

## Getting Started

1. Install Docker Desktop
2. Access MCP Toolkit in Docker Desktop
3. Browse Docker MCP Catalog
4. Select servers for your profile
5. Configure and launch
6. Connect to AI client

## Docker Hub Integration

Explore the full catalog at Docker Hub's MCP section (hub.docker.com/mcp) with filtering, search, and version management.

## Pricing

Docker Desktop subscription required. Pricing based on Docker plan tier. Individual MCP servers may have their own pricing models.