# Protocols & Connectors

Protocols and connectors give agents access to external data and tools. They may not store memory themselves, but they are often the ingestion and access layer that memory systems depend on.

## Systems

- Model Context Protocol (MCP)
- Filesystem connectors
- Notion connectors
- Slack connectors
- Gmail connectors
- Google Drive connectors
- GitHub connectors
- Browser and web automation connectors

## Research Questions

- Does the protocol or connector store memory, or only expose context?
- What data sources can it access?
- Can it write back to source systems?
- How does authentication and permissioning work?
- Can it be combined with a memory layer?
- Is it local, remote, or both?

## Landscape Notes

Connectors increase the amount of context an agent can access, but access is not the same as memory. A durable memory layer decides what should persist, how it should be retrieved, and who can use it later.
