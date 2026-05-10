# Awesome MCP Servers [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> A curated list of awesome [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) servers — connect your AI to the real world.

MCP is an open protocol (now part of the [Linux Foundation](https://www.linuxfoundation.org/)) that enables AI models (Claude, ChatGPT, Cursor, Windsurf, etc.) to securely interact with external tools, databases, APIs, and services through standardized server implementations.

**[繁體中文版](#繁體中文) | English**

---

## Contents

- [Official Reference Servers](#official-reference-servers)
- [Search & Web](#search--web)
- [Browser Automation](#browser-automation)
- [Databases — Relational](#databases--relational)
- [Databases — Vector & Graph](#databases--vector--graph)
- [Cloud & Infrastructure](#cloud--infrastructure)
- [Developer Tools](#developer-tools)
- [AI & Knowledge](#ai--knowledge)
- [Productivity & Project Management](#productivity--project-management)
- [Communication & Email](#communication--email)
- [File & Storage](#file--storage)
- [Finance & Payments](#finance--payments)
- [Data & Analytics](#data--analytics)
- [CMS & Content](#cms--content)
- [CRM & Marketing](#crm--marketing)
- [Security & Identity](#security--identity)
- [DevOps & Monitoring](#devops--monitoring)
- [Automation & Workflow](#automation--workflow)
- [Smart Home & IoT](#smart-home--iot)
- [Media & Entertainment](#media--entertainment)
- [Frameworks & SDKs](#frameworks--sdks)
- [Resources](#resources)
- [Quick Start](#quick-start)
- [How to Choose](#how-to-choose)
- [繁體中文](#繁體中文)

---

## Official Reference Servers

> Maintained by the [MCP team](https://github.com/modelcontextprotocol/servers). These are the canonical implementations.

| Name | Description | Install |
|------|-------------|---------|
| [Filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) | Secure file operations with configurable access controls | `npx -y @modelcontextprotocol/server-filesystem /path` |
| [Fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) | Web content fetching and conversion for efficient LLM usage | `uvx mcp-server-fetch` |
| [Git](https://github.com/modelcontextprotocol/servers/tree/main/src/git) | Read, search, and manipulate Git repositories | `uvx mcp-server-git` |
| [Memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) | Knowledge graph-based persistent memory system | `npx -y @modelcontextprotocol/server-memory` |
| [Sequential Thinking](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking) | Dynamic problem-solving through structured thought sequences | `npx -y @modelcontextprotocol/server-sequential-thinking` |
| [Time](https://github.com/modelcontextprotocol/servers/tree/main/src/time) | Time and timezone conversion capabilities | `uvx mcp-server-time` |
| [Everything](https://github.com/modelcontextprotocol/servers/tree/main/src/everything) | Reference/test server with prompts, resources, and tools | `npx -y @modelcontextprotocol/server-everything` |

> Archived reference servers (Brave Search, GitHub, GitLab, Google Drive, PostgreSQL, Puppeteer, Redis, Sentry, Slack, SQLite) are at [servers-archived](https://github.com/modelcontextprotocol/servers-archived).

---

## Search & Web

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Brave Search](https://github.com/brave/brave-search-mcp-server) | Privacy-focused web and local search via Brave Search API | `npx -y @brave/brave-search-mcp-server` | [![](https://img.shields.io/github/stars/brave/brave-search-mcp-server?style=flat-square)](https://github.com/brave/brave-search-mcp-server) |
| [Firecrawl](https://github.com/firecrawl/firecrawl-mcp-server) | Web scraping with JS rendering, batch processing, and search | `npx -y firecrawl-mcp` | [![](https://img.shields.io/github/stars/firecrawl/firecrawl-mcp-server?style=flat-square)](https://github.com/firecrawl/firecrawl-mcp-server) |
| [Tavily](https://github.com/tavily-ai/tavily-mcp) | AI-optimized search engine for LLMs and RAG applications | `npx -y tavily-mcp@latest` | [![](https://img.shields.io/github/stars/tavily-ai/tavily-mcp?style=flat-square)](https://github.com/tavily-ai/tavily-mcp) |
| [Exa](https://github.com/exa-labs/exa-mcp-server) | Neural search powered by embeddings for high-quality results | `npx -y exa-mcp-server` | [![](https://img.shields.io/github/stars/exa-labs/exa-mcp-server?style=flat-square)](https://github.com/exa-labs/exa-mcp-server) |
| [Perplexity](https://github.com/perplexityai/modelcontextprotocol) | Search-augmented AI via Perplexity API | See repo | [![](https://img.shields.io/github/stars/perplexityai/modelcontextprotocol?style=flat-square)](https://github.com/perplexityai/modelcontextprotocol) |
| [Apify](https://github.com/apify/apify-mcp-server) | Web scraping and data extraction at scale | `npx -y @apify/mcp-server` | [![](https://img.shields.io/github/stars/apify/apify-mcp-server?style=flat-square)](https://github.com/apify/apify-mcp-server) |
| [AgentQL](https://github.com/tinyfish-io/agentql-mcp) | Structured web data extraction with natural language selectors | `npx -y @agentql/mcp-server` | [![](https://img.shields.io/github/stars/tinyfish-io/agentql-mcp?style=flat-square)](https://github.com/tinyfish-io/agentql-mcp) |
| [Google Maps](https://github.com/cablate/mcp-google-map) | Google Maps geocoding, places, and routing | `npx @cablate/mcp-google-map` | [![](https://img.shields.io/github/stars/cablate/mcp-google-map?style=flat-square)](https://github.com/cablate/mcp-google-map) |

## Browser Automation

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Playwright](https://github.com/microsoft/playwright-mcp) | Browser automation via accessibility snapshots (by Microsoft) | `npx -y @playwright/mcp` | [![](https://img.shields.io/github/stars/microsoft/playwright-mcp?style=flat-square)](https://github.com/microsoft/playwright-mcp) |
| [Browserbase](https://github.com/browserbase/mcp-server-browserbase) | Cloud browser automation with Stagehand AI | `npx -y @browserbasehq/mcp-server` | [![](https://img.shields.io/github/stars/browserbase/mcp-server-browserbase?style=flat-square)](https://github.com/browserbase/mcp-server-browserbase) |
| [Puppeteer](https://github.com/modelcontextprotocol/servers-archived) | Browser automation with screenshot and PDF support | `npx -y @modelcontextprotocol/server-puppeteer` | — |
| [Stealth Browser](https://github.com/brian-ln/stealth-browser-mcp) | Playwright with stealth mode for anti-detection browsing | See repo | [![](https://img.shields.io/github/stars/brian-ln/stealth-browser-mcp?style=flat-square)](https://github.com/brian-ln/stealth-browser-mcp) |

## Databases — Relational

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [DBHub](https://github.com/bytebase/dbhub) | Zero-dependency server for Postgres, MySQL, SQL Server, MariaDB, SQLite | `npx dbhub` | [![](https://img.shields.io/github/stars/bytebase/dbhub?style=flat-square)](https://github.com/bytebase/dbhub) |
| [Supabase](https://github.com/supabase-community/supabase-mcp) | Manage tables, query data, and configure Supabase projects | `npx -y supabase-mcp-server` | [![](https://img.shields.io/github/stars/supabase-community/supabase-mcp?style=flat-square)](https://github.com/supabase-community/supabase-mcp) |
| [Neon](https://github.com/neondatabase/mcp-server-neon) | Serverless Postgres with branching and autoscaling | `npx -y mcp-server-neon` | [![](https://img.shields.io/github/stars/neondatabase/mcp-server-neon?style=flat-square)](https://github.com/neondatabase/mcp-server-neon) |
| [Turso](https://github.com/tursodatabase/turso-mcp) | Edge-hosted SQLite (libSQL) database management | Built into Turso CLI | [![](https://img.shields.io/github/stars/tursodatabase/turso-mcp?style=flat-square)](https://github.com/tursodatabase/turso-mcp) |
| [PostgreSQL](https://github.com/modelcontextprotocol/servers-archived) | Read-only PostgreSQL with schema inspection | `npx -y @modelcontextprotocol/server-postgres` | — |
| [SQLite](https://github.com/modelcontextprotocol/servers-archived) | SQLite database operations | `uvx mcp-server-sqlite` | — |
| [MCP Alchemy](https://github.com/runekaagaard/mcp-alchemy) | SQLAlchemy-based access to Postgres, MySQL, SQLite, Oracle, MS-SQL | `uvx mcp-alchemy` | [![](https://img.shields.io/github/stars/runekaagaard/mcp-alchemy?style=flat-square)](https://github.com/runekaagaard/mcp-alchemy) |
| [ClickHouse](https://github.com/ClickHouse/mcp-clickhouse) | Schema inspection and query capabilities for ClickHouse | `uvx mcp-clickhouse` | [![](https://img.shields.io/github/stars/ClickHouse/mcp-clickhouse?style=flat-square)](https://github.com/ClickHouse/mcp-clickhouse) |
| [MotherDuck](https://github.com/motherduckdb/mcp-server-motherduck) | Local DuckDB and MotherDuck cloud analytics | `npx -y @motherduckdb/mcp-server-motherduck` | [![](https://img.shields.io/github/stars/motherduckdb/mcp-server-motherduck?style=flat-square)](https://github.com/motherduckdb/mcp-server-motherduck) |

## Databases — Vector & Graph

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Qdrant](https://github.com/qdrant/mcp-server-qdrant) | Semantic memory layer on top of Qdrant vector database | `uvx mcp-server-qdrant` | [![](https://img.shields.io/github/stars/qdrant/mcp-server-qdrant?style=flat-square)](https://github.com/qdrant/mcp-server-qdrant) |
| [Chroma](https://github.com/chroma-core/chroma-mcp) | Vector search, full text search, metadata filtering via ChromaDB | `uvx chroma-mcp` | [![](https://img.shields.io/github/stars/chroma-core/chroma-mcp?style=flat-square)](https://github.com/chroma-core/chroma-mcp) |
| [Pinecone](https://github.com/sirmews/mcp-pinecone) | Pinecone vector search integration | `npx -y mcp-pinecone` | [![](https://img.shields.io/github/stars/sirmews/mcp-pinecone?style=flat-square)](https://github.com/sirmews/mcp-pinecone) |
| [Weaviate](https://github.com/weaviate/mcp-server-weaviate) | Connect to Weaviate collections as knowledge base | See repo | [![](https://img.shields.io/github/stars/weaviate/mcp-server-weaviate?style=flat-square)](https://github.com/weaviate/mcp-server-weaviate) |
| [Milvus](https://github.com/zilliztech/mcp-server-milvus) | Interact with Milvus vector databases | See repo | [![](https://img.shields.io/github/stars/zilliztech/mcp-server-milvus?style=flat-square)](https://github.com/zilliztech/mcp-server-milvus) |
| [Neo4j](https://github.com/neo4j-contrib/mcp-neo4j) | Knowledge graph, Cypher queries, and Aura management | See repo | [![](https://img.shields.io/github/stars/neo4j-contrib/mcp-neo4j?style=flat-square)](https://github.com/neo4j-contrib/mcp-neo4j) |
| [Redis](https://github.com/redis/mcp-redis) | Natural language interface to manage and search Redis data | See repo | [![](https://img.shields.io/github/stars/redis/mcp-redis?style=flat-square)](https://github.com/redis/mcp-redis) |
| [Astra DB](https://github.com/datastax/astra-db-mcp) | DataStax Astra DB vector database operations | `npx -y @datastax/astra-db-mcp` | [![](https://img.shields.io/github/stars/datastax/astra-db-mcp?style=flat-square)](https://github.com/datastax/astra-db-mcp) |

## Cloud & Infrastructure

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [AWS](https://github.com/awslabs/mcp) | Suite of AWS servers (S3, Lambda, CDK, DynamoDB, Terraform) | `uvx awslabs.s3-mcp-server` | [![](https://img.shields.io/github/stars/awslabs/mcp?style=flat-square)](https://github.com/awslabs/mcp) |
| [Azure](https://github.com/Azure/azure-mcp) | Interact with Azure resources from AI agents | See repo | [![](https://img.shields.io/github/stars/Azure/azure-mcp?style=flat-square)](https://github.com/Azure/azure-mcp) |
| [Azure DevOps](https://github.com/microsoft/azure-devops-mcp) | Work items, pull requests, builds, and wikis | `npx -y @azure/mcp-server-azure-devops` | [![](https://img.shields.io/github/stars/microsoft/azure-devops-mcp?style=flat-square)](https://github.com/microsoft/azure-devops-mcp) |
| [Cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) | Workers, KV, R2, D1, DNS, and 2,500+ Cloudflare APIs | `npx -y mcp-server-cloudflare` | [![](https://img.shields.io/github/stars/cloudflare/mcp-server-cloudflare?style=flat-square)](https://github.com/cloudflare/mcp-server-cloudflare) |
| [Vercel](https://github.com/vercel/mcp-adapter) | Deploy and manage Vercel projects and deployments | `npx -y @vercel/mcp-adapter` | [![](https://img.shields.io/github/stars/vercel/mcp-adapter?style=flat-square)](https://github.com/vercel/mcp-adapter) |
| [Terraform](https://github.com/hashicorp/terraform-mcp-server) | Terraform Registry, HCP Terraform, and workspace management | `npx -y @hashicorp/terraform-mcp-server` | [![](https://img.shields.io/github/stars/hashicorp/terraform-mcp-server?style=flat-square)](https://github.com/hashicorp/terraform-mcp-server) |
| [Kubernetes](https://github.com/containers/kubernetes-mcp-server) | Native Go implementation for Kubernetes and OpenShift | See repo | [![](https://img.shields.io/github/stars/containers/kubernetes-mcp-server?style=flat-square)](https://github.com/containers/kubernetes-mcp-server) |
| [Docker](https://github.com/docker/mcp-server) | Manage containers, images, and compose stacks | `npx -y @docker/mcp-server` | [![](https://img.shields.io/github/stars/docker/mcp-server?style=flat-square)](https://github.com/docker/mcp-server) |
| [Alibaba Cloud](https://github.com/aliyun/alibabacloud-mcp-server) | Access Alibaba Cloud services and APIs | `pip install alibabacloud-mcp-server` | [![](https://img.shields.io/github/stars/aliyun/alibabacloud-mcp-server?style=flat-square)](https://github.com/aliyun/alibabacloud-mcp-server) |

## Developer Tools

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [GitHub](https://github.com/github/github-mcp-server) | Official GitHub server — repos, PRs, issues, actions | `npx -y @github/mcp-server` | [![](https://img.shields.io/github/stars/github/github-mcp-server?style=flat-square)](https://github.com/github/github-mcp-server) |
| [GitLab](https://github.com/modelcontextprotocol/servers-archived) | GitLab API integration for project management | `npx -y @modelcontextprotocol/server-gitlab` | — |
| [Apollo GraphQL](https://github.com/apollographql/apollo-mcp-server) | Connect to GraphQL APIs with schema introspection | `npx -y @apollo/mcp-server` | [![](https://img.shields.io/github/stars/apollographql/apollo-mcp-server?style=flat-square)](https://github.com/apollographql/apollo-mcp-server) |
| [Appium](https://github.com/appium/appium-mcp) | Mobile app automation testing for iOS and Android | `npx -y @appium/mcp-server` | [![](https://img.shields.io/github/stars/appium/appium-mcp?style=flat-square)](https://github.com/appium/appium-mcp) |
| [Postman](https://github.com/postmanlabs/postman-mcp-server) | Access workspaces, manage collections, evaluate APIs | `npx -y @anthropic/mcp-server-postman` | [![](https://img.shields.io/github/stars/postmanlabs/postman-mcp-server?style=flat-square)](https://github.com/postmanlabs/postman-mcp-server) |
| [Semgrep](https://github.com/semgrep/mcp) | Static analysis security scanning for code vulnerabilities | `uvx semgrep-mcp` | [![](https://img.shields.io/github/stars/semgrep/mcp?style=flat-square)](https://github.com/semgrep/mcp) |
| [ESLint](https://eslint.org/docs/latest/use/mcp) | JavaScript/TypeScript linting via ESLint | `npx @eslint/mcp@latest` | — |
| [Desktop Commander](https://github.com/wonderwhy-er/desktop-commander) | Terminal execution and file operations with user control | `npx -y desktop-commander` | [![](https://img.shields.io/github/stars/wonderwhy-er/desktop-commander?style=flat-square)](https://github.com/wonderwhy-er/desktop-commander) |
| [OpenAPI Generator](https://github.com/harsha-iiiv/openapi-mcp-generator) | Convert OpenAPI 3.0+ specs into MCP servers automatically | `npx openapi-mcp-generator` | [![](https://img.shields.io/github/stars/harsha-iiiv/openapi-mcp-generator?style=flat-square)](https://github.com/harsha-iiiv/openapi-mcp-generator) |

## AI & Knowledge

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Context7](https://github.com/upstash/context7) | Up-to-date code documentation injected into LLM context | `npx -y @upstash/context7-mcp` | [![](https://img.shields.io/github/stars/upstash/context7?style=flat-square)](https://github.com/upstash/context7) |
| [Docfork](https://github.com/docfork/docfork-mcp) | Live documentation and code examples for any library | `npx -y @docfork/mcp` | [![](https://img.shields.io/github/stars/docfork/docfork-mcp?style=flat-square)](https://github.com/docfork/docfork-mcp) |
| [AgentOps](https://github.com/AgentOps-AI/agentops-mcp) | AI agent observability and monitoring | `pip install agentops-mcp` | [![](https://img.shields.io/github/stars/AgentOps-AI/agentops-mcp?style=flat-square)](https://github.com/AgentOps-AI/agentops-mcp) |
| [LangChain](https://github.com/langchain-ai/langchain-mcp-adapters) | Bridge MCP tools into LangChain/LangGraph agents | `pip install langchain-mcp-adapters` | [![](https://img.shields.io/github/stars/langchain-ai/langchain-mcp-adapters?style=flat-square)](https://github.com/langchain-ai/langchain-mcp-adapters) |
| [ReactBits](https://github.com/ibelick/reactbits) | 135+ animated React component patterns for AI reference | See repo | [![](https://img.shields.io/github/stars/ibelick/reactbits?style=flat-square)](https://github.com/ibelick/reactbits) |

## Productivity & Project Management

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Notion](https://github.com/makenotion/notion-mcp-server) | Official Notion API — pages, databases, blocks, semantic search | `npx -y @notionhq/notion-mcp-server` | [![](https://img.shields.io/github/stars/makenotion/notion-mcp-server?style=flat-square)](https://github.com/makenotion/notion-mcp-server) |
| [Linear](https://github.com/jerhadf/linear-mcp-server) | Manage Linear issues, projects, and cycles | `npx -y linear-mcp-server` | [![](https://img.shields.io/github/stars/jerhadf/linear-mcp-server?style=flat-square)](https://github.com/jerhadf/linear-mcp-server) |
| [Atlassian](https://github.com/sooperset/mcp-atlassian) | Jira + Confluence (Cloud + Data Center) | `uvx mcp-atlassian` | [![](https://img.shields.io/github/stars/sooperset/mcp-atlassian?style=flat-square)](https://github.com/sooperset/mcp-atlassian) |
| [Todoist](https://github.com/greirson/mcp-todoist) | Natural language task and project management | `npx @greirson/mcp-todoist` | [![](https://img.shields.io/github/stars/greirson/mcp-todoist?style=flat-square)](https://github.com/greirson/mcp-todoist) |
| [Trello](https://github.com/delorenj/mcp-server-trello) | Interact with Trello boards, lists, and cards | See repo | [![](https://img.shields.io/github/stars/delorenj/mcp-server-trello?style=flat-square)](https://github.com/delorenj/mcp-server-trello) |
| [Obsidian](https://github.com/cyanheads/obsidian-mcp-server) | Read, write, search notes in Obsidian vaults | `npx -y obsidian-mcp-server` | [![](https://img.shields.io/github/stars/cyanheads/obsidian-mcp-server?style=flat-square)](https://github.com/cyanheads/obsidian-mcp-server) |
| [Apple Native](https://github.com/supermemoryai/apple-mcp) | Apple Reminders, Calendar, Notes, Contacts, Maps (macOS) | `npx -y install-mcp apple-mcp` | [![](https://img.shields.io/github/stars/supermemoryai/apple-mcp?style=flat-square)](https://github.com/supermemoryai/apple-mcp) |
| [Google Calendar](https://github.com/nspady/google-calendar-mcp) | Manage Google Calendar events with multi-account support | See repo | [![](https://img.shields.io/github/stars/nspady/google-calendar-mcp?style=flat-square)](https://github.com/nspady/google-calendar-mcp) |
| [WayStation](https://github.com/WayStation-ai/mcp) | Universal connector for Notion, Monday, Airtable, and more | `npx -y @waystation/mcp` | [![](https://img.shields.io/github/stars/WayStation-ai/mcp?style=flat-square)](https://github.com/WayStation-ai/mcp) |

## Communication & Email

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Slack](https://github.com/modelcontextprotocol/servers-archived) | Channel management and messaging | `npx -y @modelcontextprotocol/server-slack` | — |
| [Slack (Advanced)](https://github.com/korotovsky/slack-mcp-server) | DMs, Group DMs, GovSlack, smart history | See repo | [![](https://img.shields.io/github/stars/korotovsky/slack-mcp-server?style=flat-square)](https://github.com/korotovsky/slack-mcp-server) |
| [Discord](https://github.com/v-3/discordmcp) | Discord bot with channel and message management | `npx -y discord-mcp` | [![](https://img.shields.io/github/stars/v-3/discordmcp?style=flat-square)](https://github.com/v-3/discordmcp) |
| [Twilio](https://github.com/twilio-labs/mcp) | SMS, voice, and all Twilio APIs | See repo | [![](https://img.shields.io/github/stars/twilio-labs/mcp?style=flat-square)](https://github.com/twilio-labs/mcp) |
| [SendGrid](https://github.com/Garoth/sendgrid-mcp) | Email marketing via Twilio SendGrid v3 API | See repo | [![](https://img.shields.io/github/stars/Garoth/sendgrid-mcp?style=flat-square)](https://github.com/Garoth/sendgrid-mcp) |
| [Google Workspace](https://github.com/taylorwilsdon/google_workspace_mcp) | Gmail, Calendar, Docs, Sheets, Slides, Drive, Chat | See repo | [![](https://img.shields.io/github/stars/taylorwilsdon/google_workspace_mcp?style=flat-square)](https://github.com/taylorwilsdon/google_workspace_mcp) |
| [Composio](https://github.com/DrDavidHall/rube-composio-mcp) | Connect to 500+ apps (Gmail, Slack, GitHub, Notion) | `npx -y rube-composio-mcp` | [![](https://img.shields.io/github/stars/DrDavidHall/rube-composio-mcp?style=flat-square)](https://github.com/DrDavidHall/rube-composio-mcp) |

## File & Storage

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Google Drive](https://github.com/modelcontextprotocol/servers-archived) | Google Drive file access and search | `npx -y @modelcontextprotocol/server-google-drive` | — |
| [S3 (AWS)](https://github.com/awslabs/mcp) | Amazon S3 bucket and object operations | `uvx awslabs.s3-mcp-server` | [![](https://img.shields.io/github/stars/awslabs/mcp?style=flat-square)](https://github.com/awslabs/mcp) |
| [Files.com](https://github.com/Files-com/files-mcp) | Unified interface for S3, Azure, GCP, SharePoint, SFTP | See repo | [![](https://img.shields.io/github/stars/Files-com/files-mcp?style=flat-square)](https://github.com/Files-com/files-mcp) |

## Finance & Payments

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Stripe](https://github.com/stripe/agent-toolkit) | Payment processing, customer management, and invoicing | `npx -y @stripe/mcp` | [![](https://img.shields.io/github/stars/stripe/agent-toolkit?style=flat-square)](https://github.com/stripe/agent-toolkit) |
| [Alpaca](https://github.com/alpacahq/alpaca-mcp-server) | Stock trading and real-time market data | `npx -y @alpacahq/mcp-server` | [![](https://img.shields.io/github/stars/alpacahq/alpaca-mcp-server?style=flat-square)](https://github.com/alpacahq/alpaca-mcp-server) |
| [Adfin](https://github.com/Adfin-Engineering/mcp-server-adfin) | Payment and invoicing platform integration | `npx -y @adfin/mcp-server` | [![](https://img.shields.io/github/stars/Adfin-Engineering/mcp-server-adfin?style=flat-square)](https://github.com/Adfin-Engineering/mcp-server-adfin) |

## Data & Analytics

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Snowflake](https://github.com/Snowflake-Labs/mcp) | Cortex Agents, SQL execution, and data management with RBAC | See repo | [![](https://img.shields.io/github/stars/Snowflake-Labs/mcp?style=flat-square)](https://github.com/Snowflake-Labs/mcp) |
| [BigQuery](https://github.com/ergut/mcp-bigquery-server) | Google BigQuery dataset exploration and SQL queries | `npx -y @ergut/mcp-bigquery-server` | [![](https://img.shields.io/github/stars/ergut/mcp-bigquery-server?style=flat-square)](https://github.com/ergut/mcp-bigquery-server) |
| [Grafana](https://github.com/grafana/mcp-grafana) | Dashboards, Prometheus/Loki queries, alerting, incidents | See repo | [![](https://img.shields.io/github/stars/grafana/mcp-grafana?style=flat-square)](https://github.com/grafana/mcp-grafana) |

## CMS & Content

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Contentful](https://github.com/contentful/contentful-mcp-server) | Contentful CMS content management and API operations | `npx -y @contentful/mcp-server` | [![](https://img.shields.io/github/stars/contentful/contentful-mcp-server?style=flat-square)](https://github.com/contentful/contentful-mcp-server) |
| [Sanity](https://github.com/sanity-io/sanity-mcp-server) | Sanity CMS document management and GROQ queries | `npx -y @sanity/mcp-server` | [![](https://img.shields.io/github/stars/sanity-io/sanity-mcp-server?style=flat-square)](https://github.com/sanity-io/sanity-mcp-server) |
| [Figma](https://github.com/figma/mcp-server-guide) | Extract design information for AI code generation | Remote MCP | [![](https://img.shields.io/github/stars/figma/mcp-server-guide?style=flat-square)](https://github.com/figma/mcp-server-guide) |
| [21st.dev Magic](https://github.com/21st-dev/magic-mcp) | AI-powered UI component creation | `npx -y @21st-dev/magic-mcp` | [![](https://img.shields.io/github/stars/21st-dev/magic-mcp?style=flat-square)](https://github.com/21st-dev/magic-mcp) |

## CRM & Marketing

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [HubSpot](https://developers.hubspot.com/mcp) | Securely connect AI clients to HubSpot CRM data | Remote MCP | — |
| [Salesforce](https://github.com/LokiMCPUniverse/salesforce-mcp-server) | Full CRM integration with query, create, update, delete | See repo | [![](https://img.shields.io/github/stars/LokiMCPUniverse/salesforce-mcp-server?style=flat-square)](https://github.com/LokiMCPUniverse/salesforce-mcp-server) |
| [NotFair](https://github.com/nowork-studio/toprank) | Google Ads MCP server. Diagnose campaign performance, recommend optimizations, and execute approved changes via the Google Ads API with a built-in human-approval gate. | Remote MCP (streamable-http) | [![](https://img.shields.io/github/stars/nowork-studio/toprank?style=flat-square)](https://github.com/nowork-studio/toprank) |

## Security & Identity

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Auth0](https://github.com/auth0/auth0-mcp-server) | Identity management and authentication flows | `npx -y @auth0/mcp-server` | [![](https://img.shields.io/github/stars/auth0/auth0-mcp-server?style=flat-square)](https://github.com/auth0/auth0-mcp-server) |
| [1Password](https://github.com/1Password/mcp-server) | Secure credential access and secret management | `npx -y @1password/mcp-server` | [![](https://img.shields.io/github/stars/1Password/mcp-server?style=flat-square)](https://github.com/1Password/mcp-server) |
| [Bitwarden](https://github.com/bitwarden/mcp-server) | Secure AI access to Bitwarden vault | See repo | [![](https://img.shields.io/github/stars/bitwarden/mcp-server?style=flat-square)](https://github.com/bitwarden/mcp-server) |

## DevOps & Monitoring

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Sentry](https://github.com/getsentry/sentry-mcp) | Error monitoring and AI-powered root cause analysis | Remote MCP | [![](https://img.shields.io/github/stars/getsentry/sentry-mcp?style=flat-square)](https://github.com/getsentry/sentry-mcp) |
| [Datadog](https://github.com/DataDog/datadog-mcp-server) | Infrastructure monitoring, APM, and log analysis | Remote MCP | [![](https://img.shields.io/github/stars/DataDog/datadog-mcp-server?style=flat-square)](https://github.com/DataDog/datadog-mcp-server) |
| [PagerDuty](https://github.com/PagerDuty/mcp-server-pagerduty) | Incident management and on-call scheduling | `npx -y @pagerduty/mcp-server` | [![](https://img.shields.io/github/stars/PagerDuty/mcp-server-pagerduty?style=flat-square)](https://github.com/PagerDuty/mcp-server-pagerduty) |

## Automation & Workflow

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [n8n](https://github.com/leonardsellem/n8n-mcp-server) | Bridge AI with n8n workflow automation | `npx -y n8n-mcp-server` | [![](https://img.shields.io/github/stars/leonardsellem/n8n-mcp-server?style=flat-square)](https://github.com/leonardsellem/n8n-mcp-server) |

## Smart Home & IoT

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Aqara](https://github.com/aqara/aqara-mcp-server) | Smart home device control and automation | `npx -y @aqara/mcp-server` | [![](https://img.shields.io/github/stars/aqara/aqara-mcp-server?style=flat-square)](https://github.com/aqara/aqara-mcp-server) |
| [Home Assistant](https://github.com/marconipoveda/mcp-server-home-assistant) | Control smart home devices via Home Assistant | `npx -y mcp-server-home-assistant` | [![](https://img.shields.io/github/stars/marconipoveda/mcp-server-home-assistant?style=flat-square)](https://github.com/marconipoveda/mcp-server-home-assistant) |

## Media & Entertainment

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [Spotify](https://github.com/varunneal/spotify-mcp) | Control Spotify playback and manage playlists | `uvx spotify-mcp` | [![](https://img.shields.io/github/stars/varunneal/spotify-mcp?style=flat-square)](https://github.com/varunneal/spotify-mcp) |
| [YouTube Music](https://github.com/instructa/mcp-youtube-music) | Search and play YouTube music tracks | `npx -y mcp-youtube-music` | [![](https://img.shields.io/github/stars/instructa/mcp-youtube-music?style=flat-square)](https://github.com/instructa/mcp-youtube-music) |

## Frameworks & SDKs

| Name | Description | Install | Stars |
|------|-------------|---------|-------|
| [FastMCP](https://github.com/jlowin/fastmcp) | High-level framework for building MCP servers in Python | `pip install fastmcp` | [![](https://img.shields.io/github/stars/jlowin/fastmcp?style=flat-square)](https://github.com/jlowin/fastmcp) |
| [TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) | Official TypeScript SDK for MCP servers and clients | `npm install @modelcontextprotocol/sdk` | [![](https://img.shields.io/github/stars/modelcontextprotocol/typescript-sdk?style=flat-square)](https://github.com/modelcontextprotocol/typescript-sdk) |
| [Python SDK](https://github.com/modelcontextprotocol/python-sdk) | Official Python SDK for MCP servers and clients | `pip install mcp` | [![](https://img.shields.io/github/stars/modelcontextprotocol/python-sdk?style=flat-square)](https://github.com/modelcontextprotocol/python-sdk) |
| [Go SDK](https://github.com/modelcontextprotocol/go-sdk) | Official Go SDK (maintained with Google) | `go get github.com/modelcontextprotocol/go-sdk` | [![](https://img.shields.io/github/stars/modelcontextprotocol/go-sdk?style=flat-square)](https://github.com/modelcontextprotocol/go-sdk) |
| [Kotlin SDK](https://github.com/modelcontextprotocol/kotlin-sdk) | Official Kotlin SDK (maintained with JetBrains) | See repo | [![](https://img.shields.io/github/stars/modelcontextprotocol/kotlin-sdk?style=flat-square)](https://github.com/modelcontextprotocol/kotlin-sdk) |
| [C# SDK](https://github.com/modelcontextprotocol/csharp-sdk) | Official C# SDK (maintained with Microsoft) | `dotnet add package ModelContextProtocol` | [![](https://img.shields.io/github/stars/modelcontextprotocol/csharp-sdk?style=flat-square)](https://github.com/modelcontextprotocol/csharp-sdk) |
| [PHP SDK](https://github.com/modelcontextprotocol/php-sdk) | Official PHP SDK (maintained with PHP Foundation) | See repo | [![](https://img.shields.io/github/stars/modelcontextprotocol/php-sdk?style=flat-square)](https://github.com/modelcontextprotocol/php-sdk) |
| [MCPJungle](https://github.com/mcpjungle/MCPJungle) | Self-hosted MCP gateway for AI agents | `pip install mcpjungle` | [![](https://img.shields.io/github/stars/mcpjungle/MCPJungle?style=flat-square)](https://github.com/mcpjungle/MCPJungle) |
| [MCP Registry](https://github.com/modelcontextprotocol/registry) | Official community-driven registry (app store for MCP) | — | [![](https://img.shields.io/github/stars/modelcontextprotocol/registry?style=flat-square)](https://github.com/modelcontextprotocol/registry) |

---

## Resources

### Directories

| Resource | URL |
|----------|-----|
| Official MCP Servers | [github.com/modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) |
| MCP Registry | [github.com/modelcontextprotocol/registry](https://github.com/modelcontextprotocol/registry) |
| MCP Awesome (1200+) | [mcp-awesome.com](https://mcp-awesome.com/) |
| MCPServers.org | [mcpservers.org](https://mcpservers.org/) |
| PulseMCP | [pulsemcp.com/servers](https://www.pulsemcp.com/servers) |
| Smithery | [smithery.ai/servers](https://smithery.ai/servers) |
| AWS MCP Docs | [awslabs.github.io/mcp](https://awslabs.github.io/mcp/) |
| Microsoft MCP Catalog | [github.com/microsoft/mcp](https://github.com/microsoft/mcp) |

### Curated Lists

| List | Stars |
|------|-------|
| [wong2/awesome-mcp-servers](https://github.com/wong2/awesome-mcp-servers) | [![](https://img.shields.io/github/stars/wong2/awesome-mcp-servers?style=flat-square)](https://github.com/wong2/awesome-mcp-servers) |
| [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | [![](https://img.shields.io/github/stars/punkpeye/awesome-mcp-servers?style=flat-square)](https://github.com/punkpeye/awesome-mcp-servers) |
| [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) | [![](https://img.shields.io/github/stars/appcypher/awesome-mcp-servers?style=flat-square)](https://github.com/appcypher/awesome-mcp-servers) |

---

## Quick Start

### Claude Desktop

Add servers to `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/path/to/allowed/files"]
    },
    "github": {
      "command": "npx",
      "args": ["-y", "@github/mcp-server"],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "your-token"
      }
    },
    "brave-search": {
      "command": "npx",
      "args": ["-y", "@brave/brave-search-mcp-server"],
      "env": {
        "BRAVE_API_KEY": "your-key"
      }
    }
  }
}
```

### Claude Code (CLI)

```bash
claude mcp add filesystem -- npx -y @modelcontextprotocol/server-filesystem /path
claude mcp add brave-search -e BRAVE_API_KEY=your-key -- npx -y @brave/brave-search-mcp-server
```

### Cursor / VS Code / Windsurf

Add to `.cursor/mcp.json`, `.vscode/mcp.json`, or equivalent:

```json
{
  "servers": {
    "playwright": {
      "command": "npx",
      "args": ["-y", "@playwright/mcp"]
    }
  }
}
```

---

## How to Choose

| Need | Recommended Server |
|------|--------------------|
| Web search | Brave Search, Tavily, Exa |
| Web scraping | Firecrawl, Apify, Playwright |
| Database (multi-DB) | DBHub |
| Database (managed) | Supabase, Neon, Turso |
| Vector search | Qdrant, Chroma, Pinecone |
| Cloud deploy | AWS, Cloudflare, Vercel |
| Code docs | Context7, Docfork |
| Project mgmt | Linear, Notion, Atlassian |
| Monitoring | Sentry, Grafana, Datadog |
| Payments | Stripe |
| Build MCP servers | FastMCP (Python), TypeScript SDK |

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines. PRs welcome!

---

## 繁體中文

### 這是什麼？

**Awesome MCP Servers** 是一份精選的 [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) 伺服器清單。MCP 是一個開放協定（現已加入 [Linux 基金會](https://www.linuxfoundation.org/)），讓 AI 模型（Claude、ChatGPT、Cursor 等）能安全地與外部工具、資料庫、API 和服務互動。

### 為什麼重要？

MCP 讓 AI 不再只是「聊天機器人」，而是真正能操作工具的智能助手：

| 用途 | MCP 伺服器 |
|------|-----------|
| 搜尋引擎 | Brave Search、Tavily、Exa |
| 瀏覽器自動化 | Playwright（微軟）、Puppeteer |
| 資料庫 | PostgreSQL、MySQL、SQLite、向量資料庫 |
| 雲端部署 | AWS、Azure、Cloudflare、Vercel |
| 開發工具 | GitHub、GitLab、Docker、ESLint |
| 生產力工具 | Notion、Linear、Jira、Todoist |
| 金流支付 | Stripe、Alpaca |
| 監控告警 | Sentry、Grafana、Datadog |

### 快速開始

1. 在上方清單中找到你需要的 MCP 伺服器
2. 複製安裝指令（通常是 `npx -y @xxx/mcp-server` 或 `pip install xxx`）
3. 加入你的 AI 工具設定檔（Claude Desktop / Claude Code / Cursor / VS Code）
4. 完成！AI 現在可以使用該工具了

### 如何貢獻？

歡迎提交 Pull Request！請參考 [CONTRIBUTING.md](CONTRIBUTING.md) 了解提交格式。

---

## License

[MIT](LICENSE) © 2026
