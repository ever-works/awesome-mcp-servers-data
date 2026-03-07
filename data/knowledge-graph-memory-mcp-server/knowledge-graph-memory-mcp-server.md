## Overview

The Knowledge Graph Memory MCP Server is an official Anthropic implementation that provides persistent memory using a local knowledge graph. It enables AI models like Claude to remember information about users across chats, eliminating context repetition.

## Key Features

- **Persistent Storage**: Data stored locally in memory.json file on your machine
- **Full Privacy Control**: You own and control all memory data
- **Knowledge Graph Structure**: Organized as entities, relations, and observations
- **Cross-Session Memory**: Remembers information across chat sessions and client restarts
- **Cross-Tool Compatibility**: Works with any MCP-compatible client (Claude, Cursor, Goose, etc.)
- **Entity Management**: Create and track primary nodes in the knowledge graph
- **Relationship Mapping**: Define directed connections between entities
- **Observation Tracking**: Store discrete pieces of information about entities

## Knowledge Graph Components

The knowledge graph consists of three main elements:

**1. Entities**: Primary nodes in the knowledge graph representing people, projects, concepts, organizations, or any trackable subject.

**2. Relations**: Directed connections between entities stored in active voice, describing how entities interact or relate to each other (e.g., "works_for", "manages", "depends_on").

**3. Observations**: Discrete pieces of information about an entity, such as preferences, characteristics, or factual data points.

## How It Works

1. AI interacts with user and identifies important information
2. Information is structured into entities, relations, and observations
3. Data is stored in local memory.json file
4. On subsequent interactions, AI retrieves relevant memories
5. Context is automatically maintained across sessions

## Benefits

**Eliminates Context Repetition**: AI doesn't need to be re-introduced to project details, client information, or user preferences in every chat.

**Persistent Across Sessions**: Memory survives chat restarts, client restarts, and even switching between different MCP-compatible tools.

**Privacy-First Design**: All data stored locally on your machine, giving you complete control over what the AI remembers.

**Flexible Ecosystem**: Not locked to Claude—works with Cursor, Goose, and any MCP-compatible client.

## Use Cases

- **Project Memory**: Remember project structure, requirements, and decisions
- **User Preferences**: Track coding style preferences, technology choices
- **Relationship Tracking**: Map organizational structures and team relationships
- **Historical Context**: Maintain context of past conversations and decisions
- **Multi-Project Management**: Keep separate contexts for different projects
- **Learning Progress**: Track what has been explained or learned

## Memory Visualizer

Community tool available (github.com/mjherich/memory-visualizer) for interactive visualization of memory graphs, allowing you to explore, debug, and analyze entities, relations, and observations from memory.json files.

## Technical Details

- **Released**: November 19, 2024
- **Language**: TypeScript
- **Distribution**: npm package
- **Downloads**: Over 1.39M
- **Storage**: Local JSON file (memory.json)
- **License**: MIT

## Installation

Available via npm:
```bash
npx @modelcontextprotocol/server-memory
```

## Integration

Compatible with all MCP clients:

- Claude Desktop
- Claude Code
- Cursor
- Goose
- Continue
- Other MCP-compatible assistants

## Data Structure Example

```json
{
  "entities": [
    {"id": "user_1", "type": "person", "name": "John"}
  ],
  "relations": [
    {"from": "user_1", "to": "project_1", "type": "works_on"}
  ],
  "observations": [
    {"entity": "user_1", "content": "Prefers TypeScript over JavaScript"}
  ]
}
```

## Pricing

Free and open-source under the MIT License.