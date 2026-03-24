## Overview

ImageMagick Conversion MCP provides tools for converting DNG (Digital Negative) RAW image files to WebP format using either ImageMagick or darktable as the conversion backend. It implements the MCP protocol over stdio transport, making it compatible with MCP clients like Claude Desktop.

## Features

- **DNG to WebP Conversion**: Convert RAW camera files to modern WebP format
- **Lossless Compression**: Maintain image quality with efficient compression
- **Automatic Fallback**: Falls back to darktable if ImageMagick conversion fails
- **Dual Backend Support**: Choose between ImageMagick and darktable processing
- **Batch Processing**: Convert multiple images efficiently
- **Quality Control**: Configurable compression settings
- **Metadata Preservation**: Retain EXIF and other image metadata
- **Format Flexibility**: Support for various input and output formats

## Supported Operations

- RAW image conversion (DNG, CR2, NEF, ARW)
- Format conversion (JPEG, PNG, WebP, TIFF)
- Image resizing and scaling
- Color space conversion
- Batch image processing
- Thumbnail generation

## Use Cases

- Convert camera RAW files for web publishing
- Optimize images for web performance
- Batch process photography collections
- Prepare images for AI model training
- Create web-optimized image galleries
- Automate photography workflows

## Requirements

- ImageMagick installed on system
- Optional: darktable for enhanced RAW processing

## Pricing

Free and open-source under the MIT license. ImageMagick and darktable are also free.