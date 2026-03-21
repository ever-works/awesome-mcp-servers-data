## Overview

MCP-Insomnia is an MCP (Model Context Protocol) server that enables AI agents to create and manage API collections in Insomnia-compatible format. It provides tools and resources for managing collections, requests, and environments that can be exported to Insomnia for testing and collaboration.

## Features

### Collection Management
- **Create Collections**: Build API test suites from scratch
- **Organize Requests**: Group related API calls together
- **Manage Folders**: Structure collections hierarchically
- **Export to Insomnia**: Generate Insomnia-compatible JSON files

### Request Building
- **HTTP Methods**: Support for GET, POST, PUT, DELETE, PATCH, etc.
- **Request Headers**: Configure authentication and content types
- **Request Bodies**: JSON, form data, and other formats
- **Query Parameters**: Add and manage URL parameters

### Environment Configuration
- **Environment Variables**: Define variables for different environments
- **Base URLs**: Configure API endpoints per environment
- **Authentication Tokens**: Store and manage API keys securely
- **Environment Switching**: Easy dev/staging/production transitions

## Use Cases

### AI-Assisted API Testing
- Generate API test collections from documentation
- Create requests based on OpenAPI/Swagger specs
- Build comprehensive test suites automatically
- Export to Insomnia for execution

### Documentation to Tests
- Convert API documentation to test collections
- Generate sample requests from examples
- Create environment configurations
- Organize tests by API endpoint

### Team Collaboration
- Generate standardized test collections
- Share Insomnia-compatible exports
- Maintain consistent API testing practices
- Version control test suites

### Test Suite Development
- Quickly scaffold API test collections
- Add authentication and headers
- Configure multiple environments
- Prepare for integration testing

## Insomnia Compatibility

The server generates collections that are fully compatible with:
- Insomnia REST Client
- Insomnia Designer
- Insomnia CLI for CI/CD
- Insomnia team workspaces

## Workflow

1. Use AI assistant to describe API endpoints
2. Generate collection structure with MCP server
3. Add requests, headers, and authentication
4. Configure environment variables
5. Export to Insomnia format
6. Import into Insomnia for testing

## Integration

Works with AI assistants supporting MCP like Claude and Cursor. Generates JSON files compatible with Insomnia's import format.

## Pricing

Free and open-source. Works with free version of Insomnia.