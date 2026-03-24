## Overview

Infrastructure Diagram MCP is an MCP server that seamlessly creates infrastructure diagrams for AWS, Azure, GCP, Kubernetes, and more. It provides multi-provider support for creating diagrams across cloud platforms, on-premises infrastructure, and hybrid/multi-cloud architectures.

## Features

- **Multi-Provider Support**: AWS, GCP, Azure, Kubernetes, on-premises
- **Hybrid Architectures**: Visualize multi-cloud and hybrid setups
- **Auto-generation**: Create diagrams from infrastructure code
- **Customizable Layouts**: Flexible diagram arrangements
- **Export Formats**: PNG, SVG, PDF output
- **Icon Libraries**: Comprehensive cloud service icons
- **Relationship Mapping**: Show connections between resources
- **Grouping**: Logical resource grouping (VPCs, regions, etc.)

## Supported Providers

### AWS
- All major AWS services
- Region and AZ representation
- VPC and subnet layouts
- Security group relationships

### Azure
- Azure services and resources
- Resource groups
- Virtual networks
- Subscription organization

### GCP
- Google Cloud services
- Project organization
- VPC networks
- Service interconnections

### Kubernetes
- Cluster architecture
- Namespaces
- Pods and services
- Ingress and networking

### On-Premises
- Data center layouts
- Network topology
- Server infrastructure
- Hybrid connections

## Diagram Capabilities

- **Architecture Diagrams**: High-level system design
- **Network Diagrams**: Detailed network topology
- **Security Diagrams**: Security zones and controls
- **Data Flow**: Show data movement between components
- **Deployment Diagrams**: Application deployment layout
- **Reference Architectures**: Standard patterns and templates

## Use Cases

- Document existing infrastructure
- Design new system architectures
- Create technical documentation
- Present architecture to stakeholders
- Plan migration strategies
- Security and compliance documentation
- Disaster recovery planning
- Training and onboarding materials

## Integration

- Parse Terraform configurations
- Import CloudFormation templates
- Read Kubernetes manifests
- API integration with cloud providers
- Export to documentation tools

## Output Formats

- **PNG**: Raster images for documents
- **SVG**: Vector graphics for editing
- **PDF**: Printable diagrams
- **Diagrams as Code**: Python code for programmatic generation

## Pricing

Free and open-source under the MIT license.