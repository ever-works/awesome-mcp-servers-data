# Google Jobs (AlphaOSINT)

A hosted MCP server that lets an assistant search job postings on Google Jobs. It pins one Apify Actor, `johnvc/Google-Jobs-Scraper`, as a single typed tool, so nothing has to be installed or self-hosted.

## Connection

- Hosted endpoint: `https://mcp.apify.com/?tools=johnvc/Google-Jobs-Scraper`
- Transport: Streamable HTTP
- Authentication: Apify OAuth, or an `Authorization: Bearer <APIFY_TOKEN>` header
- Setup notes: https://github.com/johnisanerd/alphaosint-mcp-servers/tree/main/servers/google-jobs
- Actor page: https://apify.com/johnvc/Google-Jobs-Scraper

## What it can do

- Search postings by keyword and location, with an optional location radius
- Target a country, interface language or Google domain
- Limit results to jobs posted in the last 24 hours, 3 days, 7 days or 30 days
- Return company, location, source site, posting age, qualifications and benefits highlights, and apply links for each posting
- Page through results up to a set number of jobs or pages

## Pricing

Each call runs on the user's own Apify account and is billed per page of results (up to 10 jobs). Current prices are on the Actor page.
