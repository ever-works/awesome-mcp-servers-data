## Overview

Google Drive MCP Server provides seamless integration with Google Drive and Google Workspace, allowing AI models to search, list, read, and manage files from Google Drive, Google Docs, Google Sheets, and Google Slides through the Model Context Protocol.

## Key Features

- **File Search**: Full-text search capabilities across Google Drive
- **File Listing**: Browse and list files and folders
- **File Reading**: Access content from Drive files
- **Google Docs**: Create, edit, and read Google Docs
- **Google Sheets**: Read and write to Google Sheets, manipulate data
- **Google Slides**: Access and manage presentation files
- **Google Calendar**: Integration with calendar events and scheduling
- **OAuth 2.0 Authentication**: Secure access with Google OAuth
- **File Management**: Create, update, delete, rename, move, copy files
- **Upload/Download**: Transfer files to and from Google Drive
- **Folder Operations**: Create and manage folder structures
- **Sharing**: Manage file permissions and sharing settings

## Available Implementations

**1. felores/gdrive-mcp-server** (Efficient Implementation)
- Full-text search capabilities
- Read-only access focus
- OAuth 2.0 authentication
- Optimized for performance
- MIT License

**2. a-bonus/google-docs-mcp** (Ultimate Integration)
- Google Docs support
- Google Sheets integration
- Google Drive file management
- Comprehensive document editing

**3. isaacphi/mcp-gdrive** (Sheet-Focused)
- Listing and reading files
- Searching Drive content
- Reading and writing Google Sheets
- Specialized spreadsheet operations

**4. piotr-agier/google-drive-mcp** (Comprehensive Suite)
- Google Drive, Docs, Sheets, Slides, Calendar
- Full CRUD operations
- File upload and download
- Advanced file management

**5. Official Anthropic Google Drive MCP**
- Reference implementation
- Part of official MCP servers
- Core functionality

**6. Composio Google Drive MCP**
- AI agent tools integration
- Enterprise features
- Advanced automation

## Core Capabilities

**File Operations:**
- Search files by name, content, or metadata
- List files in folders
- Read file contents
- Create new files
- Update existing files
- Delete files
- Rename files
- Move files between folders
- Copy files

**Folder Management:**
- Create folders
- List folder contents
- Move folders
- Rename folders
- Delete folders
- Navigate folder hierarchy

**Google Docs:**
- Create new documents
- Read document content
- Edit document text
- Format text (bold, italic, headings)
- Insert images and tables
- Manage document structure

**Google Sheets:**
- Read spreadsheet data
- Write to cells
- Update ranges
- Add/remove sheets
- Format cells
- Calculate formulas
- Export data

**Google Slides:**
- Read presentation content
- Access slide text
- View slide structure
- Export presentations

**Google Calendar:**
- List calendar events
- Create events
- Update events
- Delete events
- Check availability

## Use Cases

- **Document Management**: Organize and search through Drive files
- **Content Creation**: Generate Google Docs from AI conversations
- **Data Analysis**: Read and analyze Google Sheets data
- **Report Generation**: Create formatted documents and spreadsheets
- **Meeting Notes**: Auto-generate meeting notes in Google Docs
- **Calendar Management**: Schedule meetings and manage events
- **File Search**: Find files across Drive using natural language
- **Collaboration**: Manage sharing and permissions
- **Backup**: Create copies of important documents

## Authentication Setup

**Requirements:**
1. Google Cloud Project
2. Enable Google Drive API
3. Enable Google Docs/Sheets/Slides APIs (as needed)
4. Create OAuth 2.0 credentials
5. Configure OAuth consent screen
6. Download credentials JSON

**OAuth Scopes:**
- https://www.googleapis.com/auth/drive (full access)
- https://www.googleapis.com/auth/drive.readonly (read-only)
- https://www.googleapis.com/auth/drive.file (created files only)
- https://www.googleapis.com/auth/documents (Google Docs)
- https://www.googleapis.com/auth/spreadsheets (Google Sheets)
- https://www.googleapis.com/auth/presentations (Google Slides)
- https://www.googleapis.com/auth/calendar (Google Calendar)

## Natural Language Examples

"Search for all PDFs about machine learning"
"Create a new Google Doc called 'Project Plan'"
"Read the contents of my weekly report spreadsheet"
"List all files in the 'Projects' folder"
"Update cell A1 in my budget spreadsheet to 5000"
"Find documents modified last week"
"Create a calendar event for tomorrow at 2 PM"

## File Type Support

**Google Workspace Formats:**
- Google Docs (.gdoc)
- Google Sheets (.gsheet)
- Google Slides (.gslides)
- Google Forms (.gform)
- Google Drawings (.gdraw)

**Standard Formats:**
- PDF (.pdf)
- Microsoft Word (.docx)
- Microsoft Excel (.xlsx)
- Microsoft PowerPoint (.pptx)
- Text files (.txt)
- Images (.jpg, .png, .gif)
- And many more

## Security Features

- OAuth 2.0 authentication flow
- Scoped API access
- Token refresh handling
- Secure credential storage
- Permission-based access
- No plaintext password storage

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- ChatGPT (with MCP support)
- Continue
- Other MCP-compatible AI assistants

## Rate Limits

Subject to Google Drive API quotas:

- 20,000 queries per 100 seconds per project
- 1,000 queries per 100 seconds per user
- Handle rate limit errors gracefully
- Implement exponential backoff

## Installation

**Via npm:**
```bash
npm install gdrive-mcp-server
```

**Via npx:**
```bash
npx gdrive-mcp-server
```

## Configuration

Typical configuration includes:

- Google Cloud Project ID
- OAuth 2.0 Client ID
- OAuth 2.0 Client Secret
- Redirect URI
- Required OAuth scopes

## Technical Requirements

- Google account
- Google Cloud Project
- Enabled Google Drive API
- OAuth 2.0 credentials
- Network access to Google APIs

## Performance Optimization

- Use selective field filters to reduce payload
- Implement caching for frequently accessed files
- Batch requests when possible
- Use partial responses
- Leverage ETags for change detection

## Pricing

Free and open-source MCP server implementations (MIT License). Google Drive storage and API usage subject to Google Workspace pricing tier.