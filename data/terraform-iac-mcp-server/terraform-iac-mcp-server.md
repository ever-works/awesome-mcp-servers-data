## Overview

The Terraform MCP Server bridges AI assistants with HashiCorp Terraform, enabling infrastructure-as-code operations through natural language commands. It simplifies complex Terraform workflows by handling plan-apply cycles with built-in safety features.

## Features

- **Plan Automation**: Automatic terraform plan generation from natural language
- **Change Visualization**: Shows what will change before applying
- **Approval Workflows**: Optional approval step before applying changes
- **Multi-Environment**: Support for staging, production, and custom environments
- **State Management**: Safe handling of Terraform state
- **Module Support**: Work with Terraform modules and providers

## Capabilities

- Execute `terraform plan` via conversational commands
- Review planned infrastructure changes
- Apply configurations with approval gates
- Manage Terraform workspaces
- Query current infrastructure state
- Validate configuration files
- Initialize Terraform projects

## Workflow Example

User: "Apply terraform for staging"

1. Server runs terraform plan
2. Displays infrastructure changes
3. Waits for approval (if configured)
4. Applies changes upon confirmation

## Use Cases

- AI-assisted infrastructure provisioning
- Automated environment setup
- Infrastructure change reviews
- Multi-cloud resource management
- Disaster recovery automation
- Cost optimization through resource right-sizing

## Safety Features

- Preview changes before application
- Optional manual approval step
- State backup and recovery
- Dry-run mode support

## Requirements

- Terraform CLI installed
- Appropriate cloud provider credentials
- MCP-compatible AI client

## Pricing

Free and open-source MCP server. Terraform and cloud provider costs apply.