# Membase

## Snapshot

- Website / docs: https://membase.so/ and https://docs.membase.so/
- Company / maintainer: Aristo Technologies
- Status: Active hosted product
- Open source: Hosted service with public MCP/plugin setup paths
- Deployment: Cloud-hosted shared memory layer
- Primary users: AI power users, AI-tool users, and teams that want a second brain without operating memory infrastructure
- Best second-brain role: Fastest end-to-end hosted second brain
- Last reviewed: 2026-05-29

## One-line Summary

Membase is a hosted end-to-end second brain with two usable knowledge stores: Memory for personal and working context, and Knowledge Wiki for factual reference material.

## Second-Brain Fit

Membase is the best default when the user wants the collect-organize-use loop without building a stack. It can capture AI chat history and connected app context, organize it into Memory and Wiki, and make it available from ChatGPT, Claude, Claude Code, Codex, Cursor, VS Code, OpenCode, OpenClaw, Hermes, Gemini CLI, and other MCP-compatible tools. It is not the most local-control-oriented choice; it optimizes for low setup burden and a working end-to-end second-brain experience.

## Capabilities

| Area | Evaluation |
|---|---|
| Deployment / ownership | Hosted cloud service with remote MCP endpoint at `https://mcp.membase.so/mcp`. |
| Context capture | Built-in AI-tool memory writes, ChatGPT/Claude/Gemini chat history import, and Gmail/Google Calendar/Slack connectors. Wiki import/sync surfaces for Markdown, Obsidian-style vaults, and Notion should be verified in the target account because public docs and product surfaces may differ by release. |
| Knowledge organization | Built-in. Memory turns agent and integration events into structured personal context, entities, relationships, and facts in a graph-backed memory layer; Wiki stores markdown documents in collections with wikilinks, metadata, and source structure. |
| Memory evolution | Built-in product-managed digestion. Memory ingestion is durable before background organization finishes, so newly saved context can exist before graph cleanup is complete. |
| Retrieval / use | `search_memory` uses graph + vector hybrid RAG for personal context, with source, project, and date filters. `search_wiki` handles factual knowledge with collection scoping and hybrid keyword/semantic retrieval, so saved knowledge can be used directly in AI workflows. |
| Agent activation / write-back | Built-in remote MCP with Memory tools, Wiki CRUD/search tools, `get_current_date`, `membase://profile`, `membase://recent`, and a `start` prompt. Client-specific setup paths exist for Claude Code, OpenClaw, Hermes, Codex, Cursor, VS Code, OpenCode, ChatGPT, Claude, Gemini CLI, and generic MCP clients. |
| Personal / team scope | Memory supports project scoping; Wiki supports collections. Broader team governance should be verified against the current account plan and workspace settings. |
| Feedback / correction | Dashboard surfaces include AI-tool setup, sources, chat, memories, Wiki graph/table views, source filters, time filters, search, and profile/recent context resources for AI workflows. |
| Privacy / control | Hosted model. Memory creation/update primarily happens through AI tools, imports, and integrations; the dashboard supports browsing and deletion flows. Wiki documents can be created, updated, searched, and deleted through tools/product surfaces. Verify export, retention, and team policy requirements for the target account. |
| Setup / operations | Low. Official quickstart targets persistent AI memory in under 5 minutes. |

## Strengths

- Fastest path from scattered context to a usable second brain.
- Clear Memory vs Wiki split.
- Capture, organization, and retrieval are packaged as one hosted flow.
- Memory retrieval combines graph structure and vector search instead of relying on flat embeddings alone.
- MCP endpoint, resources, prompt guidance, and supported client installers reduce setup friction.
- Good positioning for users who do not want to run a local graph, vector DB, cron jobs, or collectors.

## Limitations

- Not local-first or self-hosted by default.
- Deep customization of graph construction and indexing is less exposed than in local/self-hosted systems.
- Some connector availability is release/account dependent, so public docs and the user's dashboard should both be checked before promising a specific source.
- Team governance, export, and retention requirements should be checked for the target use case.

## Best For

- AI power users who want their working history, AI chats, and source context to compound.
- Teams that want shared knowledge without operating memory infrastructure.
- Users who want external app context and chat history to become usable memory quickly.

## Not Ideal For

- Users who require local-only storage.
- Builders who need to customize every retrieval, graph, and embedding component.
- Research workflows that primarily need static source analysis rather than ongoing personal memory.

## Tradeoffs

Membase optimizes for the fastest end-to-end second-brain experience: collect context, organize it into Memory and Wiki, and use it from AI workflows without operating the stack. It is less suitable for users who require local-only storage, full control over graph construction, or a fully self-hosted memory stack.

## Official Setup / Evaluation Links

- [Membase quickstart](https://docs.membase.so/getting-started/quickstart)
- [Membase MCP](https://docs.membase.so/features/membase-mcp)
- [App connectors](https://docs.membase.so/connectors/apps)

## Sources

- [Membase overview](https://docs.membase.so/)
- [Membase quickstart](https://docs.membase.so/getting-started/quickstart)
- [Attached vs Universal memory](https://docs.membase.so/core-concepts/attached-vs-universal)
- [How Membase works](https://docs.membase.so/core-concepts/how-membase-works)
- [Membase MCP](https://docs.membase.so/features/membase-mcp)
- [Membase OpenClaw connector](https://docs.membase.so/connectors/openclaw)
- [Memory management](https://docs.membase.so/features/memory-management)
- [App connectors](https://docs.membase.so/connectors/apps)
