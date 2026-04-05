## Overview

A stdio MCP Server wrapping custom Python runtime (LocalPythonExecutor) from HuggingFace's smolagents framework. Provides safeguards while limiting operations and imports allowed inside the runtime.

## Features

- Custom Python runtime with safety safeguards
- Easy local setup without Docker or VM
- Restricted operations and imports for security
- Stdio transport mode