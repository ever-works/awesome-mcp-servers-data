## Overview

The Argo CD MCP Server, developed by Akuity, provides a natural language interface to Argo CD's GitOps continuous delivery capabilities. It wraps calls to the Argo CD API, allowing AI assistants to manage Kubernetes deployments declaratively.

## Features

- **Application Management**: Create, update, and delete Argo CD applications
- **Sync Operations**: Trigger and monitor application synchronization
- **Deployment Status**: Query application health and sync status
- **GitOps Workflows**: Manage Git-based deployment workflows
- **Rollback Support**: Revert applications to previous versions
- **Multi-Cluster**: Manage deployments across multiple Kubernetes clusters

## Capabilities

- List and describe Argo CD applications
- Synchronize applications with Git repositories
- View deployment history and status
- Manage application resources and manifests
- Configure sync policies and auto-sync
- Monitor application health and metrics
- Execute rollbacks and promotions

## Use Cases

- AI-assisted GitOps workflows
- Automated deployment management
- Multi-environment promotion pipelines
- Deployment troubleshooting and debugging
- Application health monitoring
- Configuration drift detection
- Automated rollback operations

## Integration with Argo CD

- Direct API integration with Argo CD
- Supports all Argo CD authentication methods
- Compatible with Argo CD RBAC policies
- Works with Argo CD notifications and webhooks

## Requirements

- Argo CD instance (self-hosted or managed)
- Argo CD API credentials
- MCP-compatible AI client
- Kubernetes cluster access

## Developer

Developed and maintained by Akuity, the company founded by Argo project creators.

## Pricing

Free and open-source MCP server. Argo CD is open-source. Akuity offers managed Argo CD with additional features.