## Overview

The Fetch MCP server is an official Anthropic implementation designed for web content fetching and conversion for efficient LLM usage. It retrieves and transforms web content—HTML, JSON, plain text, and Markdown—into clean, token-optimized formats.

## Key Features

- **Multi-Format Support**: Handles HTML, JSON, plain text, and Markdown
- **Markdown Conversion**: Converts webpages to clean Markdown for better LLM comprehension
- **Content Truncation**: Configurable maximum content length to manage token usage
- **Pagination Support**: Process long articles in manageable chunks via start_index parameter
- **Token Optimization**: Reduces costs and improves LLM understanding through efficient formatting
- **Live Web Access**: Gives LLMs real-time access to web content
- **Header Support**: Custom HTTP headers for authentication and requests
- **Error Handling**: Robust handling of network and content errors

## How It Works

1. AI identifies need for web content
2. Fetch server retrieves the URL content
3. Content is converted to optimal format (usually Markdown)
4. Large content can be paginated using max_length and start_index
5. Clean, formatted content returned to AI

## Complementary to Search

Fetch and search tools are complementary:

- **Search** (Brave, Tavily, etc.): Finds relevant URLs
- **Fetch**: Reads and converts the content from those URLs

An agent would first use a search tool to find relevant pages, then use Fetch to consume their content.

## Parameters

**max_length**: Maximum content length to retrieve (for token management)

**start_index**: Starting position for pagination (enables processing extremely long articles in chunks)

**headers**: Custom HTTP headers for the request

**timeout**: Request timeout duration

## Supported Content Types

- **HTML Pages**: Converted to clean Markdown
- **JSON APIs**: Structured data retrieval
- **Plain Text**: Direct text content
- **Markdown Files**: Already-formatted content
- **RSS/Atom Feeds**: Feed content extraction

## Token Savings

Markdown conversion provides significant benefits:

- Saves tokens by removing HTML formatting overhead
- Reduces API costs
- Improves LLM's content comprehension
- Focuses on semantic content over presentation

## Community Variants

While Anthropic maintains an official Python implementation, the community has developed powerful variants:

- **Node.js implementations**: JavaScript/TypeScript versions
- **Rust implementations**: High-performance alternatives
- **Extended features**: Additional parsing and extraction capabilities

## Use Cases

- **Documentation Retrieval**: Fetch and parse technical documentation
- **Article Reading**: Convert news articles and blog posts
- **API Integration**: Retrieve and parse JSON API responses
- **Research**: Gather content from multiple web sources
- **Data Collection**: Extract structured data from web pages
- **Content Summarization**: Retrieve content for AI summarization
- **Fact Checking**: Fetch source material for verification

## Integration with Claude Desktop

Configured easily in Claude Desktop to give Claude live web access for reading and understanding web content on demand.

## Technical Details

- Official Python implementation in modelcontextprotocol/servers repository
- Supports HTTP/HTTPS protocols
- Handles redirects automatically
- Respects robots.txt (configurable)
- User-agent customization
- Timeout management

## Example Workflow

1. User asks about recent news on a topic
2. AI uses search tool to find relevant articles
3. AI uses Fetch to retrieve article content
4. Content converted to Markdown
5. AI analyzes and summarizes the content

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Other MCP-compatible AI assistants

## Pricing

Free and open-source under the MIT License.