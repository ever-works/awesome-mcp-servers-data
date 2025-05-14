# apisix-mcp

**Description:**  
APISIX Model Context Protocol (MCP) server enables integration between large language models (LLMs) and the Apache APISIX Admin API. It allows natural language-based viewing and management of APISIX resources via MCP-compatible AI clients.

**Source:** [https://github.com/api7/apisix-mcp](https://github.com/api7/apisix-mcp)

**Category:** api-integration-mcp-servers

**Tags:** mcp, apisix, api-integration, gateway

---

## Features

### Common Operations
- **get_resource**: Retrieve resources by type (routes, services, upstreams, etc.)
- **delete_resource**: Remove resources by ID
- **send_request_to_gateway**: Send one or multiple requests to the APISIX gateway

### API Resources Operations
- **create_route / update_route / delete_route**: Manage routes
- **create_service / update_service / delete_service**: Manage services
- **create_upstream / update_upstream / delete_upstream**: Manage upstreams
- **create_ssl / update_ssl / delete_ssl**: Manage SSL certificates
- **create_or_update_proto**: Manage protobuf definitions
- **create_or_update_stream_route**: Manage stream routes

### Plugin Operations
- **get_all_plugin_names**: List all available plugin names
- **get_plugin_info / get_plugins_by_type / get_plugin_schema**: Retrieve plugin configurations
- **create_plugin_config / update_plugin_config**: Manage plugin configurations
- **create_global_rule / update_global_rule**: Manage plugin global rules
- **get_plugin_metadata / create_or_update_plugin_metadata / delete_plugin_metadata**: Manage plugin metadata

### Security Configuration
- **get_secret_by_id / create_secret / update_secret**: Manage secrets
- **create_or_update_consumer / delete_consumer**: Manage consumers
- **get_credential / create_or_update_credential / delete_credential**: Manage consumer credentials
- **create_consumer_group / delete_consumer_group**: Manage consumer groups

### Integration
- Supports configuration via Smithery, npm, or from source code.
- Designed to work with AI clients such as Cursor, Claude, Copilot, etc.
- Requires configuration of APISIX server host, ports, API key, and other environment variables.

### Technical Details
- Written primarily in TypeScript.
- Licensed under Apache-2.0.

---

## Pricing
No pricing information is provided; the project is open-source under the Apache-2.0 license.
