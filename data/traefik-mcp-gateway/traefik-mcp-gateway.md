## Overview

Traefik's MCP Gateway governs how agents access MCP servers (tools, prompts, resources) with identity-aware policy, session-smart routing, and deep observability. The Model Context Protocol (MCP) middleware enables secure, governed access to MCP servers by acting as an OAuth-compliant gateway.

## Features

- **OAuth 2.1/2.0 Compliant**: Standard-compliant access control
- **Resource Metadata Discovery**: Automatic MCP server capability discovery
- **Task-Based Access Control (TBAC)**: Fine-grained permission management
- **YAML Policy Engine**: Declarative policy configuration
- **Identity-Aware Routing**: Route based on agent identity
- **Session Management**: Smart session handling and persistence
- **Deep Observability**: Comprehensive monitoring and logging
- **Centralized Access Control**: Single point of policy enforcement

## Policy Management

YAML policies combine:
- Agent identity
- Tasks and tools
- Transaction conditions
- Resource constraints
- Time-based access

## Key Capabilities

- Control which agents can access which MCP servers
- Define granular permissions for tools and resources
- Monitor agent behavior and resource usage
- Audit all MCP transactions
- Enforce compliance policies
- Manage authentication flows

## Use Cases

- Enterprise AI agent governance
- Multi-tenant MCP deployments
- Compliance and audit requirements
- Security policy enforcement
- Resource access control
- Agent behavior monitoring
- Identity-based routing

## Integration with Traefik Hub

Part of Traefik Hub platform providing:
- API gateway functionality
- Kubernetes ingress
- Service mesh
- API management
- Developer portal

## Getting Started

Configuration through:
- YAML-based policy definitions
- Kubernetes CRDs
- Dynamic configuration
- OAuth provider integration

## Integration Benefits

- Centralized MCP governance
- Fine-grained access control
- Simplified policy management
- Enhanced security posture
- Comprehensive audit trails
- Multi-tenant isolation

## Cloud-Native Architecture

- Kubernetes-native deployment
- Container-ready
- Microservices compatible
- Scalable and resilient

## Compatibility

Works with any MCP server and MCP-compatible AI agent. Supports OAuth 2.0/2.1 identity providers.

## Pricing

Traefik Proxy is open-source. Traefik Hub (including MCP Gateway) offers free and enterprise tiers.