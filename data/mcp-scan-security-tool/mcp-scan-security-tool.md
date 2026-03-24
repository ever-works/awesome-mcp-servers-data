## Overview

mcp-scan is a security tool designed to scan MCP servers for vulnerabilities, detect tool poisoning, and provide continuous security monitoring. It addresses the growing security concerns around the Model Context Protocol ecosystem, where over 30 CVEs have been discovered in 60 days.

## Features

- **Vulnerability Scanning**: Scan all installed MCP servers for known security issues
- **Tool Definition Pinning**: Pin tool definitions to detect unauthorized changes
- **Change Detection**: Automatically identify modifications to tool schemas and behaviors
- **Continuous Monitoring**: Run in proxy mode for real-time security monitoring
- **CVE Database**: Access to comprehensive CVE database for MCP servers
- **Tool Poisoning Detection**: Identify compromised tools, plugins, or dependencies
- **Security Reporting**: Generate detailed security audit reports
- **Compliance Checking**: Verify servers against OWASP MCP Top 10 guidelines

## Usage

```bash
# Scan all installed MCP servers
uvx mcp-scan

# Pin tool definitions and detect changes
uvx mcp-scan --pin

# Continuous monitoring via proxy
uvx mcp-scan proxy
```

## Security Concerns Addressed

- **Command Injection**: Detect servers vulnerable to command injection attacks
- **Path Traversal**: Identify file system access vulnerabilities
- **SSRF**: Find Server-Side Request Forgery vulnerabilities
- **Hard-coded Credentials**: Locate exposed secrets and API keys
- **Tool Interference**: Detect malicious tool interactions
- **Memory Poisoning**: Identify compromised model memory
- **Prompt Injection**: Find prompt injection vulnerabilities

## OWASP MCP Top 10

Based on the OWASP MCP Top 10 project, which catalogs the most critical MCP security risks including:
1. Model Misbinding
2. Context Spoofing
3. Prompt-State Manipulation
4. Insecure Memory References
5. Covert Channel Abuse
6. Tool Poisoning
7. Excessive Permissions
8. Inadequate Input Validation
9. Authentication Bypass
10. Supply Chain Compromise

## Use Cases

- Scan MCP servers before deployment to production
- Monitor production MCP servers for security changes
- Audit third-party MCP servers for vulnerabilities
- Implement continuous security scanning in CI/CD pipelines
- Generate security compliance reports for audits

## Pricing

Free and open-source as part of the OWASP project.