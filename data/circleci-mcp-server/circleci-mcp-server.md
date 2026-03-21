## Overview

The CircleCI MCP Server connects your AI assistant to CI/CD data, allowing you to debug builds, analyze test results, and optimize pipelines using natural language. The server runs locally and integrates with a variety of editors and LLM development tools.

## Features

### Build Operations
- **Trigger Builds**: Start builds with specific parameters
- **Monitor Status**: Check build and workflow status
- **Access Logs**: Retrieve detailed build logs for debugging
- **Build History**: Query past builds by branch, status, or time

### Test Analytics
- **Test Results**: Analyze test outcomes and failures
- **Performance Metrics**: Track test execution times
- **Flaky Test Detection**: Identify unreliable tests
- **Coverage Analysis**: View code coverage trends

### Pipeline Optimization
- **Performance Insights**: Identify slow steps and bottlenecks
- **Resource Usage**: Monitor credit consumption
- **Workflow Analysis**: Optimize pipeline configurations
- **Caching Recommendations**: Improve build times

### Artifact Management
- **Download Artifacts**: Retrieve build artifacts
- **Artifact History**: Track artifact changes over time
- **Storage Metrics**: Monitor artifact storage usage

## CircleCI Platform Capabilities

### CI/CD Features
- Docker and machine executors
- Parallel job execution
- Workflow orchestration
- Advanced caching strategies
- Reusable config with orbs

### Integrations
- GitHub and Bitbucket
- Slack and Jira notifications
- AWS, GCP, Azure deployments
- Third-party deployment tools

### Enterprise Features
- Self-hosted runners
- IP ranges and security
- Audit logging
- Advanced insights and analytics

## Use Cases

### Build Debugging
- Query failed builds by branch or commit
- Analyze error messages and logs
- Compare successful vs failed builds
- Get AI-assisted debugging suggestions

### Test Management
- Identify most frequently failing tests
- Analyze flaky test patterns
- Track test performance over time
- Generate test quality reports

### Pipeline Optimization
- Identify slowest pipeline steps
- Find optimization opportunities
- Analyze resource consumption
- Implement caching improvements

### Team Productivity
- Monitor build queue times
- Track team velocity metrics
- Identify deployment bottlenecks
- Generate performance reports

## Integration

Works with AI assistants supporting MCP including Claude, Cursor, VS Code extensions, and other compatible tools. The server runs locally on your machine and connects to CircleCI's API. Requires CircleCI API token for authentication.

## Pricing

CircleCI offers a free tier with 6,000 build minutes per month. Paid plans provide additional credits and features. The MCP server is free to use with any CircleCI plan.