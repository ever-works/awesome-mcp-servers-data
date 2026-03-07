## Overview

Starting with version 2025.2, IntelliJ IDEA and all JetBrains IDEs come with an integrated MCP server, allowing external AI clients such as Claude Desktop, Cursor, VS Code, and others to access powerful IDE tools. The standalone repository is no longer maintained as functionality is now built into the IDEs.

## Features

- **File analysis**: Analyzes files for errors and warnings using IntelliJ inspections, identifying coding issues, syntax errors, and other problems with severity, description, and location information
- **Symbol information**: Retrieves information about symbols at specified positions, providing the same information as IntelliJ IDEA's Quick Documentation feature
- **Refactoring**: Performs rename refactoring for variables, functions, classes, and other symbols as a context-aware utility that understands code structure
- **Project metadata**: Retrieves dependencies, modules, and run configurations from the project
- **Command execution**: Executes terminal commands or run configurations in the IDE without prompting for user confirmation each time
- **Code intelligence**: Leverages IntelliJ's powerful code analysis and indexing capabilities
- **Multi-language support**: Works with all languages supported by JetBrains IDEs

## Supported IDEs

- IntelliJ IDEA
- PyCharm
- WebStorm
- Android Studio
- PhpStorm
- GoLand
- Rider
- CLion
- All other JetBrains IDEs version 2025.2+

## Setup and Configuration

Configuration is automatic through IDE settings:

1. Go to Settings | Tools | MCP Server
2. Click Enable MCP Server
3. In the Clients Auto-Configuration section, click Auto-Configure for each external client (Claude Code, Claude Desktop, Cursor, VS Code, Codex, Windsurf)

## Transport Support

Supports SSE and JVM-based proxy for STDIO communication, eliminating the need for the NPM package previously required.

## Use Cases

- AI-powered code analysis and error detection
- Intelligent refactoring assistance
- Quick documentation lookup during development
- Project structure exploration
- Automated code quality checks
- Cross-file symbol analysis

## Pricing

Included with JetBrains IDE subscriptions. Free for open-source projects and educational use.