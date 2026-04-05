## Overview

WorkOS AuthKit acts as a spec-compliant OAuth 2.1 authorization server for MCP. The MCP server acts as the Resource Server; AuthKit handles authorization, token issuance, consent screens, and client registration.

## Features

- **SSO-Integrated Access**: IT teams can manage MCP access through existing identity providers
- **OAuth 2.1 Compliance**: Scoped tokens, PKCE, and consent flows following the MCP specification
- **Client Registration Support**: Both Client ID Metadata Documents (CIMD, current spec default) and Dynamic Client Registration (DCR, for backwards compatibility)
- **Minimal Integration**: Point server's protected resource metadata at an AuthKit domain and verify JWTs on incoming requests

## Deployment Options

- **AuthKit**: Full authorization server handling OAuth flows, consent, and token issuance
- **Standalone Connect**: Runs as middleware for MCP OAuth flows without requiring a migration. Users authenticate with your existing system; AuthKit handles only the OAuth authorization and token issuance that MCP clients need

## Pricing

See WorkOS pricing documentation for details.