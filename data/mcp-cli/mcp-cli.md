# MCP CLI

A command-line inspector for testing, interacting with, and managing MCP (Model Context Protocol) servers. It helps developers and users validate and debug server implementations directly from the terminal.

## Features
- **Inspect MCP Servers:** Send JSON-RPC 2.0 requests over stdio to MCP servers and inspect responses.
- **List Available Tools:** Query the server for all available tools and their input schemas.
- **Test Individual Tools:** Invoke specific server tools (such as `read_file` or `read_multiple_files`) with custom arguments.
- **Explore Resources:** List and interact with resources exposed by the MCP server.
- **jq Integration:** Use jq filters to process and extract information from JSON responses (e.g., listing tool names, extracting input schemas, or getting call responses).
- **Shell Helper Functions:** Define reusable shell functions (`mcp_tools`, `mcp_call`, `mcp_resources`) for common MCP server operations.
- **Debugging Support:**
  - Validate server-provided JSON Schemas.
  - Monitor server logs by redirecting stderr to a file and using `tail`.
  - Test error handling by sending invalid requests or arguments.
- **Automation:** Enables scripting and automating MCP server testing and debugging workflows.

## Pricing
No pricing information is provided.

## Source
[Inspecting and Debugging MCP Servers Using CLI and jq](https://blog.fka.dev/blog/2025-03-25-inspecting-mcp-servers-using-cli/)
