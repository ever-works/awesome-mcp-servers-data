## Overview

MinIO is previewing an MCP server that enables interaction with and management of MinIO AIStor, their commercial object-store offering, through natural language conversations with LLMs such as Anthropic Claude or OpenAI ChatGPT. This implementation makes exploring and using data in an AIStor object store easier than ever.

## Features

- **25+ Tools**: Comprehensive toolset for object storage operations
- **Bucket Management**: List, create, remove, and check bucket existence
- **Object Operations**: Upload, download, copy, delete objects
- **Presigned URLs**: Generate presigned URLs for secure temporary access
- **Content Retrieval**: Support for both text and binary files
- **Administrative Functions**: Core commands like list buckets, get object tags, get bucket transition rules
- **Conversational Interface**: Natural language interaction with object storage clusters

## Core Tools

The server exposes four core tools:
- ListBuckets: List all buckets in the storage cluster
- ListObjects: List objects within a bucket
- GetObject: Retrieve object contents
- PutObject: Upload objects to storage

## Technical Implementation

Built using Go (production version) and TypeScript with the MCP SDK. Provides a secure and standardized way for LLMs to interface with S3-compatible storage.

## Use Cases

Administrators can perform tasks like:
- Review bucket contents through conversation
- Analyze objects and tag them for future processing
- Manage object storage infrastructure using human-language commands
- Integrate object storage operations into AI-powered workflows

## Compatibility

Works with S3-compatible APIs and MinIO object storage. Compatible with Claude, ChatGPT, and other MCP-enabled AI assistants.

## Pricing

MCP server is in preview. MinIO AIStor pricing applies separately for the object storage service.