## Overview

The Kubernetes MCP Server is a Model Context Protocol server for Kubernetes and OpenShift that enables AI assistants like VS Code, Microsoft Copilot, and Cursor to safely and intelligently interact with Kubernetes clusters. Unlike other implementations, this is a Go-based native implementation that interacts directly with the Kubernetes API server.

## Key Features

- **Native API Integration**: Direct Kubernetes API interaction (NOT a kubectl wrapper)
- **No External Dependencies**: No need for kubectl, helm, or other CLI tools installed
- **Multi-Cluster Support**: Interact with multiple Kubernetes clusters simultaneously
- **Native Binaries**: Distributed as single binaries for Linux, macOS, and Windows
- **High Performance**: Low-latency direct API communication
- **Helm Support**: Chart installation, listing releases, uninstalling releases
- **Read-Only Mode**: Debug or inspect clusters without making changes
- **Safety Modes**: Configurable access levels (read-only, non-destructive, full)
- **Generic Resource Operations**: CRUD operations on any Kubernetes resource including custom resources
- **Extended Pod Operations**: Event retrieval, log access, command execution, and resource metrics (top)

## Major Implementations

**1. containers/kubernetes-mcp-server (Go)**
- Native Kubernetes API integration
- No external tool dependencies
- Single binary distribution
- Production-ready performance

**2. Flux159/mcp-server-kubernetes (Node.js)**
- Non-destructive mode for read and create/update-only access
- Secrets masking for security
- Optional OpenTelemetry integration
- Multi-source kubeconfig loading

**3. rohitg00/kubectl-mcp-server**
- Multiple transport support: stdio, SSE, HTTP, streamable-http
- Visual HTML dashboards
- Powerful CLI for shell-friendly tool discovery
- Multi-cluster context management

**4. alexei-led/k8s-mcp-server**
- Bridge between LLMs and Kubernetes CLI tools
- Built-in kubectl, helm, istioctl, argocd support
- Single containerized environment
- Security-focused design

## Supported Operations

**Cluster Management:**
- List nodes, pods, deployments, services
- Get resource details
- Create, update, delete resources
- Apply manifests
- Scale deployments

**Helm Operations:**
- Install charts
- List releases
- Upgrade releases
- Uninstall releases
- Rollback deployments

**Pod Operations:**
- View logs
- Execute commands (kubectl exec)
- Port forwarding
- Resource metrics (CPU, memory)
- Event monitoring

**Advanced:**
- Custom Resource Definitions (CRDs)
- Network policies
- RBAC configuration
- Service mesh (Istio) management
- GitOps (ArgoCD) operations

## Natural Language Queries

Cluster administrators can pose natural language questions:

- "Show me all pods in CrashLoopBackOff in the last 24 hours"
- "Why is my deployment not scaling?"
- "List all services in the production namespace"
- "What's the CPU usage of my pods?"
- "Deploy nginx with 3 replicas"

## Security Features

- **Service Account Support**: Run with dedicated service accounts
- **Read-Only Configuration**: Optional read-only mode for safe exploration
- **RBAC Compliance**: Respects Kubernetes RBAC policies
- **Secrets Masking**: Automatic masking of sensitive information
- **Configurable Safety Modes**: Control level of access and modifications
- **Audit Logging**: Track all operations for compliance

## Use Cases

- **Cluster Administration**: Manage Kubernetes clusters via natural language
- **Troubleshooting**: Diagnose issues with AI assistance
- **Resource Management**: Create and modify resources conversationally
- **Monitoring**: Query cluster state and metrics
- **GitOps**: Manage ArgoCD applications
- **Service Mesh**: Configure Istio resources
- **CI/CD Integration**: Automate deployments with AI
- **Learning**: Explore Kubernetes with AI guidance

## Multi-Cluster Management

All implementations support managing multiple clusters:

- Load multiple kubeconfig files
- Switch contexts seamlessly
- Query across clusters
- Consistent operations across environments

## Observability

Optional OpenTelemetry integration provides:

- Request tracing
- Performance metrics
- Error tracking
- Distributed tracing

## Compatible AI Clients

- VS Code with Copilot
- Microsoft Copilot
- Cursor
- Claude Desktop
- Claude Code
- IntelliJ IDEA
- PyCharm
- Other MCP-compatible IDEs and AI assistants

## Installation

**Go Native Binary:**
```bash
# Download from releases
curl -L https://github.com/containers/kubernetes-mcp-server/releases/latest/download/kubernetes-mcp-server-linux
```

**Node.js:**
```bash
npm install -g mcp-server-kubernetes
```

**Python:**
```bash
pip install mcp-kubernetes-server
```

## Configuration

Typically uses existing kubeconfig files:

- ~/.kube/config (default)
- Multiple config files supported
- Environment variable override (KUBECONFIG)
- In-cluster configuration for pod deployment

## Pricing

Free and open-source. Multiple implementations available under permissive licenses (MIT, Apache 2.0).