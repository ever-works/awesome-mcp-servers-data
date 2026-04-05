## Overview

MarkItDown is a comprehensive document conversion server that transforms various file formats into high-quality Markdown, optimized for LLM consumption and text analysis workflows. It focuses on maintaining semantic meaning and formatting valuable for both AI processing and human readability.

## Supported File Formats

- **Office Documents**: PDF, PowerPoint (PPTX), Word (DOCX), Excel (XLSX/XLS)
- **Media Files**: Images (with EXIF metadata and OCR), Audio (with EXIF metadata and speech transcription)
- **Web Content**: HTML, RSS feeds, YouTube URLs, Wikipedia pages
- **Data Formats**: CSV, JSON, XML, ZIP files (recursively processes contents)
- **Publishing Formats**: EPub, Jupyter notebooks (.ipynb)
- **Email**: Outlook messages (.msg)
- **Advanced**: Azure Document Intelligence integration for enhanced PDF processing

## Advanced Capabilities

- **LLM-Powered Image Descriptions**: Generates detailed image descriptions when provided with an OpenAI client
- **Audio Transcription**: Converts audio content to text for speech analysis
- **Azure Document Intelligence**: Enhanced PDF processing through Azure's document understanding service
- **Plugin System**: Extensible architecture for supporting additional file formats
- **Document Structure Preservation**: Maintains headings, lists, tables, links, and slide organization

## Key Use Cases

- Convert PowerPoint presentations to Markdown for documentation sites
- Extract text from PDFs with proper heading structure intact
- Transform Excel spreadsheets into readable Markdown tables
- Process speaker notes and alt text from presentations
- Convert charts to readable data tables

## Why Markdown

Markdown is extremely close to plain text with minimal markup while still representing important document structure. Mainstream LLMs natively understand Markdown and often incorporate it into responses unprompted, suggesting they have been trained on vast amounts of Markdown-formatted text. Markdown conventions are also highly token-efficient.

## Pricing

Free and open-source.