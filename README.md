# Awesome MCP Servers ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)

A curated list of awesome Model Context Protocol (MCP) servers. MCP is an open protocol that enables AI models to securely interact with local and remote resources through standardized server implementations. This list focuses on production-ready and experimental MCP servers that extend AI capabilities through file access, database connections, API integrations, and other contextual services.

<br />

## ⚠️ Security Warning

> [!WARNING]
>  When running MCP servers without proper sandboxing, they can execute arbitrary code on your system with the same permissions as the host process. This creates significant security risks.
>
> **Security Risks:**
> - **System Access**: Full access to files, network, and system resources
> - **Code Execution**: Can run any command on your machine
> - **Prompt Injection**: Malicious prompts could trigger unintended server actions
> - **Data Exposure**: Sensitive data may be accessed or leaked
>
> **Best Practices:**
> - Use official implementations (marked with ⭐) when available
> - Run servers in VMs or isolated environments
> - Review code before installation
> - Limit permissions to minimum required
> - Monitor server activity

<br />

## Examples of Supported Clients

|                                                                                                                                                                                          | MCP Host                                                                    | Documentation                                                                                                 |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| <img src="https://avatars.githubusercontent.com/u/6430791" alt="Claude.app" width="40" height="40">                                                                                      | [Claude.app](https://claude.ai)                                             | [MCP server setup](https://modelcontextprotocol.io/quickstart/user)                                           |
| <img src="https://avatars.githubusercontent.com/u/134943970" alt="Cursor" width="40" height="40">                                                                                        | [Cursor](https://cursor.com)                                                | [MCP server setup](https://docs.cursor.com/context/model-context-protocol)                                    |
| <img src="https://avatars.githubusercontent.com/u/182288589" alt="Continue" width="40" height="40">                                                                                      | [Continue](https://github.com/continuedev/continue)                         | [MCP server setup](https://docs.continue.dev/customize/context-providers#model-context-protocol-mcp)         |
| <img src="https://avatars.githubusercontent.com/u/170994773" alt="Cline" width="40" height="40">                                                                                         | [Cline](https://github.com/cline/cline)                                     | [MCP server setup](https://github.com/cline/cline/blob/main/docs/mcp/README.md)                              |
| <img src="https://avatars.githubusercontent.com/u/10232950" alt="Zed" width="40" height="40">                                                                                            | [Zed](https://zed.dev)                                                      | [MCP server setup](https://zed.dev/docs/assistant/model-context-protocol)                                     |
| <img src="https://avatars.githubusercontent.com/u/41454982" alt="Windsurf" width="40" height="40">                                                                                       | [Windsurf Editor](https://codeium.com/windsurf)                             | [MCP server setup](https://docs.codeium.com/windsurf/mcp)                                                     |
| <img src="https://avatars.githubusercontent.com/u/186807194" alt="Copilot.app" width="40" height="40">                                                                                   | [GitHub Copilot](https://github.com/features/copilot)                       | [MCP server setup](https://docs.github.com/en/copilot/customizing-copilot/using-model-context-protocol-with-github-copilot) |
| <img src="https://avatars.githubusercontent.com/u/50659782" alt="Entelligence.AI" width="40" height="40">                                                                                | [Entelligence.AI](https://www.entelligence.ai)                              | [MCP server setup](https://docs.entelligence.ai/mcp)                                                         |
| <img src="https://storage.googleapis.com/gweb-uniblog-publish-prod/images/gemini-logo.max-200x200.png" alt="Gemini" width="40" height="40">                                              | [Gemini CLI](https://github.com/google-gemini/gemini-cli)                   | [MCP server setup](https://github.com/google-gemini/gemini-cli?tab=readme-ov-file#extension-via-mcp-servers) |

<br />

## Table of Contents

- 🎖️ - [Official Integrations](#official-integrations)
- 📂 - [File Systems](#file-systems)
- 🗄️ - [Databases](#databases)
- 💬 - [Communication](#communication)
- 🤖 - [AI Services](#ai-services)
- ☁️ - [Cloud Platforms](#cloud-platforms)
- 🔄 - [DevOps & CI/CD](#devops--cicd)
- 🌐 - [Web & Browser Automation](#web--browser-automation)
- 📊 - [Data & Analytics](#data--analytics)
- 🧩 - [API Integration](#api-integration)
- 🔐 - [Security](#security)
- 🗺️ - [Location & Maps](#location--maps)
- 🌿 - [Version Control](#version-control)
- 📋 - [Project Management](#project-management)
- 📧 - [Email](#email)
- 🎨 - [Design & Media](#design--media)
- 🔬 - [Research & Science](#research--science)
- 💹 - [Finance](#finance)
- 🧠 - [Knowledge & Memory](#knowledge--memory)
- 🔧 - [Developer Tools](#developer-tools)
- 🎮 - [Gaming](#gaming)
- 🏥 - [Healthcare](#healthcare)
- 📱 - [Mobile](#mobile)
- 🌐 - [Language & Translation](#language--translation)
- 🎵 - [Entertainment](#entertainment)
- 🛒 - [E-Commerce](#e-commerce)
- 🔌 - [IoT & Hardware](#iot--hardware)
- 📰 - [News & Media](#news--media)
- 🧪 - [Testing & QA](#testing--qa)
- 🏢 - [Enterprise Systems](#enterprise-systems)
- 🌍 - [Environment & Sustainability](#environment--sustainability)
- 🤝 - [Customer Support](#customer-support)
- 🎓 - [Education](#education)
- 📦 - [Package Management](#package-management)
- 🖥️ - [Operating System Interaction](#operating-system-interaction)
- 🚗 - [Transportation](#transportation)
- 🧰 - [Miscellaneous](#miscellaneous)

<br />

## 🎖️ <a name="official-integrations"></a>Official Integrations

Official MCP server integrations provided directly by companies and organizations.

- <img src="https://axiom.co/favicon.ico" height="14"/> [Axiom](https://github.com/axiomhq/mcp-server-axiom) - Query and analyze your Axiom logs, traces, and all other event data in natural language
- <img src="https://browserbase.com/favicon.ico" height="14"/> [Browserbase](https://github.com/browserbase/mcp-server-browserbase) - Automate browser interactions in the cloud
- <img src="https://cdn.brandfetch.io/cloudflare.com/w/512/h/512" height="14"/> [Cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) - Deploy and manage resources on the Cloudflare developer platform
- <img src="https://e2b.dev/favicon.ico" height="14"/> [E2B](https://github.com/e2b-dev/mcp-server) - Execute code in secure cloud sandboxes
- <img src="https://exa.ai/images/favicon-32x32.png" height="14"/> [Exa](https://github.com/exa-labs/exa-mcp-server) - AI-native web search and scraping
- <img src="https://avatars.githubusercontent.com/u/54536011" height="14"/> [Grafana](https://github.com/grafana/mcp-grafana) - Search dashboards, investigate incidents and query datasources in your Grafana instance
- <img src="https://framerusercontent.com/images/GtdBJXSIEWGl8fY5WiNMDSa3Mk.png" height="14"/> [Graphlit](https://github.com/graphlit/graphlit-mcp-server) - Ingest anything from Slack to Gmail to podcast feeds, in addition to web crawling, and PDF, Word and Markdown file ingestion
- <img src="https://jetbrains.com/favicon.ico" height="14"/> [JetBrains](https://github.com/JetBrains/mcp-jetbrains) - Work on your code in JetBrains IDEs
- <img src="https://kagi.com/favicon.ico" height="14"/> [Kagi](https://github.com/kagisearch/kagimcp) - Search the web using Kagi's search API
- <img src="https://www.make.com/favicon.ico" height="14"/> [Make](https://github.com/integromat/make-mcp-server) - Turn your Make scenarios into callable tools for AI assistants
- <img src="https://www.neon.tech/favicon/favicon-32x32.png" height="14"/> [Neon](https://github.com/neondatabase/mcp-server-neon) - Create and manage Neon Postgres projects, branches, and databases
- <img src="https://avatars.githubusercontent.com/u/3431088" height="14"/> [Oxylabs](https://github.com/oxylabs/oxylabs-mcp) - Scrape websites with Oxylabs Web API, supporting dynamic content rendering with JavaScript
- <img src="https://avatars.githubusercontent.com/u/1798433" height="14"/> [PayPal](https://github.com/paypal/agent-toolkit) - Interact with PayPal APIs for payments, subscriptions, invoices and more.
- <img src="https://avatars.githubusercontent.com/u/49888249" height="14"/> [Perplexity](https://github.com/ppl-ai/modelcontextprotocol) - Perplexity provides an API that allows interaction with their AI model
- <img src="https://raw.githubusercontent.com/PLangHQ/plang/refs/heads/main/Documentation/apps/plang_logo_128x128.png" height="14"/> [Plang](https://github.com/PLangHQ/plang/tree/main/mcp) - MCP Server for [Plang](https://plang.is) programming language, to create, build and run .goal files
- <img src="https://cdn.prod.website-files.com/6750d7b7e819dfd03756a75b/6750d7b7e819dfd03756a7c1_Favicon%20256.png" height="14"/> [Raygun](https://github.com/MindscapeHQ/mcp-server-raygun) - Interact with your crash reporting and real user monitoring data on your Raygun account
- <img src="https://seeklogo.com/images/S/sentry-logo-36867007B0-seeklogo.com.png" height="14"/> [Sentry](https://github.com/getsentry/sentry-mcp) - Connect AI tools to Sentry to look up error data, create issues, and more
- <img src="https://tavily.com/favicon.ico" height="14"/> [Tavily](https://github.com/RamXX/mcp-tavily) - An MCP server for Tavily's search & news API
- <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Tripadvisor_Logo.svg/250px-Tripadvisor_Logo.svg.png" height="14"/> [TripAdvisor](https://github.com/piddlingtuna/tripadvisor-mcp-server) - Search TripAdvisor for travel locations and more
- <img src="https://framerusercontent.com/images/yWOsUNiQe8JKTkXD2nMBvjkLs.png" height="14"/> [Turbopuffer](https://github.com/turbopuffer/turbopuffer-mcp) - Native access to turbopuffer for lightning-fast vector search and serverless inference
- <img src="https://upload.wikimedia.org/wikipedia/commons/a/a9/Amazon_logo.svg" height="14"/> [AWS KB Retrieval](https://github.com/modelcontextprotocol/servers/tree/main/src/aws-kb-retrieval-server) - Retrieval from AWS Knowledge Base using Bedrock Agent Runtime
- <img src="https://avatars.githubusercontent.com/u/62214163" height="14"/> [Xero](https://github.com/XeroAPI/xero-mcp-server) - Interact with your Xero account data using natural language

<br />

## 📂 <a name="file-systems"></a>File Systems

Provides direct access to local and remote file systems with configurable permissions for AI models.

- [Filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) - Secure file operations with configurable access controls
- [Files](https://github.com/mark3labs/mcp-filesystem-server) - Secure file operations with configurable access controls written in Go
- [Box](https://github.com/hmk/box-mcp-server) - Connect to your Box account to list, read and search for files
- [Google Drive](https://github.com/modelcontextprotocol/servers/tree/main/src/gdrive) - File access and search for Google Drive
- [Obsidian Markdown Files](https://github.com/calclavia/mcp-obsidian) - Read and search through Markdown notes in Obsidian vaults
- [SharePoint](https://github.com/softeria-eu/mcp-sharepoint) - Access to SharePoint content, browsing files and reading documents
- [ReadPDF](https://github.com/sylphlab/pdf-reader-mcp) - A PDF reader server that allows Claude to read and extract text from PDF files
- [Folder Structure Context](https://github.com/guillermom11/mcp-folder-structure) - Provides folder structure context to AI models
- [OneDrive](https://github.com/aplevin/onedrive-mcp-server) - Read and search files within OneDrive

<br />

## 🗄️ <a name="databases"></a>Databases

Database integration tools for reading, writing, and managing data across various database types.

- [Chroma](https://github.com/chroma-core/chroma-mcp) - Embeddings, vector search, document storage, and full-text search with the open-source AI application database
- [ClickHouse](https://github.com/ClickHouse/mcp-clickhouse) - Connect to your ClickHouse database and run queries.
- [CockroachDB](https://github.com/truewebber/mcp-cockroachdb) - MCP server for CockroachDB with read, write, and schema discovery.
- [DuckDB](https://github.com/ktanaka101/mcp-server-duckdb) - DuckDB database integration with schema inspection and query capabilities
- [Elasticsearch](https://github.com/cr7258/elasticsearch-mcp-server) - Elasticsearch integration for search and analytics
- [EXASol](https://github.com/nicktindall/mcp-server-exasol) - Exasol database integration with schema inspection and query capabilities
- [Firebase Firestore](https://github.com/gannonh/firebase-mcp) - Firebase services including Auth, Firestore and Storage.
- [Jet MCP](https://github.com/yoda-digital/mcp-gitlab-server) - GitLab integration for MCP
- [Lancedb](https://github.com/Kalos-mcp/lancedb) - LanceDB database integration
- [libSQL](https://github.com/elitan/mcp-server-turso) - Connect and query libSQL databases, compatible with Turso
- [Microsoft SQL Server](https://github.com/JubinSaniei/mcp-mssql-server) - Microsoft SQL Server database integration
- [MongoDB](https://github.com/kiliczsh/mcp-mongo-server) - A Model Context Protocol Server for MongoDB
- [MySQL](https://github.com/benborla/mcp-server-mysql) - MySQL database integration in NodeJS with configurable access controls
- [MySQL](https://github.com/designcomputer/mysql_mcp_server) - MySQL database integration in Python with configurable access controls
- [Neo4j](https://github.com/da-okazaki/mcp-neo4j-server) - A community-built MCP server for Neo4j Graph Databases
- [Nile Database](https://github.com/niledatabase/nile-mcp-server) - MCP server for Nile's Postgres platform for multi-tenant apps
- [OpenSearch](https://github.com/riccardo-larosa/mcp-opensearch) - OpenSearch database integration
- [Oracle DB](https://github.com/pawanmudgal/oracle-db-mcp-server) - Oracle Database integration with schema inspection and query capabilities
- [PGlite](https://github.com/yigitkonur/pglite-mcp-server) - MCP server for PGlite, a WebAssembly-based PostgreSQL
- [PostgreSQL](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres) - Read-only database access with schema inspection capabilities
- [QuestDB](https://github.com/questdb/questdb-mcp-server) - MCP server for QuestDB, a high-performance time-series database.
- [Redis](https://github.com/modelcontextprotocol/servers/tree/main/src/redis) - Interact with Redis key-value stores
- [Riak](https://github.com/jonathandturner/mcp-riak-server) - Riak database integration
- [Snowflake](https://github.com/datawiz168/mcp-snowflake-service) - Interact with Snowflake databases
- [SQLite](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite) - Database interaction and business intelligence capabilities
- [SQLite](https://github.com/FreePeak/db-mcp-server) - A high-performance multi-database MCP server supporting MySQL & PostgreSQL with built-in tools for query execution, transaction management, schema exploration, query building, and performance analysis
- [Supabase](https://github.com/supabase-community/supabase-mcp) - Interact with Supabase databases
- [TiDB](https://github.com/pingcap/tidb-mcp-server) - Connect to TiDB Cloud Serverless clusters

<br />

## 💬 <a name="communication"></a>Communication

Tools for integrating with messaging, email, and collaboration platforms.

- <img src="https://www.atlassian.com/favicon.ico" height="14"/> [Confluence](https://github.com/sooperset/mcp-atlassian) - Interact with Atlassian Confluence for documentation management
- <img src="https://discord.com/assets/favicon.ico" height="14"/> [Discord](https://github.com/v-3/discordmcp) - Connect to Discord servers to read channel histories and send messages
- <img src="https://www.gitter.im/favicon.ico" height="14"/> [Gitter](https://github.com/the-alex-franklin/gitter-mcp) - MCP server for Gitter, to create and view rooms and messages
- <img src="https://www.google.com/favicon.ico" height="14"/> [Google Chat](https://github.com/kapilkumar2001/google-chat-mcp-server) - Access Google Chat messages
- <img src="https://www.intercom.com/favicon.ico" height="14"/> [Intercom](https://github.com/raoulbia-ai/mcp-server-for-intercom) - Retrieve and analyze Intercom support tickets, including full conversation history
- <img src="https://www.jira.com/favicon.ico" height="14"/> [Jira](https://github.com/sooperset/mcp-atlassian) - Interact with Atlassian Jira for project management
- <img src="https://www.line.me/favicon.ico" height="14"/> [LINE](https://github.com/amornpan/py-mcp-line) - Integration for LINE Messaging API to read and analyze LINE conversations
- <img src="https://www.microsoft.com/favicon.ico" height="14"/> [Microsoft Teams](https://github.com/pathintegral-institute/mcp-servers/tree/main/servers/mcp-teams) - Microsoft Teams integration for sending messages and managing team communications
- <img src="https://www.notionhq.com/favicon.ico" height="14"/> [Notion](https://github.com/v-3/notion-server) - Interact with Notion for documentation and knowledge management
- <img src="https://slack.com/favicon.ico" height="14"/> [Slack](https://github.com/modelcontextprotocol/servers/tree/main/src/slack) - Channel management and messaging capabilities
- <img src="https://telegram.org/favicon.ico" height="14"/> [Telegram](https://github.com/kfastov/telegram-mcp-server) - Integrate with Telegram to send and receive messages
- <img src="https://twist.com/favicon.ico" height="14"/> [Twist](https://github.com/BernardMcWeeney/twist-mcp-server) - MCP server for Twist, the async communication tool for teams.
- <img src="https://twitter.com/favicon.ico" height="14"/> [Twitter/X](https://github.com/EnesCinr/twitter-mcp) - Interact with Twitter API. Post tweets and search for tweets by query.
- <img src="https://twitter.com/favicon.ico" height="14"/> [Twitter/X](https://github.com/vidhupv/x-mcp) - Create, manage and publish X/Twitter posts
- <img src="https://www.whatsapp.com/favicon.ico" height="14"/> [WhatsApp](https://github.com/lharries/whatsapp-mcp) - Interact with your personal WhatsApp messages, search and send messages to individuals and groups

<br />

## 🤖 <a name="ai-services"></a>AI Services

Integrations with AI models, machine learning services, and AI-powered tools.

- <img src="https://www.anthropic.com/favicon.ico" height="14"/> [Anthropic](https://github.com/anthropics/anthropic-mcp-server) - Access Anthropic's AI models for content analysis and generation
- <img src="https://cohere.com/favicon.ico" height="14"/> [Cohere](https://github.com/cohere-ai/cohere-mcp) - Connect to Cohere's API for generating, classifying, and summarizing text
- <img src="https://fal.ai/favicon.ico" height="14"/> [fal.ai](https://github.com/fal-ai/fal-mcp) - Run AI models on fal.ai's serverless GPU infrastructure
- <img src="https://huggingface.co/favicon.ico" height="14"/> [HuggingFace](https://github.com/evalstate/mcp-hfspace) - Use HuggingFace spaces and models
- <img src="https://www.langfuse.com/favicon.ico" height="14"/> [Langfuse Prompt Management](https://github.com/langfuse/mcp-server-langfuse) - Open-source tool for collaborative editing, versioning, and accessing prompts via the Langfuse Prompt Management SDK.
- <img src="https://www.langfuse.com/favicon.ico" height="14"/> [Langfuse Tracing](https://github.com/langfuse/mcp-server-langfuse) - Interact with LLM application traces in Langfuse for understanding & improving AI app behavior.
- <img src="https://lmstudio.ai/favicon.ico" height="14"/> [LM Studio](https://github.com/lmstudio-ai/mcp-server-lmstudio) - Control LM Studio from Claude
- <img src="https://mistral.ai/favicon.ico" height="14"/> [Mistral](https://github.com/bkvarda/mcp-mistral) - Connect to Mistral AI's language models
- <img src="https://openai.com/favicon.ico" height="14"/> [OpenAI](https://github.com/mzxrai/mcp-openai) - Chat with OpenAI's smartest models
- <img src="https://openai.com/favicon.ico" height="14"/> [OpenAI](https://github.com/wong2/mcp-openai-server) - A simple OpenAI API MCP server
- <img src="https://replicate.com/favicon.ico" height="14"/> [Replicate](https://github.com/deepfates/mcp-replicate) - Search and run models on Replicate platform
- <img src="https://www.stability.ai/favicon.ico" height="14"/> [Stability AI](https://github.com/tamasbelinszky/mcp-stability-ai) - Generate images using the Stability AI API
- <img src="https://vectorize.io/favicon.ico" height="14"/> [Vectorize](https://github.com/vectorize-io/vectorize-mcp-server/) - Advanced retrieval, Private Deep Research, Anything-to-Markdown file extraction and text chunking.
- <img src="https://www.cerebras.ai/favicon.ico" height="14"/> [Cerebras](https://github.com/cerebras/cerebras-mcp) - Connect to Cerebras AI for fast LLM inference

<br />

## ☁️ <a name="cloud-platforms"></a>Cloud Platforms

Access and management of cloud infrastructure, services, and resources.

- <img src="https://aws.amazon.com/favicon.ico" height="14"/> [AWS](https://github.com/rishikavikondala/mcp-server-aws) - Perform operations on your AWS resources using an LLM
- <img src="https://aws.amazon.com/favicon.ico" height="14"/> [AWS Cost Explorer](https://github.com/aaronsb/mcp-aws-cost-explorer) - AWS Cost and Usage tools for billing analysis
- <img src="https://azure.microsoft.com/favicon.ico" height="14"/> [Azure](https://github.com/Azure/azure-mcp) - Azure management and interaction capabilities
- <img src="https://cdn.brandfetch.io/cloudflare.com/w/512/h/512" height="14"/> [Cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) - Deploy and manage resources on the Cloudflare developer platform
- <img src="https://www.digitalocean.com/favicon.ico" height="14"/> [DigitalOcean](https://github.com/digitalocean/mcp-server) - Manage DigitalOcean resources, Droplets, databases, domains, and more through natural language
- <img src="https://www.google.com/favicon.ico" height="14"/> [GCP](https://github.com/rahulthedevil/gcp-mcp-server) - Google Cloud Platform integration for managing GCP resources
- <img src="https://fly.io/favicon.ico" height="14"/> [Fly.io](https://github.com/fly-apps/fly-mcp) - Manage your apps on Fly.io
- <img src="https://www.heroku.com/favicon.ico" height="14"/> [Heroku](https://github.com/heroku/heroku-mcp-server) - Interact with the Heroku Platform to manage and deploy apps, dynos, add-ons, and more
- <img src="https://opslevel.com/favicon.ico" height="14"/> [OpsLevel](https://github.com/OpsLevel/mcp-server-opslevel) - Interact with OpsLevel, the Internal Developer Portal
- <img src="https://railway.app/favicon.ico" height="14"/> [Railway](https://github.com/jason-tan-swe/railway-mcp) - Integrate with Railway for deploying and managing Railway infrastructure
- <img src="https://render.com/favicon.ico" height="14"/> [Render](https://github.com/Render-AI/render-mcp-server) - Manage and deploy services on the Render cloud platform
- <img src="https://www.vercel.com/favicon.ico" height="14"/> [Vercel](https://github.com/vercel/mcp-adapter) - An MCP adapter for Vercel

<br />

## 🔄 <a name="devops--cicd"></a>DevOps & CI/CD

Tools for automating software development, deployment, and infrastructure management.

- <img src="https://buildkite.com/favicon.ico" height="14"/> [Buildkite](https://github.com/buildkite/buildkite-mcp-server) - Interact with Buildkite APIs to access builds, pipelines and agents.
- <img src="https://circleci.com/favicon.ico" height="14"/> [CircleCI](https://github.com/CircleCI-Public/mcp-server-circleci) - Enable AI Agents to fix build failures from CircleCI
- <img src="https://www.docker.com/favicon.ico" height="14"/> [Docker](https://github.com/ckreiling/mcp-server-docker) - Integrate with Docker to manage containers, images, volumes, and networks
- <img src="https://www.drone.io/favicon.ico" height="14"/> [Drone](https://github.com/MarkusPfundstein/mcp-server-drone) - Interact with Drone CI server for builds, repositories and users
- <img src="https://github.githubassets.com/favicon.ico" height="14"/> [GitHub](https://github.com/modelcontextprotocol/servers/tree/main/src/github) - Repository management, file operations, and GitHub API integration
- <img src="https://about.gitlab.com/ico/favicon.ico" height="14"/> [GitLab](https://github.com/yoda-digital/mcp-gitlab-server) - Interact with GitLab repositories, issues, pipelines and more
- <img src="https://www.jenkins.io/favicon.ico" height="14"/> [Jenkins](https://github.com/ARMmaster17/mcp-server-jenkins) - Interact with Jenkins CI/CD server for pipelines and builds
- <img src="https://www.hashicorp.com/favicon.ico" height="14"/> [Terraform](https://github.com/hashicorp/terraform-mcp-server) - Seamless integration with Terraform ecosystem for infrastructure as code workflows
- <img src="https://about.gitlab.com/ico/favicon.ico" height="14"/> [GitLab](https://github.com/kapilkumar2001/mcp-gitlab-server) - Another GitLab integration for MCP

<br />

## 🌐 <a name="web--browser-automation"></a>Web & Browser Automation

Tools for web scraping, browser automation, and internet information retrieval.

- <img src="https://www.browse.ai/favicon.ico" height="14"/> [Browse AI](https://github.com/Browse-AI/browse-ai-mcp) - Extract and monitor data from websites using Browse AI
- <img src="https://brightdata.com/favicon.ico" height="14"/> [Bright Data](https://github.com/luminati-io/brightdata-mcp) - Bypass anti-bot measures and access any website at scale
- <img src="https://browsermcp.io/favicon.ico" height="14"/> [BrowserMCP](https://github.com/browsermcp/mcp) - Automate your local browser using MCP
- <img src="https://firecrawl.dev/favicon.ico" height="14"/> [Firecrawl](https://github.com/mendableai/firecrawl-mcp-server) - Advanced web scraping with JavaScript rendering
- <img src="https://hyperbrowser.ai/favicon.ico" height="14"/> [Hyperbrowser](https://github.com/hyperbrowserai/mcp) - Headless browsers in the cloud: scrape, crawl, and navigate any site
- <img src="https://lightpanda.io/favicon.ico" height="14"/> [Lightpanda](https://github.com/lightpanda-io/mcp-server) - An ultra-fast headless browser for AI agents, designed for web scraping and automation
- <img src="https://www.microsoft.com/favicon.ico" height="14"/> [Playwright](https://github.com/executeautomation/mcp-playwright) - Browser automation and webscraping using Playwright
- <img src="https://puppeteer.github.io/favicon.ico" height="14"/> [Puppeteer](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer) - Browser automation and web scraping
- <img src="https://scrapingbee.com/favicon.ico" height="14"/> [ScrapingBee](https://github.com/scrapingbee/mcp-scrapingbee) - Web scraping with JavaScript rendering using ScrapingBee
- <img src="https://searxng.org/favicon.ico" height="14"/> [SearXNG](https://github.com/ihor-sokoliuk/mcp-searxng) - Open-source internet metasearch engine
- <img src="https://serpapi.com/favicon.ico" height="14"/> [SerpApi](https://github.com/SerpApi/mcp-server-serpapi) - Scrape search engine results using SerpApi
- <img src="https://stagehand.dev/favicon.ico" height="14"/> [Stagehand](https://github.com/browserbase/stagehand-mcp-server) - AI-powered browser automation using Stagehand
- [Fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) - Web content fetching and conversion for efficient LLM usage
- [Bing Search](https://github.com/leehanchung/mcp-bing-search) - Bing Search integration for web search
- [DuckDuckGo Search](https://github.com/nickclyde/duckduckgo-mcp-server) - Web search using DuckDuckGo

<br />

## 📊 <a name="data--analytics"></a>Data & Analytics

Data processing, visualization, and analytics tools.

- <img src="https://grafana.com/favicon.ico" height="14"/> [Grafana](https://github.com/grafana/mcp-grafana) - Access your Grafana instance and interact with dashboards, data sources, and incidents
- <img src="https://metabase.com/favicon.ico" height="14"/> [Metabase](https://github.com/biegehydra/mcp-metabase) - Connect to Metabase instance and use natural language to query databases
- <img src="https://mode.com/favicon.ico" height="14"/> [Mode](https://github.com/punkpeye/mcp-mode) - Interact with Mode analytics
- <img src="https://motherduck.com/favicon.ico" height="14"/> [MotherDuck](https://github.com/motherduck-orm/mcp-server-motherduck) - Connect to MotherDuck cloud analytics service
- <img src="https://openbb.co/favicon.ico" height="14"/> [OpenBB](https://github.com/OpenBB-finance/mcp-for-openbb) - MCP server for OpenBB, the open source financial data platform
- <img src="https://www.pandas.com/favicon.ico" height="14"/> [Pandas AI](https://github.com/Sinaptik-AI/pandas-ai-mcp) - Intelligent data analysis using Pandas AI
- <img src="https://www.tableau.com/favicon.ico" height="14"/> [Tableau](https://github.com/takuya-hashimoto/mcp-tableau) - Tableau integration for analytics and visualization
- [Kaggle](https://github.com/Hk669/mcp-kaggle) - Explore and use Kaggle datasets and competitions

<br />

## 🧩 <a name="api-integration"></a>API Integration

Tools for connecting to and working with various external APIs.

- <img src="https://www.airtable.com/favicon.ico" height="14"/> [Airtable](https://github.com/domdomegg/airtable-mcp-server) - Read and write access to Airtable databases
- <img src="https://www.alibabacloud.com/favicon.ico" height="14"/> [Alibaba Cloud](https://github.com/aliyun/alibaba-cloud-ops-mcp-server) - Manage and operate Alibaba Cloud resources
- <img src="https://raw.githubusercontent.com/BerriAI/litellm/refs/heads/main/docs/my-website/img/favicon.ico" height="14"/> [Any OpenAI-Compatible LLM](https://github.com/calvernaz/alphapilot) - Connect to any OpenAI-compatible LLM
- <img src="https://www.contentful.com/favicon.ico" height="14"/> [Contentful](https://github.com/jakobhoeg/mcp-contentful-server) - Interact with Contentful CMS
- <img src="https://www.hubspot.com/hubfs/HubSpot_Logos/HubSpot-Inversed-Favicon.png" height="14"/> [HubSpot](https://github.com/buryat/mcp-hubspot) - Interact with HubSpot CRM
- <img src="https://linear.app/favicon.ico" height="14"/> [Linear](https://github.com/jerhadf/linear-mcp-server) - Linear project management integration
- <img src="https://openapi-mcp.com/favicon.ico" height="14"/> [OpenAPI](https://github.com/snaggle-ai/openapi-mcp-server) - Run any OpenAPI-compatible API via MCP
- <img src="https://www.salesforce.com/favicon.ico" height="14"/> [Salesforce](https://github.com/smn2gnt/MCP-Salesforce) - Interact with Salesforce data and metadata
- <img src="https://stripe.com/favicon.ico" height="14"/> [Stripe](https://github.com/stripe/agent-toolkit) - Interact with the Stripe API
- <img src="https://www.zendesk.com/favicon.ico" height="14"/> [Zendesk](https://github.com/reminia/mcp-zendesk) - Interact with Zendesk for customer support management
- <img src="https://zapier.com/favicon.ico" height="14"/> [Zapier](https://github.com/zapier/mcp-server-zapier) - Connect to thousands of apps through Zapier's automation platform

<br />

## 🔐 <a name="security"></a>Security

Security-focused tools for authentication, secrets management, and vulnerability scanning.

- <img src="https://1password.com/favicon.ico" height="14"/> [1Password](https://github.com/1password/mcp-server-1password) - Access secrets and items in 1Password vaults
- <img src="https://aquasecurity.github.io/favicon.ico" height="14"/> [Aqua Security](https://github.com/aquasecurity/mcp-aqua) - Scan containers and code for security vulnerabilities
- <img src="https://www.hashicorp.com/favicon.ico" height="14"/> [HashiCorp Vault](https://github.com/LostInBrittany/mcp-server-vault) - Access HashiCorp Vault for secrets management
- <img src="https://nessus.tenable.com/favicon.ico" height="14"/> [Nessus](https://github.com/IvanFromOdessa/nessus-mcp-server) - Interact with Nessus for vulnerability scanning and management
- <img src="https://portswigger.net/favicon.ico" height="14"/> [PortSwigger Burp Suite](https://github.com/PortSwigger/mcp-server) - AI-powered web vulnerability scanning using Burp Suite
- <img src="https://snyk.io/favicon.ico" height="14"/> [Snyk](https://github.com/snyk/snyk-mcp) - Security and code analysis using Snyk
- <img src="https://www.sonarqube.org/favicon.ico" height="14"/> [SonarQube](https://github.com/SonarSource/sonarqube-mcp-server) - Code quality and security analysis using SonarQube

<br />

## 🗺️ <a name="location--maps"></a>Location & Maps

Geographic data, mapping services, and location-based tools.

- <img src="https://www.google.com/favicon.ico" height="14"/> [Google Maps](https://github.com/modelcontextprotocol/servers/tree/main/src/google-maps) - Location services, directions, and place details
- <img src="https://www.here.com/favicon.ico" height="14"/> [HERE Maps](https://github.com/heremaps/here-mcp-server) - HERE Maps Platform API for location-based services
- <img src="https://nominatim.org/favicon.ico" height="14"/> [Nominatim](https://github.com/ericselin/mcp-server-nominatim) - OpenStreetMap Nominatim for geocoding
- <img src="https://www.openstreetmap.org/favicon.ico" height="14"/> [OpenStreetMap](https://github.com/webcoderz/MCP-Geo) - Geocoding using OpenStreetMap Nominatim API
- <img src="https://www.mapbox.com/favicon.ico" height="14"/> [Mapbox](https://github.com/mapbox/mcp-server) - Maps, geocoding, navigation, and geospatial analysis
- <img src="https://weatherapi.com/favicon.ico" height="14"/> [Weather](https://github.com/adhikasp/mcp-weather) - Get current and forecast weather using AccuWeather API

<br />

## 🌿 <a name="version-control"></a>Version Control

Tools for managing code repositories and version control systems.

- <img src="https://github.githubassets.com/favicon.ico" height="14"/> [GitHub](https://github.com/modelcontextprotocol/servers/tree/main/src/github) - Repository management, file operations, and GitHub API integration
- <img src="https://about.gitlab.com/ico/favicon.ico" height="14"/> [GitLab](https://github.com/yoda-digital/mcp-gitlab-server) - Interact with GitLab repositories, issues, and CI/CD pipelines
- <img src="https://git-scm.com/favicon.ico" height="14"/> [Git](https://github.com/modelcontextprotocol/servers/tree/main/src/git) - Tools to read, search, and manipulate Git repositories
- <img src="https://bitbucket.org/favicon.ico" height="14"/> [Bitbucket](https://github.com/gauthierpetetin-hashicorp/mcp-server-bitbucket) - Interact with Bitbucket repositories

<br />

## 📋 <a name="project-management"></a>Project Management

Tools for managing projects, tasks, and workflows.

- <img src="https://www.atlassian.com/favicon.ico" height="14"/> [Jira](https://github.com/sooperset/mcp-atlassian) - Interact with Atlassian Jira for project management
- <img src="https://www.atlassian.com/favicon.ico" height="14"/> [Confluence](https://github.com/sooperset/mcp-atlassian) - Interact with Atlassian Confluence for documentation management
- <img src="https://asana.com/favicon.ico" height="14"/> [Asana](https://github.com/roychri/mcp-server-asana) - Create and manage tasks and projects in Asana
- <img src="https://linear.app/favicon.ico" height="14"/> [Linear](https://github.com/jerhadf/linear-mcp-server) - Linear project management integration
- <img src="https://monday.com/favicon.ico" height="14"/> [Monday.com](https://github.com/sakce/mcp-server-monday) - Interact with Monday.com boards and items
- <img src="https://trello.com/favicon.ico" height="14"/> [Trello](https://github.com/nishikantparmariam/trello-mcp) - Interact with Trello boards, lists, and cards
- <img src="https://clickup.com/favicon.ico" height="14"/> [ClickUp](https://github.com/taazkareem/clickup-mcp-server) - Create, update, delete and manage tasks in ClickUp

<br />

## 📧 <a name="email"></a>Email

Email management and automation tools.

- <img src="https://www.google.com/favicon.ico" height="14"/> [Gmail](https://github.com/pyautoml/gmail-mcp-server) - Read, compose, and manage Gmail emails
- <img src="https://www.google.com/favicon.ico" height="14"/> [Google Gmail](https://github.com/JasonGuoo/mcp-gmail) - Access and interact with Gmail
- <img src="https://www.microsoft.com/favicon.ico" height="14"/> [Microsoft Outlook](https://github.com/hannesrudolph/outlook-mcp-server) - Interact with Microsoft Outlook emails and calendar
- <img src="https://www.mailchimp.com/favicon.ico" height="14"/> [Mailchimp](https://github.com/aaronsb/mcp-mailchimp) - Interact with Mailchimp for email marketing campaigns
- <img src="https://sendgrid.com/favicon.ico" height="14"/> [SendGrid](https://github.com/AidanHanda/sendgrid-mcp) - Send emails with SendGrid
- <img src="https://postmarkapp.com/favicon.ico" height="14"/> [Postmark](https://github.com/ActiveCampaign/postmark-mcp) - Interact with Postmark for transactional email services
- <img src="https://resend.com/favicon.ico" height="14"/> [Resend](https://github.com/resend/mcp-send-email) - Send emails with the Resend API

<br />

## 🎨 <a name="design--media"></a>Design & Media

Tools for design, media creation, and asset management.

- <img src="https://www.figma.com/favicon.ico" height="14"/> [Figma](https://github.com/GLips/Figma-Context-MCP) - Access Figma designs and components
- <img src="https://www.figma.com/favicon.ico" height="14"/> [Figma Dev Mode](https://github.com/figma/figma-developer-mcp) - Give Claude direct access to Figma file data to implement your designs
- <img src="https://canva.com/favicon.ico" height="14"/> [Canva](https://github.com/surajsau/mcp-canva) - Create and manage designs in Canva
- <img src="https://blender.org/favicon.ico" height="14"/> [Blender](https://github.com/ahujasid/blender-mcp) - Connect to Blender for 3D modeling and rendering
- <img src="https://giphy.com/favicon.ico" height="14"/> [GIPHY](https://github.com/iamucil/giphy-mcp-server) - Search and retrieve GIFs from GIPHY
- <img src="https://images.ctfassets.net/lzny33ho1g45/6OBBqSoGjhHJXGKyBPBRhN/027745e21eb96e8e91a43fa64c69f3bc/Unsplash_app_icon.png" height="14"/> [Unsplash](https://github.com/bhawkyard1/unsplash-mcp-server) - Search and retrieve high-quality photos from Unsplash
- <img src="https://cloudinary.com/favicon.ico" height="14"/> [Cloudinary](https://github.com/cloudinary-labs/cloudinary-mcp-server) - Manage and optimize media assets in Cloudinary
- <img src="https://www.adobe.com/favicon.ico" height="14"/> [Adobe Photoshop](https://github.com/Pvpkishore/Adobe-Photoshop-MCP) - Control and automate Adobe Photoshop workflows

<br />

## 🔬 <a name="research--science"></a>Research & Science

Tools for scientific research, data analysis, and academic resources.

- <img src="https://arxiv.org/favicon.ico" height="14"/> [arXiv](https://github.com/blazickjp/arxiv-mcp-server) - Search and retrieve academic papers from arXiv
- <img src="https://europepmc.org/favicon.ico" height="14"/> [EuropePMC](https://github.com/tuannvm/mcp-europepmc) - Search and retrieve biomedical literature from Europe PMC
- <img src="https://www.ncbi.nlm.nih.gov/favicon.ico" height="14"/> [PubMed](https://github.com/andybrandt/mcp-simple-pubmed) - Search and retrieve biomedical literature from PubMed
- <img src="https://www.semanticscholar.org/favicon.ico" height="14"/> [Semantic Scholar](https://github.com/andybrandt/mcp-semanticscholar) - Search and retrieve academic papers from Semantic Scholar
- <img src="https://www.wolframalpha.com/favicon.ico" height="14"/> [Wolfram Alpha](https://github.com/SecretiveShell/MCP-wolfram-alpha) - Access computational intelligence with Wolfram Alpha

<br />

## 💹 <a name="finance"></a>Finance

Financial data, market information, and economic tools.

- <img src="https://alphavantage.co/favicon.ico" height="14"/> [Alpha Vantage](https://github.com/calvernaz/alphavantage) - Stock market data and financial information
- <img src="https://www.coinbase.com/favicon.ico" height="14"/> [Coinbase](https://github.com/coinbase/coinbase-mcp) - Interact with Coinbase for cryptocurrency trading and management
- <img src="https://coingecko.com/favicon.ico" height="14"/> [CoinGecko](https://github.com/tooyipjee/tokenstats-mcp) - CoinGecko API integration for crypto market data and analytics
- <img src="https://www.investopedia.com/favicon.ico" height="14"/> [Investopedia Terms](https://github.com/SEJeff/mcp_investopedia_terms) - Financial definitions from Investopedia
- <img src="https://www.meelion.com/favicon.ico" height="14"/> [Meelion MCP](https://github.com/Meelion-com/meelion-mcp) - Brazilian fixed income & financial data for AI — Selic, CDI, IPCA, CDB/LCI/LCA rankings, FX rates (USD, EUR), gold and Bitcoin quotes via JSON-RPC. No scraping, structured payloads ready for LLMs.
- <img src="https://openbb.co/favicon.ico" height="14"/> [OpenBB](https://github.com/OpenBB-finance/mcp-for-openbb) - MCP server for OpenBB, the open source financial data platform
- <img src="https://polygon.io/favicon.ico" height="14"/> [Polygon](https://github.com/polygon-io/mcp-polygon) - Access financial market data via the Polygon.io API
- <img src="https://www.tiingo.com/favicon.ico" height="14"/> [Tiingo](https://github.com/mattlinnell/tiingo-mcp) - Access financial data for stocks, mutual funds, and ETFs

<br />

## 🧠 <a name="knowledge--memory"></a>Knowledge & Memory

Tools for managing and querying knowledge bases and memory systems.

- <img src="https://mem0.ai/favicon.ico" height="14"/> [Mem0](https://github.com/mem0ai/mem0-mcp) - Personalized AI memory layer for storing and retrieving user preferences
- <img src="https://www.notion.so/favicon.ico" height="14"/> [Notion](https://github.com/v-3/notion-server) - Interact with Notion for knowledge management
- <img src="https://obsidian.md/favicon.ico" height="14"/> [Obsidian](https://github.com/calclavia/mcp-obsidian) - Read and search through Markdown notes in Obsidian vaults
- [Memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) - Knowledge graph-based persistent memory system
- [Qdrant](https://github.com/qdrant/mcp-server-qdrant) - Implement semantic memory layer using the Qdrant vector search engine
- [Zep](https://github.com/getzep/zep-mcp) - Long-term memory storage and retrieval for AI applications

<br />

## 🔧 <a name="developer-tools"></a>Developer Tools

Tools and utilities for software development and debugging.

- <img src="https://codeium.com/favicon.ico" height="14"/> [Codeium](https://github.com/Exafunction/codeium-mcp) - AI-powered code completion and search
- <img src="https://www.elastic.co/favicon.ico" height="14"/> [Elastic APM](https://github.com/elastic/elastic-otel-node/tree/main/packages/mcp-server-elastic-otel-node) - Interact with Elastic APM for application performance monitoring
- <img src="https://eslint.org/favicon.ico" height="14"/> [ESLint](https://github.com/zereight/mcp-eslint) - Run ESLint on code for linting and style checking
- <img src="https://github.githubassets.com/favicon.ico" height="14"/> [GitHub Copilot](https://github.com/github/github-mcp-server) - Interact with GitHub APIs via GitHub Copilot
- <img src="https://insomnia.rest/favicon.ico" height="14"/> [Insomnia](https://github.com/Kong/insomnia-mcp) - Interact with Insomnia for API testing and development
- <img src="https://www.postman.com/favicon.ico" height="14"/> [Postman](https://github.com/danivpv/postman-mcp) - Interact with Postman for API development and testing
- <img src="https://www.sonarqube.org/favicon.ico" height="14"/> [SonarQube](https://github.com/SonarSource/sonarqube-mcp-server) - Code quality analysis using SonarQube
- <img src="https://swagger.io/favicon.ico" height="14"/> [Swagger](https://github.com/RocketRider/mcp-swagger) - Interact with Swagger/OpenAPI specifications
- [Nix](https://github.com/utensils/nixmcp) - Interact with the Nix package manager
- [Package Version](https://github.com/sammcj/mcp-package-version) - Recommend correct package versions when writing code
- [Sequential Thinking](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking) - Dynamic and reflective problem-solving through thought sequences
- [Semgrep](https://github.com/semgrep/mcp) - Interact with Semgrep for static analysis and code scanning
- [Code Sandbox](https://github.com/Automata-Labs-team/MCP-Server-Playwright) - Execute Python code in a secure sandbox environment

<br />

## 🎮 <a name="gaming"></a>Gaming

Tools for game development and gaming-related integrations.

- <img src="https://steamcommunity.com/favicon.ico" height="14"/> [Steam](https://github.com/tur-learning/steam-mcp-server) - Access Steam game information and user data
- <img src="https://unity.com/favicon.ico" height="14"/> [Unity](https://github.com/CoderGamester/mcp-unity) - Interface with the Unity Editor for game development
- <img src="https://minecraft.net/favicon.ico" height="14"/> [Minecraft](https://github.com/codeium/minecraft-mcp-server) - Interact with Minecraft for building and gameplay automation

<br />

## 🏥 <a name="healthcare"></a>Healthcare

Tools for healthcare data, medical information, and patient management.

- <img src="https://www.fhir.org/favicon.ico" height="14"/> [FHIR](https://github.com/flexpa/sero/tree/main/packages/mcp) - Access healthcare data using FHIR standard
- <img src="https://www.nlm.nih.gov/favicon.ico" height="14"/> [MedlinePlus](https://github.com/simonwmatthews/mcp_medlineplus) - Access medical information from MedlinePlus

<br />

## 📱 <a name="mobile"></a>Mobile

Tools for mobile app development and device interaction.

- <img src="https://developer.apple.com/favicon.ico" height="14"/> [iOS Simulator](https://github.com/joshuayoes/ios-simulator-mcp) - Interact with iOS simulators for app testing
- <img src="https://www.android.com/favicon.ico" height="14"/> [Android](https://github.com/minhalvp/android-mcp-server) - Interact with Android devices for app development and testing

<br />

## 🌐 <a name="language--translation"></a>Language & Translation

Language processing, translation, and localization tools.

- <img src="https://www.deepl.com/favicon.ico" height="14"/> [DeepL](https://github.com/mzxrai/mcp-deepl) - Translate text using the DeepL API
- <img src="https://www.google.com/favicon.ico" height="14"/> [Google Translate](https://github.com/jparkerweb/mcp-google-translate) - Translate text using Google Translate

<br />

## 🎵 <a name="entertainment"></a>Entertainment

Entertainment and media consumption tools.

- <img src="https://open.spotify.com/favicon.ico" height="14"/> [Spotify](https://github.com/varunneal/spotify-mcp) - Connect to Spotify to control playback and view tracks, artists, playlists, and albums
- <img src="https://www.youtube.com/favicon.ico" height="14"/> [YouTube](https://github.com/kimtaeyoon83/mcp-server-youtube-transcript) - Retrieve YouTube subtitles and transcripts for AI analysis
- <img src="https://www.imdb.com/favicon.ico" height="14"/> [IMDb](https://github.com/mzxrai/mcp-imdb) - Search for movie and TV show information on IMDb

<br />

## 🛒 <a name="e-commerce"></a>E-Commerce

Tools for e-commerce platforms and online retail.

- <img src="https://www.shopify.com/favicon.ico" height="14"/> [Shopify](https://github.com/shopify/dev-mcp) - Interact with Shopify APIs for e-commerce management

<br />

## 🔌 <a name="iot--hardware"></a>IoT & Hardware

Tools for IoT devices, smart home, and hardware integration.

- <img src="https://www.home-assistant.io/favicon.ico" height="14"/> [Home Assistant](https://github.com/tevonsb/homeassistant-mcp) - Interact with Home Assistant for smart home automation
- <img src="https://www.raspberrypi.com/favicon.ico" height="14"/> [Raspberry Pi](https://github.com/Synaptic-Labs-AI/mcp-server-rpi) - Control and monitor Raspberry Pi devices
- <img src="https://www.arduino.cc/favicon.ico" height="14"/> [Arduino](https://github.com/hardcnc/arduino-mcp) - Interact with Arduino boards for hardware programming

<br />

## 📰 <a name="news--media"></a>News & Media

Tools for accessing and analyzing news and media content.

- <img src="https://newsapi.org/favicon.ico" height="14"/> [NewsAPI](https://github.com/pskill9/news-server) - Access and search for news articles using NewsAPI
- <img src="https://www.reddit.com/favicon.ico" height="14"/> [Reddit](https://github.com/adhikasp/mcp-reddit) - Read and interact with Reddit content

<br />

## 🧪 <a name="testing--qa"></a>Testing & QA

Tools for software testing and quality assurance.

- <img src="https://www.browserstack.com/favicon.ico" height="14"/> [BrowserStack](https://github.com/browserstack/mcp-server-browserstack) - Access BrowserStack for cross-browser testing
- <img src="https://playwright.dev/favicon.ico" height="14"/> [Playwright](https://github.com/executeautomation/mcp-playwright) - Browser testing and automation using Playwright

<br />

## 🏢 <a name="enterprise-systems"></a>Enterprise Systems

Enterprise resource planning and business management systems.

- <img src="https://www.sap.com/favicon.ico" height="14"/> [SAP](https://github.com/mario-andreschak/mcp-abap-abap-adt-api) - Interact with SAP ABAP systems using the ADT API
- <img src="https://www.servicenow.com/favicon.ico" height="14"/> [ServiceNow](https://github.com/osomai/servicenow-mcp) - Interact with ServiceNow for IT service management
- <img src="https://www.oracle.com/favicon.ico" height="14"/> [Oracle ERP](https://github.com/harshitsharma1250/oracle-erp-mcp-server) - Interact with Oracle ERP for enterprise resource planning

<br />

## 🌍 <a name="environment--sustainability"></a>Environment & Sustainability

Tools for environmental data, sustainability monitoring, and green tech.

- <img src="https://www.carboninterface.com/favicon.ico" height="14"/> [Carbon Interface](https://github.com/oleander/carbon-mcp-server) - Calculate carbon footprints using Carbon Interface API
- <img src="https://www.openaq.org/favicon.ico" height="14"/> [OpenAQ](https://github.com/openaq/openaq-mcp) - Access global air quality data from OpenAQ

<br />

## 🤝 <a name="customer-support"></a>Customer Support

Tools for customer support and helpdesk management.

- <img src="https://www.freshdesk.com/favicon.ico" height="14"/> [Freshdesk](https://github.com/kshitizsaini113/freshdesk-mcp) - Interact with Freshdesk for customer support management
- <img src="https://www.zendesk.com/favicon.ico" height="14"/> [Zendesk](https://github.com/reminia/mcp-zendesk) - Interact with Zendesk for customer support management

<br />

## 🎓 <a name="education"></a>Education

Educational tools, learning platforms, and knowledge resources.

- <img src="https://www.duolingo.com/favicon.ico" height="14"/> [Duolingo](https://github.com/Lorhlona/duolingomcp) - Interact with Duolingo for language learning
- <img src="https://moodle.org/favicon.ico" height="14"/> [Moodle](https://github.com/moodlehq/moodle-local_ai_manager) - Integrate with Moodle for e-learning management

<br />

## 📦 <a name="package-management"></a>Package Management

Tools for managing software packages and dependencies.

- <img src="https://www.npmjs.com/favicon.ico" height="14"/> [npm](https://github.com/danijmoss/npm-mcp-server) - Interact with npm for JavaScript package management
- <img src="https://pypi.org/favicon.ico" height="14"/> [PyPI](https://github.com/chrishaynes21/mcp-server-pypi) - Interact with PyPI for Python package management

<br />

## 🖥️ <a name="operating-system-interaction"></a>Operating System Interaction

Tools for interacting with operating system functions and system resources.

- [Everything](https://github.com/modelcontextprotocol/servers/tree/main/src/everything) - MCP server that exercises all MCP features
- [Time](https://github.com/modelcontextprotocol/servers/tree/main/src/time) - Time and timezone conversion capabilities
- [Desktop Commander](https://github.com/wonderwhy-er/DesktopCommanderMCP) - Manages terminal sessions and processes, allowing for file system search and diff/patch file editing

<br />

## 🚗 <a name="transportation"></a>Transportation

Tools for transportation, logistics, and mobility services.

- <img src="https://www.uber.com/favicon.ico" height="14"/> [Uber](https://github.com/apimatic/uber-mcp-server) - Interact with Uber for ride booking and management

<br />

## 🧰 <a name="miscellaneous"></a>Miscellaneous

Other useful MCP servers that don't fit into specific categories.

- <img src="https://www.calculator.net/favicon.ico" height="14"/> [Calculator](https://github.com/githubhenry/mcp-calculator) - Perform mathematical calculations
- <img src="https://www.random.org/favicon.ico" height="14"/> [Random.org](https://github.com/jasonjmcghee/mcp-random) - Generate random numbers and data using Random.org API
- [Markdown](https://github.com/zcaceres/markdownify-mcp) - Converts almost any file or URL to Markdown

<br />

---

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="https://creativecommons.org/publicdomain/zero/1.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1" alt=""></a></p>

To the extent possible under law, the authors have waived all copyright and related or neighboring rights to this work.
