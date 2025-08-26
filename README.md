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
    - [Deployment](#deployment)
    - [Monitoring](#monitoring)
    - [Database](#database)
    - [Payment](#payment)
  - [Configuration Guide](#configuration-guide)
  - [How to Use](#how-to-use)
  - [How to Contribute](#how-to-contribute)
  - [Schema Validation](#schema-validation)
  - [License](#license)

## Available Services

### Filesystem

- [Server Filesystem](https://github.com/modelcontextprotocol/server-filesystem) - A server filesystem service that provides file system access capabilities

### Productivity

- [Notion](https://github.com/makenotion/notion-mcp-server) - Connect to Notion workspace for reading and writing pages, databases, and blocks
- [Google Workspace](https://github.com/taylorwilsdon/google_workspace_mcp) - For reading and writing Google documents, spreadsheets, and presentations

### Communication

- [Slack](https://github.com/korotovsky/slack-mcp-server) - A powerful Slack MCP server with multiple transport methods, DMs, and smart history fetch logic
- [Calendly](https://github.com/meAmitPatil/calendly-mcp-serve) - A Model Context Protocol server for integrating with Calendly scheduling platform

### Analytics

- [Google Analytics](https://github.com/surendranb/google-analytics-mcp) - Connect to Google Analytics for reading and writing events, user properties, and metrics

### Automation

- [Chrome Automation](https://github.com/JackZhao98/chrome-automation-mcp) - Chrome Automation MCP powered by Playwright

### Deployment

- [Netlify MCP](https://github.com/netlify/netlify-mcp) - A Model Context Protocol server for integrating with Netlify deployment platform

### Monitoring

- [Sentry](https://github.com/getsentry/sentry-mcp) - A Model Context Protocol server for integrating with Sentry error tracking platform

### Database

- [Redis](https://github.com/redis/mcp-redis) - The official Redis MCP Server is a natural language interface designed for agentic applications to manage and search data in Redis efficiently

### Payment

- [Stripe MCP](https://docs.stripe.com/mcp) - Let your AI agents interact with the Stripe API. Includes tools for managing customers, products, prices, invoices, payments and more.

## Configuration Guide

Each service configuration follows this format:

```json
{
  "id": "service-identifier",
  "name": "Service Name",
  "category": "Service Category",
  "description": "Service Description",
  "author": "Author",
  "tags": ["tag1", "tag2"],
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
