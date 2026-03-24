## Overview

RSS Crawler MCP Server is an advanced RSS feed management system that fetches, parses, and stores RSS feeds in a SQLite database. It enables seamless news and article retrieval for language models through filtering, searching, and Firecrawl-powered article access.

## Features

- **SQLite Storage**: Persistent storage of RSS feed data in SQLite database
- **Automated Crawling**: Scheduled fetching and parsing of RSS feeds
- **Advanced Filtering**: Filter articles by date, source, keywords, and categories
- **Full-text Search**: Search across all stored articles efficiently
- **Firecrawl Integration**: Enhanced article extraction using Firecrawl
- **Feed Management**: Add, remove, and update RSS feed sources
- **Deduplication**: Automatically detect and handle duplicate articles
- **Performance Optimization**: Efficient database queries for fast retrieval

## Technical Features

- Incremental updates to minimize bandwidth usage
- Configurable crawl intervals
- Support for RSS 2.0 and Atom feeds
- Article metadata extraction (author, publication date, tags)
- Image and media URL extraction
- Feed health monitoring

## Use Cases

- Build custom news aggregation systems
- Create searchable article databases for AI analysis
- Monitor multiple news sources from a single interface
- Perform historical analysis of news trends
- Generate automated news summaries and digests

## Pricing

Free and open-source. Firecrawl integration may require separate API subscription.