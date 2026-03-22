## Overview

A Model Context Protocol (MCP) server for querying Weights & Biases data including models, runs, sweeps, Weave traces, evaluations, and datasets. This integration enables AI assistants to interact with comprehensive ML experiment tracking and model management through natural language.

## Features

- **Experiment Tracking**: Query W&B runs and sweeps with powerful filtering and sorting
- **Weave Traces**: Query Weave evaluations and traces with pagination options
- **Model Management**: Access and query model registry data
- **Dataset Exploration**: Interact with W&B datasets and artifacts
- **Wandbot Integration**: Integration with wandbot support agent for assistance
- **Context Window Management**: Returns complete trace data or just metadata to avoid overwhelming LLM context

## Available Tools

- **query_wandb_tool**: Execute queries against W&B experiment tracking data including Runs & Sweeps
- **query_weave_traces_tool**: Query Weave evaluations and traces with filtering, sorting, and pagination
- Additional tools for model registry and dataset access

## Key Capabilities

- Filter and sort experiment runs by metrics, parameters, or tags
- Analyze hyperparameter sweeps and optimization results
- Track model versions and lineage
- Query trace data for LLM evaluation
- Access training artifacts and datasets
- Generate experiment summaries and reports

## Use Cases

- Conversational experiment analysis
- Hyperparameter optimization insights
- Model performance comparison
- LLM trace analysis and debugging
- Dataset exploration and validation
- Automated experiment reporting

## Integration Benefits

- Natural language access to ML experiments
- Streamlined model development workflow
- AI-assisted hyperparameter tuning
- Simplified trace analysis for LLM applications
- Comprehensive artifact management

## Supported Clients

Claude, Cursor, Windsurf, ChatGPT, and any MCP-compatible AI assistant.

## Pricing

Free tier available. W&B Pro and Enterprise plans provide additional features and scale.