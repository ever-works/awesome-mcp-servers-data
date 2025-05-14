# strava-mcp

A Model Context Protocol (MCP) server for connecting to the Strava API, providing access to sports and activity data for AI-driven analysis via the MCP protocol. It is written in TypeScript and primarily intended to expose Strava data and functionalities as "tools" that Large Language Models (LLMs) can utilize through the MCP standard.

**Source:** [https://github.com/r-huijts/strava-mcp](https://github.com/r-huijts/strava-mcp)

**Category:** data-access-integration-mcp-servers

**Tags:** mcp, strava, sports, api-integration, data-access

---

## Features
- **MCP Server for Strava:** Acts as a bridge between the Strava API and clients using the MCP protocol, enabling seamless integration with LLMs.
- **Natural Language Interaction:** Designed for AI assistants to answer natural language queries about Strava data.
- **Comprehensive Strava Data Access:**
  - Recent activities and athlete profile
  - Activity streams and detailed activity data
  - Athlete statistics (recent, YTD, all-time)
  - Specific activity details by ID
  - Club membership list
  - Starred segments and segment details
  - Segment exploration (search by area)
  - Star/unstar segments
  - Segment efforts and effort lists (with date filtering)
  - Athlete routes and route details
  - Export routes in GPX or TCX format
  - Activity streams (detailed time-series data)
  - Activity laps (lap-by-lap breakdown)
  - Athlete heart rate and power zones
- **Authentication Handling:**
  - Supports Strava OAuth authentication flow
  - Automatic access token refreshing with updates to environment variables
- **Configuration:**
  - Supports environment variable config for Strava credentials and export path
- **Export Functionality:**
  - Ability to export routes to local files in GPX/TCX formats
- **Installation & Setup:**
  - Step-by-step setup instructions for integrating with Claude Desktop and Strava API
- **Extensible:**
  - Open source and welcoming to contributions
- **License:** MIT License

## Pricing
No pricing information provided (open-source project).

---

**Note:** For integration, proper setup of Strava API credentials and configuration of environment variables is required. The project supports seamless operation by handling token refreshes automatically.