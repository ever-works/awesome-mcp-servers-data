## Overview

AWS MCP Server is a fully managed remote Model Context Protocol server that provides AI assistants with secure access to AWS services through natural language interactions. It transforms AWS infrastructure management by allowing developers to create, read, update, delete, and list resources using conversational commands.

## Key Features

- **Unified Interface**: Consolidates capabilities from AWS API MCP and AWS Knowledge servers into one interface
- **15,000+ AWS APIs**: Access to over 15,000 AWS APIs including newly released services
- **AWS Documentation**: Direct access to AWS documentation and best practices
- **Agent SOPs**: Pre-built workflows (standard operating procedures) that guide AI agents through common AWS tasks
- **Natural Language Management**: Create and manage AWS infrastructure using conversational language
- **IAM-Based Security**: Zero credential exposure with standard AWS Identity and Access Management controls
- **CloudTrail Audit Logging**: Complete audit logging through AWS CloudTrail for compliance
- **Syntactic Validation**: All API calls are syntactically validated before execution

## Architecture

**MCP Client-Server Model**: Host applications (chatbots, IDEs, AI tools) have MCP clients that maintain 1:1 connections with MCP servers. Common clients include:

- Agentic AI coding assistants (Kiro, Cline, Cursor, Windsurf)
- Chatbot applications like Claude Desktop
- Visual Studio Code with Copilot
- Other MCP-compatible tools

MCP Servers for AWS use this protocol to provide AI applications access to AWS documentation, contextual guidance, and best practices through the standardized client-server architecture.

## Available AWS MCP Server Categories

- **Essential**: Official AWS managed servers
- **Documentation**: AWS Knowledge servers for documentation access
- **Infrastructure**: CloudFormation, CDK, and Cloud Control API servers
- **Serverless**: AWS Lambda integration servers
- **Data**: Database and analytics services integration
- **Healthcare**: AWS HealthLake integration
- **Compute**: EC2, ECS, and container services
- **Storage**: S3, EBS, and storage management

## Security & Compliance

Built with safety and control in mind:

- Syntactically validated API calls
- IAM-based permissions with zero credential exposure
- Complete CloudTrail audit logging
- Fine-grained access controls
- Role-based security policies

## Use Cases

- Infrastructure provisioning and management
- Resource discovery and inventory
- Compliance and security auditing
- Cost optimization analysis
- Deployment automation
- Troubleshooting and diagnostics
- Documentation search and learning

## Deployment Options

Guidance available for deploying Model Context Protocol servers on AWS infrastructure with scalability and security best practices.

## Pricing

Pay only for the AWS resources you use and any applicable data transfer costs. The MCP server itself has no additional charges.