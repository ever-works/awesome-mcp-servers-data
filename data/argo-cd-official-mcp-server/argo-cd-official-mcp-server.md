## Overview

The Argo CD MCP Server from Argo CD Labs is an official implementation of Model Context Protocol (MCP) server for Argo CD, enabling AI assistants to interact with your Argo CD applications through natural language. This server bridges the gap between GitOps and AI-powered development, making Kubernetes application management conversational.

## Features

- **Application Management**: Create, sync, delete, and rollback applications
- **Project Management**: Manage Argo CD projects and configurations
- **Repository Management**: Add/remove Git repositories and Helm charts
- **Cluster Management**: Manage Kubernetes cluster connections
- **Sync Operations**: Execute and monitor synchronization operations
- **Health Monitoring**: Monitor application health and status
- **RBAC Management**: Role-based access control configuration
- **GitOps Workflows**: Natural language GitOps operations
- **Multi-tenancy Support**: Manage multiple tenants and environments
- **Application Sets**: Work with ApplicationSet resources

## Natural Language Capabilities

Users can manage deployments using plain conversational language:
- "What applications are out of sync in production?"
- "Sync the api-service application"
- "Rollback the frontend to the previous version"
- "Show me the health status of all apps in staging"

## Comprehensive API Coverage

Includes comprehensive Argo CD API coverage with JWT token authentication for secure operations.

## Transport Protocols

Supports both stdio and HTTP stream transport protocols for seamless integration with Visual Studio Code and other MCP clients.

## Use Cases

- GitOps continuous delivery with natural language
- Kubernetes application lifecycle management
- Multi-environment deployment coordination
- Application health monitoring and troubleshooting
- Automated sync and rollback operations
- Team collaboration on deployments

## Integration with EKS

Works with Amazon EKS and other Kubernetes distributions for GitOps continuous delivery using natural language.

## Supported Clients

VS Code, Cursor, Claude Desktop, and any MCP-compatible AI assistant.

## Authentication

Requires Argo CD connection details and JWT token for secure API access.

## Pricing

Open-source implementation. Argo CD and Kubernetes hosting costs apply separately.