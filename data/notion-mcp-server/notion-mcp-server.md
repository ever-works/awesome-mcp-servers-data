## Features

### Database Operations
- Query databases
- Create database entries
- Update properties
- Filter and sort data

### Page Management
- Create pages
- Update page content
- Retrieve page blocks
- Manage page properties

### Workspace Access
- List workspaces
- Access workspace settings
- Manage permissions

## Authentication
Requires NOTION_API_KEY environment variable.

## Setup Examples

**Cursor:**
```json
{
  "mcpServers": {
    "notion": {
      "url": "https://mcp.notion.com/mcp",
      "env": {
        "NOTION_API_KEY": "your-api-key"
      }
    }
  }
}
```

**Claude Desktop:** Edit config file with similar structure.

## Use Cases
Multi-platform content management, AI agent integration for Notion databases and pages.