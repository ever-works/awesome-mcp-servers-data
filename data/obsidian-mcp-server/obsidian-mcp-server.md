## Overview

The Obsidian MCP Server provides comprehensive access to your Obsidian vault, enabling LLMs and AI agents to read, write, search, and manage your notes and files through the Obsidian Local REST API plugin. It acts as a bridge between AI assistants and your personal knowledge base.

## Key Features

- **Note Reading**: Access and read note contents
- **Note Writing**: Create new notes with content
- **Content Updates**: Append, prepend, or overwrite existing notes
- **Search Capabilities**: Global text search and regex pattern matching
- **Search & Replace**: Find and replace content across vault
- **Directory Listing**: Browse vault structure and files
- **Note Deletion**: Remove notes when needed
- **Frontmatter Management**: Read and modify YAML frontmatter
- **Tag Management**: Add, remove, and search by tags
- **Automated Vault Management**: AI-driven organization and maintenance

## Core Capabilities

**Reading:**
- Read individual notes
- Access note metadata
- Retrieve frontmatter data
- List vault directories
- Browse files by path

**Writing:**
- Create new notes
- Append content to existing notes
- Prepend content to notes
- Overwrite note contents completely
- Update frontmatter fields

**Searching:**
- Full-text search across vault
- Regex pattern matching
- Tag-based search
- Search and replace operations
- Filter by metadata

**Management:**
- Add and remove tags
- Update frontmatter properties
- Organize note structure
- Delete obsolete notes
- Maintain vault consistency

## Use Cases

**Direct AI Access to Knowledge Base:**
AI assistants can read and reference existing notes for context, understanding, and information retrieval from your personal knowledge repository.

**Automated Note-Taking:**
Create, update, and organize notes through AI interactions, automatically capturing information from conversations and research.

**Enhanced Search:**
Leverage AI for finding connections across your entire vault, discovering relationships you might have missed.

**Content Organization:**
AI can help tag, categorize, and structure notes for better organization and retrieval.

**Knowledge Graph Building:**
Automatically create links between related notes and build comprehensive knowledge networks.

**Meeting Notes Automation:**
Generate meeting notes automatically with proper formatting, tags, and frontmatter.

**Research Assistance:**
Compile research from multiple notes, synthesize information, and create summaries.

## Setup Requirements

**Prerequisites:**
1. Obsidian application installed
2. Obsidian Local REST API Plugin installed and enabled
3. Plugin configured with API credentials
4. Vault path configured in plugin settings

## Available Implementations

**1. cyanheads/obsidian-mcp-server** (Full-featured)
- Comprehensive tool suite
- Complete CRUD operations
- Advanced search capabilities
- Frontmatter and tag management
- Production-ready stability

**2. Obsidian HTTP MCP** (Lightweight)
- HTTP-based vault exposure
- Natural language search
- Automated note modifications
- Analytics and summaries
- Cursor integration optimized

**3. markuspfundstein/obsidian** (Alternative implementation)
- Additional tool options
- Custom configuration
- Alternative API approach

## Obsidian Local REST API

The MCP server communicates with Obsidian through the Local REST API plugin:

- Local HTTP API for vault access
- Secure authentication
- Comprehensive endpoint coverage
- Real-time vault updates
- No cloud dependency

## AI Workflow Integration

**With Claude Desktop:**
- Ask questions about notes
- Create notes from conversations
- Search vault via natural language
- Organize and tag automatically

**With Cursor:**
- Reference notes while coding
- Generate documentation
- Search code-related notes
- Maintain development journals

**With VS Code:**
- Integrate notes with development
- Auto-generate project documentation
- Maintain technical knowledge base

## Frontmatter Management

Frontmatter is YAML metadata at the top of Markdown notes:

```yaml
---
title: My Note
tags: [project, important]
date: 2026-03-07
---
```

The MCP server can:
- Read frontmatter fields
- Add new fields
- Update existing fields
- Remove fields
- Maintain YAML validity

## Tag System

Comprehensive tag management:

- Add tags to notes
- Remove tags from notes
- Search notes by tags
- List all vault tags
- Batch tag operations
- Tag hierarchy support

## Search Features

**Text Search:**
- Case-sensitive or insensitive
- Whole word matching
- Multi-term queries

**Regex Search:**
- Advanced pattern matching
- Complex query support
- Capture groups

**Search & Replace:**
- Global replacements
- Preview before replace
- Undo support via Obsidian

## Security Considerations

- Local API, no cloud dependency
- Authentication via API key
- Restricted to configured vault
- File system permissions respected
- No external data transmission

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- Continue
- Custom MCP implementations

## Natural Language Operations

Example AI interactions:

- "Create a note about today's standup meeting"
- "Find all notes tagged with 'project-alpha'"
- "Add a summary section to my weekly review note"
- "Search for notes mentioning machine learning"
- "Tag all notes about Python with 'programming'"

## Installation

**Step 1: Install Obsidian Local REST API Plugin**
- Open Obsidian Settings
- Navigate to Community Plugins
- Search for "Local REST API"
- Install and enable

**Step 2: Configure Plugin**
- Set API key
- Configure port (default 27123)
- Enable CORS if needed

**Step 3: Install MCP Server**
```bash
npm install obsidian-mcp-server
```

**Step 4: Configure MCP Client**
Add vault path and API credentials to your MCP client configuration.

## Pricing

Free and open-source. Obsidian application pricing applies (free for personal use, paid for commercial).