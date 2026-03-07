## Overview

The Everything MCP Server is Anthropic's official, open-source test and reference server for the Model Context Protocol. It is explicitly designed as a test and reference server and contains no production-grade security, error handling, or performance optimizations. It serves as the perfect starting point for validating MCP client implementations.

## Purpose

Before connecting your app (an MCP client) to a real production system, you connect it to the Everything server to verify that your application can correctly:

- Discover tools
- Read resources
- Handle prompts
- Manage the connection lifecycle

All according to the MCP specification.

## Key Features

- **Mock Tools**: Pre-packaged variety of mock tools for testing
- **Sample Data**: Example data sets for development
- **Example Prompts**: Reference prompt implementations
- **Protocol Validation**: Verify MCP spec compliance
- **Client Testing**: Test tool discovery mechanisms
- **Resource Handling**: Validate resource reading capabilities
- **Prompt Management**: Test prompt handling workflows
- **Connection Lifecycle**: Verify connection management

## What It Includes

**Tools:**
- Sample calculation tools
- Mock data retrieval tools
- Test transformation tools
- Example utility functions
- Simulated API operations

**Resources:**
- Static data resources
- Dynamic resource generation
- File-like resource access
- Structured data examples

**Prompts:**
- Template prompts
- Parameterized prompts
- Multi-step prompt examples
- Context-aware prompts

## Use Cases

**MCP Client Development:**
- Validate new MCP client implementations
- Test protocol compliance
- Debug connection issues
- Verify tool discovery logic

**Integration Testing:**
- Test MCP integration before production deployment
- Validate error handling
- Check edge cases
- Ensure spec compliance

**Learning and Education:**
- Learn MCP protocol mechanics
- Understand client-server interactions
- Study reference implementations
- Build proof-of-concept projects

**Testing Tools:**
Use the built-in MCP Server Inspector to test and debug server functionality in a browser-based interface. Anthropic provides an MCP Inspector command-line tool for testing and debugging MCP servers.

## Not for Production

**Important Limitations:**

The Everything server is NOT suitable for production use:

- No production-grade security
- No comprehensive error handling
- No performance optimizations
- No data persistence
- No authentication/authorization
- No rate limiting
- Mock data only

## Installation

Available via npm:
```bash
npx @modelcontextprotocol/server-everything
```

No configuration required for basic testing.

## Testing Workflow

**Step 1: Start Everything Server**
Launch the server in your development environment.

**Step 2: Connect MCP Client**
Point your MCP client to the Everything server.

**Step 3: Verify Tool Discovery**
Ensure client can discover all available tools.

**Step 4: Test Tool Execution**
Execute various tools and verify responses.

**Step 5: Validate Resources**
Read different resource types.

**Step 6: Handle Prompts**
Process example prompts.

**Step 7: Test Lifecycle**
Verify connection, disconnection, and error scenarios.

## MCP Inspector

The MCP Server Inspector provides:

- Browser-based testing interface
- Real-time request/response viewing
- Tool execution testing
- Resource browsing
- Prompt testing
- Connection monitoring

## Development Benefits

**Rapid Prototyping:**
- Quick setup with no external dependencies
- No API keys or credentials needed
- Instant feedback on client behavior
- Fast iteration cycles

**Comprehensive Testing:**
- Cover all MCP features
- Test error scenarios
- Validate edge cases
- Ensure spec compliance

**Safe Development:**
- No production data at risk
- No real systems affected
- Predictable behavior
- Controlled test environment

## Statistics

Released: November 19, 2024
Estimated Downloads: 354k total (12.4k per week)
License: MIT
Maintenance: Active (official Anthropic project)

## Spec Compliance

The Everything server demonstrates:

- Proper tool definition format
- Correct resource structure
- Standard prompt templates
- Valid response formats
- Error handling patterns
- Connection management

## Example Tools

Typical mock tools include:

- **add**: Add two numbers
- **greet**: Generate greeting message
- **echo**: Echo input text
- **random**: Generate random data
- **calculate**: Perform calculations
- **transform**: Transform data structures

## Example Resources

Sample resources:

- **config**: Mock configuration data
- **users**: Sample user list
- **documents**: Test documents
- **settings**: Example settings

## Example Prompts

- **greeting**: Generate personalized greeting
- **summary**: Summarize provided text
- **analysis**: Analyze data structure

## Compatible MCP Clients

Works with all MCP-compatible clients:

- Claude Desktop (for testing)
- Claude Code (for testing)
- Cursor (for testing)
- Custom MCP client implementations
- Development tools

## Learning Resources

Official resources:

- Anthropic MCP Course (Skilljar)
- Model Context Protocol documentation
- Example servers repository
- MCP specification

## Development Tools

**MCP Inspector:**
- Visual debugging
- Request/response inspection
- Tool testing interface
- Resource browsing

**Command-Line Tools:**
- npx execution
- Configuration testing
- Connection verification

## Best Practices

**When to Use:**
- Developing new MCP clients
- Learning MCP protocol
- Testing integrations
- Validating implementations
- Educational purposes

**When NOT to Use:**
- Production deployments
- Real data processing
- Performance benchmarking
- Security-sensitive operations
- High-availability requirements

## Transitioning to Production

After validating with Everything server:

1. Identify production MCP servers for your use case
2. Configure authentication and credentials
3. Implement proper error handling
4. Add logging and monitoring
5. Set up security measures
6. Deploy to production environment

## Pricing

Free and open-source under the MIT License. No costs or API limits for testing and development.