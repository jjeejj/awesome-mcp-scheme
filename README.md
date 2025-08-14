# Awesome MCP Scheme

A collection of Model Context Protocol (MCP) service configurations for quick setup and deployment of various MCP services.

[中文文档](./README-zh.md)

## Table of Contents

- [Available Services](#available-services)
- [Configuration Guide](#configuration-guide)
- [How to Use](#how-to-use)
- [How to Contribute](#how-to-contribute)

## Available Services

### Filesystem

- [Server Filesystem](https://github.com/modelcontextprotocol/server-filesystem) - A server filesystem service that provides file system access capabilities

### Productivity

- [Notion](https://github.com/makenotion/notion-mcp-server) - Connect to Notion workspace for reading and writing pages, databases, and blocks
- [Google Workspace](https://github.com/taylorwilsdon/google_workspace_mcp) - For reading and writing Google documents, spreadsheets, and presentations

### Communication

- [Slack](https://github.com/korotovsky/slack-mcp-server) - A powerful Slack MCP server with multiple transport methods, DMs, and smart history fetch logic

### Analytics

- [Google Analytics](https://github.com/surendranb/google-analytics-mcp) - Connect to Google Analytics for reading and writing events, user properties, and metrics

### Automation

- [Chrome Automation](https://github.com/JackZhao98/chrome-automation-mcp) - Chrome Automation MCP powered by Playwright

## 配置说明

每个服务的配置遵循以下格式：

\`\`\`json
{
"id": "服务唯一标识",
"name": "服务名称",
"category": "服务类别",
"description": "服务描述",
"author": "作者",
"tags": ["标签 1", "标签 2"],
"config": [
{
"key": "配置键",
"value": "配置值",
"is_user_fill": "是否需要用户填写",
"fill_fields": [
{
"input_type": "输入类型",
"out_type": "输出类型",
"replace_placehold": "替换占位符",
"desc": "描述",
"doc": "文档链接",
"placeholder": "示例值"
}
]
}
]
}
\`\`\`

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
