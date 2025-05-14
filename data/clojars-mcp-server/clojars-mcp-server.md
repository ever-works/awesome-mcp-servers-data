# Clojars-MCP-Server

A Model Context Protocol (MCP) server that provides tools for fetching dependency information from Clojars, the Clojure community's artifact repository.

## Features
- Fetch the latest version of any Clojars dependency (Maven artifact)
- Check if a specific version of a Clojars dependency exists
- Provides simple, focused responses
- Easy integration with Claude and other MCP-compatible tools
- Exposes two main tools:
  - `get_clojars_latest_version`: Retrieves the latest version of a specified Clojars dependency
  - `check_clojars_version_exists`: Checks if a specific version of a dependency exists
- Supports configuration for Claude Desktop and VSCode Claude extension
- Can be run directly via `npx`, installed globally via `npm`, or manually built and configured

## Installation
- **Via npx:** `npx clojars-deps-server`
- **Global install:** `npm install -g clojars-deps-server`
- **Via Smithery:** `npx -y @smithery/cli install clojars-deps-server --client claude`
- **Manual installation:** Clone the repository, install dependencies, build, and configure in the desired client

## License
MIT License

## Source
[https://github.com/Bigsy/Clojars-MCP-Server](https://github.com/Bigsy/Clojars-MCP-Server)

## Pricing
This project is open-source and available under the MIT license. No pricing or paid plans.