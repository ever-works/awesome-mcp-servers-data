## Overview

LaunchDarkly provides three hosted MCP servers, each focused on a different product area: feature management for managing feature flags, AI Configs for managing AI configurations and variations, and observability for querying logs, traces, errors, and dashboards. Create, evaluate, and modify feature flags from within your IDE using natural language.

## Features

### Feature Management Server
- **create-flag**: Create new feature flags in a project (defaults to boolean temporary flag, OFF in all environments)
- **get-flag**: Get detailed configuration for a single feature flag scoped to a specific environment
- **list-flags**: Search and browse feature flags in a project
- **toggle-flag**: Turn a feature flag's targeting on or off in a specific environment

### AI Configs Server
- Manage AI model configurations and variations
- Control AI feature rollouts and experiments
- Test different AI model settings across environments

### Observability Server
- Query logs, traces, and error data
- Access dashboards and metrics
- Monitor feature flag usage and performance

## Use Cases

### Progressive Deployment
- Gradually roll out features to subsets of users
- Control feature availability by environment
- Manage percentage-based rollouts

### A/B Testing & Experimentation
- Configure multivariate tests
- Track experiment performance
- Analyze feature impact on key metrics

### Risk Mitigation
- Instantly disable problematic features
- Test in production with controlled exposure
- Separate deployment from release

### Environment Management
- Manage flags across dev, staging, and production
- Configure different targeting rules per environment
- Synchronize flag states across teams

## Integration

Works with any AI client supporting MCP including Cursor, Windsurf, Claude Desktop, and Raycast. Supports both interactive login via Device Authorization Grant and automated login via Private Key JWT.

## Pricing

Free tier available with usage-based pricing for advanced features. Enterprise plans include dedicated support and custom integrations.