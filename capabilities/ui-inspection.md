# Feedback / Correction

## What This Capability Means

Feedback and correction cover whether users can see what the system knows, filter it by useful dimensions, correct bad memories, and verify that source imports or agent writes landed where expected.

## Evaluation Questions

- Can users browse, search, filter, edit, delete, or correct memory?
- Are source, date, project, collection, or workspace filters visible?
- Can users inspect ingestion, sync, connector, or indexing status?
- Is the primary interface built for humans, developers, agents, or all three?

## Solution Matrix

| Solution | Support label | Adoption path | Caveats |
|---|---|---|---|
| Membase | Built-in | Dashboard for sources, chat, memories, Wiki graph/table views, filters, and agent setup. | Export, retention, and plan-specific governance should be verified. |
| OpenHuman | Built-in | Desktop UI, Memory Tree, Markdown vault, onboarding, voice, and app surfaces. | Early beta behavior should be tested directly. |
| GBrain | Partial | CLI and operations UI for HTTP MCP admin, jobs, request logs, calibration, and live activity. | Not a polished Notion/Roam-style knowledge UI. |
| Supermemory | Built-in | Hosted app, console, connector status, projects, and filters. | Team/admin inspection depends on plan and setup. |
| Mem0/OpenMemory | Built-in | Platform dashboard and self-hosted dashboard/server paths. | Application owners still define user-facing review flows. |
| Zep/Graphiti | Partial | Developer/platform UI and graph APIs. | End-user second-brain UI is not the primary surface. |
| Cognee | Partial | Developer/admin surfaces and MCP tool references. | End-user inspection should be verified for the target workflow. |
| Khoj | Built-in | Web, desktop, browser, and editor/client interfaces. | Inspection depends on source and deployment choices. |
| Obsidian/Logseq + AI bridge | Built-in | Graph, backlinks, tags, properties, search, pages, and blocks. | Agent writes need review discipline. |
| ChatGPT Memory | Built-in | Settings, Manage memories, memory search/sort controls, and memory sources. | Only covers ChatGPT platform memory. |
| Claude Projects/Claude Code | Built-in | Claude project UI, knowledge base, instructions, sharing controls, and RAG indicators. | Project visibility depends on workspace plan and permissions. |
| NotebookLM | Built-in | Notebook UI, sources panel, source selection, labels, and generated artifacts. | Strong inspection for imported sources, not full second-brain operations. |

## Sources

- [Membase memory management](https://docs.membase.so/features/memory-management)
- [ChatGPT Memory FAQ](https://help.openai.com/en/articles/8590148-memory-faq)
- [NotebookLM source docs](https://support.google.com/notebooklm/answer/16215270?hl=en)
