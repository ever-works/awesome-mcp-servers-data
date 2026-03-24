## Overview

The Official Mapbox MCP Server transforms any AI agent or application into a geospatially-aware system by providing seamless access to Mapbox's comprehensive location intelligence platform. It offers a hosted endpoint for simple setup or can be self-hosted for custom deployments.

## Features

- **Global Geocoding**: Convert addresses to coordinates and vice versa worldwide
- **POI Search**: Search millions of businesses and points of interest using the Search Box Text Search API
- **Multi-modal Routing**: Calculate routes for driving, walking, cycling with real-time traffic
- **Travel Time Matrices**: Calculate travel times and distances between multiple points using Matrix API
- **Route Optimization**: Optimize routes for multiple stops and waypoints
- **Map Matching**: Snap GPS traces to the road network with support for different travel profiles
- **Isochrone Generation**: Create travel time polygons showing reachable areas
- **Static Map Images**: Generate static map images programmatically
- **Offline Calculations**: Perform geospatial calculations without API calls
- **Real-time Traffic**: Access live traffic data for accurate routing

## Installation Options

### Hosted Endpoint (Recommended)
Connect directly to Mapbox's hosted MCP endpoint at `https://mcp.mapbox.com/mcp` without installing anything locally. Simply requires a Mapbox Access Token.

### Self-hosted
Install and run locally for custom configurations and on-premises deployments.

## Use Cases

- Build location-aware AI applications
- Create intelligent routing and logistics systems
- Develop geofencing and proximity alerts
- Generate travel time analyses
- Build store locators and delivery planning tools
- Create custom map visualizations
- Implement location-based recommendations
- Analyze geographic patterns and trends

## API Coverage

- Search Box API for geocoding and POI search
- Directions API for routing
- Matrix API for travel time calculations
- Map Matching API for GPS trace alignment
- Isochrone API for reachability analysis
- Static Images API for map generation

## Pricing

Free and open-source MCP server. Mapbox services require an access token:
- **Free Tier**: Generous monthly quotas for all APIs
- **Pay-as-you-go**: Scalable pricing based on usage
- **Enterprise**: Custom pricing for high-volume applications