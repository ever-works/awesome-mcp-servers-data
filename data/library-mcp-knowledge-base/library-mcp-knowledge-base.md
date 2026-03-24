## Overview

Library MCP Knowledge Base is a simple MCP server that enables AI assistants like Claude Desktop to explore and interact with Markdown knowledge bases. It's designed for folders containing files with .md extensions that start with metadata including title, tags, and URL.

## Features

- **Metadata Support**: Parse and utilize frontmatter metadata (title, tags, URL)
- **File Discovery**: Automatically discover and index Markdown files
- **Tag-based Navigation**: Browse content by tags and categories
- **Full-text Search**: Search across all markdown content
- **Link Resolution**: Handle internal links between documents
- **Hierarchical Structure**: Support for nested folder organizations
- **URL Mapping**: Associate markdown files with original URLs
- **Version Tracking**: Track changes to knowledge base content

## Metadata Format

Expected frontmatter structure:
```markdown
---
title: Document Title
tags: [tag1, tag2, tag3]
url: https://original-source.com
---

Document content here...
```

## Use Cases

- Organize personal knowledge bases (Zettelkasten, digital gardens)
- Manage documentation repositories
- Build searchable note collections
- Create research databases
- Organize bookmarks and saved articles
- Maintain technical documentation
- Build team knowledge wikis

## Integration

Works with tools like:
- Claude Desktop for conversational knowledge base queries
- Custom note-taking applications
- Documentation generation systems
- Content management workflows

## Pricing

Free and open-source.