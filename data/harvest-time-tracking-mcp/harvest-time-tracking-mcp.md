## Overview

Harvest Time Tracking MCP provides integration with the Harvest time tracking and project management API, allowing Claude and other MCP-compatible AI assistants to interact with your Harvest account. It helps manage time entries, projects, clients, and more through natural language conversations.

## Features

- **Time Entry Management**: Create, update, and delete time entries
- **Timer Controls**: Start and stop timers with natural language commands
- **Project Management**: List and manage projects and tasks
- **Client Management**: Access and organize client information
- **User Information**: Retrieve current user details and permissions
- **Time Range Queries**: List time entries for specific date ranges
- **Flexible Entry Creation**: Create entries via duration or start/end times
- **Detailed Retrieval**: Get comprehensive information about specific entries

## API Tools Provided

- `get_current_user` - Retrieve authenticated user information
- `list_time_entries` - Query time entries with filters
- `get_time_entry` - Get detailed information about a specific entry
- `create_time_entry` - Create new time entries with project and task assignment
- `create_time_entry_via_start_end` - Create entries using start and end times
- `update_time_entry` - Modify existing time entries
- `delete_time_entry` - Remove time entries

## Use Cases

- Log work hours through AI conversations
- Generate timesheet reports via natural language queries
- Manage project time allocation efficiently
- Track billable and non-billable hours automatically
- Analyze time spent across projects and clients
- Automate time entry creation from calendar events

## Pricing

Free and open-source under the MIT license. Requires Harvest account (14-day free trial, then paid plans).