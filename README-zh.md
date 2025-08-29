# Awesome MCP Scheme

这个仓库收集了一系列 Model Context Protocol (MCP) 的服务配置方案，用于快速配置和部署各种 MCP 服务。

[English](./README.md)

## 目录

- [可用服务](#可用服务)
  - [文件系统](#文件系统)
  - [生产力工具](#生产力工具)
  - [通信](#通信)
  - [分析](#分析)
  - [自动化](#自动化)
  - [部署](#部署)
  - [监控](#监控)
  - [数据库](#数据库)
  - [支付](#支付)
  - [CRM](#crm)
  - [网络](#网络)
  - [实用工具](#实用工具)
- [配置说明](#配置说明)
- [如何使用](#如何使用)
- [如何贡献](#如何贡献)

## 可用服务

### 文件系统

- [Server Filesystem](https://github.com/modelcontextprotocol/server-filesystem) - 提供文件系统访问能力的服务

### 生产力工具

- [Notion](https://github.com/makenotion/notion-mcp-server) - 连接 Notion 工作区，用于读写页面、数据库和块
- [Google Workspace](https://github.com/taylorwilsdon/google_workspace_mcp) - 用于读写 Google 文档、表格和演示文稿

### 通信

- [Slack](https://github.com/korotovsky/slack-mcp-server) - 功能强大的 Slack MCP 服务器，支持多种传输方式、DMs 和智能历史记录获取
- [Calendly](https://github.com/meAmitPatil/calendly-mcp-server) - 用于与 Calendly 预约平台集成的模型上下文协议服务器

### 分析

- [Google Analytics](https://github.com/surendranb/google-analytics-mcp) - 连接 Google Analytics，用于读写事件、用户属性和自定义维度指标

### 自动化

- [Chrome Automation](https://github.com/JackZhao98/chrome-automation-mcp) - 基于 Playwright 的 Chrome 自动化 MCP 服务

### 部署

- [Netlify MCP](https://github.com/netlify/netlify-mcp) - 用于与 Netlify 部署平台集成的模型上下文协议服务器

### 监控

- [Sentry](https://github.com/getsentry/sentry-mcp) - 用于与 Sentry 错误跟踪平台集成的模型上下文协议服务器

### 数据库

- [Redis](https://github.com/redis/mcp-redis) - 官方 Redis MCP 服务器，为智能代理应用设计的自然语言接口，可高效地管理和搜索 Redis 中的数据

### 支付

- [Stripe MCP](https://docs.stripe.com/mcp) - 让 AI 代理与 Stripe API 交互。包括管理客户、产品、价格、发票、支付等工具。

### CRM

- [HubSpot MCP Server](https://www.npmjs.com/package/@hubspot/mcp-server) - HubSpot 的 MCP 服务器，使 AI 客户端能够无缝执行 HubSpot 操作并与您的 HubSpot 数据交互

### 网络

- [IPinfo Geolocation](https://github.com/briandconnelly/mcp-server-ipinfo) - 使用 ipinfo.io API 获取 IP 地址详细信息的模型上下文协议服务器

### 实用工具

- [Time Server](https://github.com/modelcontextprotocol/servers/tree/main/src/time) - 提供当前时间信息的模型上下文协议服务器

## 配置说明

每个服务的配置遵循以下格式：

```json
{
  "id": "服务唯一标识",
  "name": "服务名称",
  "category": "服务类别",
  "description": "服务描述",
  "author": "作者",
  "tags": ["标签1", "标签2"],
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
```

## 如何使用

1. 选择你需要的服务配置
2. 根据服务的 `config` 配置填写必要的参数
3. 使用 MCP 客户端加载配置并启动服务

## 如何贡献

1. Fork 这个仓库
2. 创建你的功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开一个 Pull Request

## Schema 验证

所有的服务配置都需要符合 [schema.json](./schema.json) 定义的格式。你可以使用这个 schema 来验证你的配置是否正确。

## 许可证

MIT License - 详见 [LICENSE](./LICENSE) 文件
