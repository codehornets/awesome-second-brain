# Context Capture

## What This Capability Means

Context capture is how raw personal, team, and source context enters the second brain: AI conversations, notes, documents, email, calendar, Slack, Drive, Notion, browser data, code, or custom events.

## Evaluation Questions

- Is capture built in, connector-based, API-based, or custom?
- Does capture preserve source, timestamp, and permissions?
- Does the system distinguish raw import from curated memory?
- Can users disconnect a source without losing needed history?

## Solution Matrix

| Solution | Support label | Adoption path | Caveats |
|---|---|---|---|
| Membase | Built-in + Integration | Agent writes, ChatGPT/Claude/Gemini chat import, Gmail/Google Calendar/Slack, and account-dependent Wiki import/sync surfaces for Markdown, Obsidian-style vaults, or Notion. | Do not present Drive, GitHub, Notion, or Obsidian as universally available without checking current docs and the target account UI. |
| OpenHuman | Built-in + Integration | 118+ OAuth integrations, auto-fetch, local Memory Tree, Markdown vault. | Beta behavior and connector reliability need hands-on verification. |
| GBrain | Built-in + Custom collector | Markdown import, capture, webhooks, source-specific collectors. | External APIs require collector work. |
| Supermemory | Built-in + Integration | MCP/API plus Drive, Gmail, Notion, OneDrive, GitHub, Web Crawler. | Connector permissions and sync state matter. |
| Mem0/OpenMemory | API + Integration | SDK/API/MCP writes from app or AI workflow. | Capture design is application-owned. |
| Zep/Graphiti | API | Chat history, business data, graph endpoints. | Requires app integration. |
| Cognee | Built-in + API | MCP memory/data tools and graph processing. | Standalone vs shared mode affects where data lands. |
| Khoj | Built-in | Files, notes, PDFs, Markdown, org-mode, Notion pages. | Better for personal source Q&A than broad cross-tool capture. |
| Obsidian/Logseq + AI bridge | Built-in notes + Integration | Local notes plus plugin/import/filesystem bridge. | Agent-ready capture depends on the bridge. |
| ChatGPT Memory | Built-in | Saved memories and reference chat history inside ChatGPT. | Not a general external source-ingestion backend. |
| Claude Projects/Claude Code | Built-in | Project uploads, project instructions, chat context, and enabled connectors. | Capture is Claude-scoped unless external memory is added. |
| NotebookLM | Built-in | Upload/import for docs, PDFs, web URLs, YouTube, audio, Gemini Chats, and other supported source types. | Imported sources can be bounded/static depending on source type. |

## Sources

- [Membase overview](https://docs.membase.so/)
- [Supermemory connectors](https://supermemory.ai/docs/connectors/overview)
- [Khoj docs](https://docs.khoj.dev/)
