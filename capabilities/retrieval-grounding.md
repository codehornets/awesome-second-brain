# Retrieval / Use

## What This Capability Means

Retrieval and use cover how the system finds relevant memory, whether it can preserve source context, and whether people or AI tools can apply that context during real work.

## Evaluation Questions

- Does retrieval use keyword search, vector search, graph retrieval, RAG, or a hybrid model?
- Are source, timestamp, project, collection, and permission signals available at retrieval time?
- Can users or AI tools cite or inspect the source behind a memory?
- Can users distinguish fresh source data from stale, imported, or inferred memory?

## Solution Matrix

| Solution | Support label | Adoption path | Caveats |
|---|---|---|---|
| Membase | Built-in | Graph + vector hybrid RAG for Memory; hybrid Wiki search with source/project/date filters. | Verify source availability and current connector behavior for the target account. |
| OpenHuman | Built-in | Local Memory Tree, semantic search, Markdown vault, and context compression. | Source/provenance behavior needs hands-on verification. |
| GBrain | Built-in | Keyword search, vector/hybrid query, graph/link signals, timeline/fact retrieval, and `think` synthesis. | Quality depends on sync, embeddings, and curated source structure. |
| Supermemory | Built-in | Search, RAG, memory graph, project scoping, metadata, and API filters. | Connector and project scoping must be configured carefully. |
| Mem0/OpenMemory | Built-in | Layered memory search with user IDs, run IDs, and metadata. | App owners define grounding and source metadata quality. |
| Zep/Graphiti | Built-in | Temporal knowledge graph, facts, episodes, and Graph RAG. | Best when application data is modeled explicitly. |
| Cognee | Built-in | Knowledge graph memory and recall tools. | Retrieval quality depends on ingestion and graph processing mode. |
| Khoj | Built-in | Natural-language search and chat over files and notes. | Strong source Q&A, weaker as a broad second-brain layer across tools. |
| Obsidian/Logseq + AI bridge | Integration | Local search, backlinks, graph views, and bridge-provided RAG/search. | Grounding quality depends on the selected bridge. |
| ChatGPT Memory | Partial | Platform memory and chat history reference. | Source and retrieval internals are platform-controlled. |
| Claude Projects/Claude Code | Built-in | Project knowledge search/RAG and Claude context surfaces. | Grounding is scoped to Claude contexts and plan behavior. |
| NotebookLM | Built-in | Source-grounded notebook retrieval and source selection. | Strong for bounded source sets, weak as a live second brain across workflows. |

## Sources

- [Membase MCP](https://docs.membase.so/features/membase-mcp)
- [Zep graph documentation](https://help.getzep.com/v2/understanding-the-graph)
- [NotebookLM source docs](https://support.google.com/notebooklm/answer/16215270?hl=en)
