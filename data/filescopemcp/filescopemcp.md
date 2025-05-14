# FileScopeMCP

[GitHub Repository](https://github.com/admica/FileScopeMCP)

## Overview
FileScopeMCP is an open-source Model Context Protocol (MCP) server for codebase analysis. It identifies important files based on dependency relationships, generates visual diagrams, and provides importance scores to help AI assistants and developers understand the structure of a software project. It supports several popular programming languages and stores all analysis data in JSON format for persistence and reuse.

## Features
- **File Importance Analysis**
  - Ranks files on a 0-10 scale based on their role in the codebase.
  - Calculates importance using incoming/outgoing dependencies, file type, location, and naming significance.
  - Instantly pinpoints the most critical files in your project.
- **Dependency Tracking**
  - Maps bidirectional dependency relationships between files.
  - Identifies which files import or are imported by a given file.
  - Distinguishes between local and package dependencies.
  - Multi-language support: Python, JavaScript, TypeScript, C, C++, Rust, Lua, and Zig.
- **Visualization**
  - Generates Mermaid diagrams to visualize file relationships.
  - Color-coded visualization based on importance scores.
  - Supports dependency graphs, directory trees, and hybrid views.
  - Output in Mermaid text (.mmd) or HTML with client-side rendering, theme toggle, and responsive design.
  - Customizable diagram depth, filtering, and layout options.
- **File Summaries**
  - Allows human or AI-generated summaries to be attached to any file.
  - Summaries persist across server restarts.
- **Multiple Project Support**
  - Manage multiple file trees for different project areas.
  - Separate configurations for distinct base directories.
  - Cached trees for faster operation.
- **Persistent Storage**
  - All data stored in JSON files, including configuration metadata, dependency trees, importance scores, and summaries.
- **Cross-Platform Compatibility**
  - Handles Windows and Unix path formats, absolute/relative paths, and URL-encoded paths.
- **Caching**
  - Implements caching for faster repeated operations.
- **File Watching**
  - Toggle file watching on/off.
  - Update file watching configuration (debounce timing, auto-rebuild, new/deleted/changed file detection).
  - Get current status of file watching.
- **Available Tools (via MCP server)**
  - File tree management: list, create, select, delete trees.
  - File analysis: list files, get importance, find important files, read content, recalculate importance.
  - File summaries: get/set summaries.
  - Diagram generation: generate diagrams with different styles, formats, and layout options.

## Technical Details
- Built with TypeScript/Node.js.
- Implements the Model Context Protocol for integration with compatible tools (e.g., Cursor).
- Uses Mermaid.js for diagram generation.
- JSON-based storage for configuration and results.
- Cross-platform build scripts for Windows, Linux, and Mac.

## Supported Languages
- Python
- JavaScript
- TypeScript
- C
- C++
- Rust
- Lua
- Zig

## License
GPL-3.0 License

## Pricing
FileScopeMCP is open-source and free to use under the GPL-3.0 license.