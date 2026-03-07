## Overview

The Puppeteer MCP server is an official Model Context Protocol server providing comprehensive browser automation capabilities using Puppeteer. It enables LLMs to interact with web pages, capture screenshots, and execute JavaScript in real browser environments.

## Key Features

- **Browser Automation**: Control Chrome/Chromium browsers programmatically
- **Screenshot Capture**: Full-page or element-specific screenshots
- **JavaScript Execution**: Run custom JavaScript in browser context
- **Console Monitoring**: Capture and analyze browser console messages
- **Resource Management**: Efficient browser instance lifecycle management
- **Security Controls**: Configurable security settings and dangerous operation blocking
- **Headless Configuration**: Run browsers with or without UI
- **Docker Support**: Container deployment with headless Chromium
- **Existing Window Support**: Connect to already-running Chrome instances

## Installation Options

**NPX Installation (Recommended):**
```bash
npx -y @modelcontextprotocol/server-puppeteer
```

Configuration for Claude Desktop:
```json
{
  "mcpServers": {
    "puppeteer": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-puppeteer"]
    }
  }
}
```

**Docker Installation:**
- Docker version uses headless Chromium
- NPX version opens browser window by default
- Full containerization support for isolated execution

## Headless Configuration

Customize Puppeteer's browser behavior using PUPPETEER_LAUNCH_OPTIONS:

```json
{
  "env": {
    "PUPPETEER_LAUNCH_OPTIONS": "{\"headless\": false, \"args\": []}"
  }
}
```

This allows control over:
- Headless mode (true/false)
- Browser arguments
- Window size and position
- GPU acceleration
- Sandbox settings

## Security Features

Dangerous LaunchOptions that reduce security can be allowed or blocked:

- When false (default), dangerous args like `--no-sandbox` and `--disable-web-security` will throw errors
- Prevents accidental security reductions
- Configurable based on trust level and use case

## Supported Operations

**Page Navigation:**
- Navigate to URLs
- Click elements
- Fill forms
- Submit data

**Content Interaction:**
- Find elements by selectors
- Extract text and attributes
- Modify page content
- Trigger events

**Capture & Analysis:**
- Screenshot capture (full page, viewport, or specific elements)
- Console message monitoring
- Network request/response inspection
- Performance metrics

**JavaScript Execution:**
- Execute custom scripts
- Access DOM
- Manipulate page state
- Return data to AI

## Use Cases

- **Automated Testing**: E2E testing of web applications
- **Web Scraping**: Extract data from dynamic web pages
- **Form Automation**: Automatically fill and submit forms
- **Visual Testing**: Capture screenshots for regression testing
- **Data Collection**: Gather information from interactive sites
- **Monitoring**: Check website status and content
- **PDF Generation**: Convert web pages to PDF
- **Performance Analysis**: Measure page load and render times

## Deployment Options

**Local Development:**
- NPX with local Chromium installation
- Opens visible browser window for debugging

**Containerized:**
- Docker with headless Chromium
- Isolated execution environment
- No local browser installation required

**Cloud:**
- Successfully deployed on Cloudflare Workers
- Integration with Browserless.io for managed browser instances

## Browser Support

- Chrome (primary)
- Chromium
- Microsoft Edge (Chromium-based)

## Integration with Existing Chrome

Can connect to existing Chrome windows for:

- Debugging running applications
- Interacting with authenticated sessions
- Working with specific browser profiles

## Technical Details

- Built on Google Puppeteer
- Node.js implementation
- Async/await API
- Event-driven architecture
- DevTools Protocol communication

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Other MCP-compatible assistants

## Performance Considerations

- Browser instances managed efficiently
- Automatic cleanup of resources
- Configurable timeouts
- Page caching options
- Memory management

## Pricing

Free and open-source under the MIT License. Cloud deployment costs depend on hosting provider.