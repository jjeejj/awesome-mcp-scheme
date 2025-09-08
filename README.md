# Awesome MCP Scheme

A collection of Model Context Protocol (MCP) service configurations for quick setup and deployment of various MCP services.

[中文文档](./README-zh.md)

## Table of Contents

- [Awesome MCP Scheme](#awesome-mcp-scheme)
  - [Table of Contents](#table-of-contents)
  - [Available Services](#available-services)
    - [Filesystem](#filesystem)
    - [Productivity](#productivity)
    - [Communication](#communication)
    - [Analytics](#analytics)
    - [Automation](#automation)
    - [Design](#design)
    - [Deployment](#deployment)
    - [Monitoring](#monitoring)
    - [Database](#database)
    - [Payment](#payment)
    - [Network](#network)
    - [Utilities](#utilities)
    - [Visualization](#visualization)
  - [Configuration Guide](#configuration-guide)
  - [How to Use](#how-to-use)
  - [How to Contribute](#how-to-contribute)
  - [Schema Validation](#schema-validation)
  - [License](#license)

## Available Services

### Filesystem

- [Server Filesystem](https://www.npmjs.com/package/@modelcontextprotocol/server-filesystem) - A server filesystem service that provides file system access capabilities

### Productivity

- [Notion](https://github.com/makenotion/notion-mcp-server) - Connect to Notion workspace for reading and writing pages, databases, and blocks
- [Google Workspace](https://github.com/taylorwilsdon/google_workspace_mcp) - For reading and writing Google documents, spreadsheets, and presentations
- [WordPress MCP](https://github.com/Automattic/wordpress-mcp) - A Model Context Protocol server for interacting with WordPress sites

### Communication

- [Slack](https://github.com/korotovsky/slack-mcp-server/) - A powerful Slack MCP server with multiple transport methods, DMs, and smart history fetch logic
- [Zoom MCP Server](https://github.com/javaprogrammerlb/zoom-mcp-server) - A Model Context Protocol server for interacting with Zoom
- [Calendly](https://github.com/meAmitPatil/calendly-mcp-server) - A Model Context Protocol server for integrating with Calendly scheduling platform

### Analytics

- [Google Analytics](https://github.com/surendranb/google-analytics-mcp) - Connect to Google Analytics for reading and writing events, user properties, and metrics

### Automation

- [Chrome Automation](https://github.com/JackZhao98/chrome-automation-mcp) - Chrome Automation MCP powered by Playwright

### Design

- [Framelink Figma MCP](https://github.com/GLips/Figma-Context-MCP) - A Model Context Protocol server for interacting with Figma

### Deployment

- [Netlify MCP](https://github.com/netlify/netlify-mcp) - A Model Context Protocol server for interacting with Netlify

### Monitoring

- [Sentry](https://github.com/getsentry/sentry-mcp) - A Model Context Protocol server for interacting with Sentry

### Database

- [Redis](https://github.com/redis/mcp-redis) - A Model Context Protocol server for interacting with Redis

### Payment

- [Stripe MCP](https://docs.stripe.com/mcp) - A Model Context Protocol server for interacting with Stripe

### Network

- [IPinfo Geolocation](https://github.com/briandconnelly/mcp-server-ipinfo) - A Model Context Protocol server for IP address geolocation

### Utilities

- [Time Server](https://github.com/modelcontextprotocol/servers/tree/main/src/time) - A Model Context Protocol server that provides current time information. Allows AI agents to access real-time information for time-based operations and scheduling

### Visualization

- [MCP ECharts](https://github.com/hustcc/mcp-echarts) - Generate visual charts using ECharts with AI MCP dynamically for chart generation and data analysis

## Configuration Guide

Each service configuration follows this format:

```json
{
  "id": "service-identifier",
  "name": "Service Name",
  "category": "Service Category",
  "description": "Service Description",
  "long_description": "Long Description"
  "author": "Author",
  "tags": ["tag1", "tag2"],
  "homepage": "https://example.com",
  "icon": "https://example.com/icon.png"
  "prerequisites": [],
  "config": [
    {
      "key": "config-key",
      "value": "config-value",
      "is_user_fill": "whether-user-input-required",
      "fill_fields": [
        {
          "input_type": "input-type",
          "out_type": "output-type",
          "replace_placehold": "placeholder-to-replace",
          "desc": "description",
          "doc": "documentation-url",
          "placeholder": "example-value"
        }
      ]
    }
  ]
}
```

## How to Use

1. Choose your desired service configuration
2. Fill in the necessary parameters in the `config` section
3. Use the MCP client to load the configuration and start the service

## How to Contribute

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Schema Validation

All service configurations must comply with the format defined in [schema.json](./schema.json). You can use this schema to validate your configurations.

## License

MIT License - see the [LICENSE](./LICENSE) file for details
