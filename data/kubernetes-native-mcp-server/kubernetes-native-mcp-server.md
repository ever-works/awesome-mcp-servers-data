## Overview

The Kubernetes Native MCP Server is a Go-based implementation that provides direct interaction with the Kubernetes API server. Unlike other implementations that wrap kubectl, this server natively communicates with Kubernetes APIs for better performance and integration.

## Features

- **Native API Integration**: Direct communication with Kubernetes API server, not a kubectl wrapper
- **Resource Inspection**: View and analyze Kubernetes resources (pods, deployments, services, etc.)
- **Event Monitoring**: Access cluster events for troubleshooting
- **Debug Capabilities**: AI-assisted debugging of cluster failures and issues
- **Cross-Platform**: Available for Linux, macOS, and Windows
- **Multiple Distribution Methods**: Native binary, npm package, Python package, and Docker image

## Supported Operations

- List and describe Kubernetes resources
- View cluster events and logs
- Inspect resource configurations
- Monitor pod status and health
- Query deployment states
- Analyze service configurations

## Installation Options

- Native binary for Linux, macOS, Windows
- npm package for Node.js environments
- Python package for Python workflows
- Container/Docker image for containerized deployments

## Use Cases

- AI-assisted Kubernetes cluster management
- Automated troubleshooting and debugging
- Resource optimization and cost management
- Cluster health monitoring
- DevOps workflow automation
- Infrastructure-as-Code generation

## Advantages Over kubectl Wrappers

- Better performance with native API calls
- More reliable and consistent behavior
- Enhanced error handling and reporting
- Deeper integration capabilities

## Pricing

Free and open-source under standard open-source license.