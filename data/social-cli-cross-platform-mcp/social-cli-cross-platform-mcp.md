## Overview

Social CLI Cross-Platform MCP is a command-line tool and MCP server for posting to multiple social media platforms including Twitter/X, Reddit, LinkedIn, and Instagram from your terminal or via AI agents. It provides a unified posting interface with streamlined authentication management.

## Features

- **CLI Interface**: Post from terminal with simple commands
- **MCP Integration**: Use with AI assistants for automated posting
- **Multi-Platform**: Support for Twitter/X, Reddit, LinkedIn, Instagram
- **Unified API**: Consistent interface across all platforms
- **Authentication Management**: Secure credential storage
- **Template Support**: Reusable post templates
- **Media Uploads**: Support for images and videos
- **Draft Management**: Save and edit drafts

## Supported Platforms

### Twitter/X
- Post tweets
- Add images and videos
- Thread creation
- Hashtag support

### Reddit
- Submit posts to subreddits
- Text and link posts
- Image and video posts
- Flair selection

### LinkedIn
- Post to personal profile
- Company page posting
- Article sharing
- Media attachments

### Instagram
- Photo posting
- Video posting
- Caption and hashtags
- Location tagging

## CLI Commands

```bash
# Post to single platform
social-cli post twitter "Your tweet text"

# Post to multiple platforms
social-cli post --all "Universal message"

# Post with image
social-cli post instagram "Caption" --image photo.jpg

# Create draft
social-cli draft create "Draft content"
```

## MCP Features

- Natural language post creation
- AI-assisted content optimization
- Scheduled posting through AI
- Platform-specific formatting
- Automatic hashtag suggestions

## Authentication

- OAuth for supported platforms
- API key management
- Secure credential storage
- Multi-account support
- Token refresh handling

## Use Cases

- Cross-post content from terminal
- Automate social media updates
- Script social media workflows
- Integrate with CI/CD pipelines
- Build custom posting tools
- Schedule posts via cron jobs

## Configuration

Simple YAML or JSON configuration:
```yaml
platforms:
  twitter:
    api_key: xxx
  reddit:
    client_id: xxx
```

## Pricing

Free and open-source under the MIT license.