<div align="center">

# Awesome AI Second Brain

[![Context Engineering Banner](assets/awesome-second-brain.png)](https://membase.so/?utm_source=github&utm_medium=awesome-second-brain)

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)

[![Follow on X](https://img.shields.io/badge/Follow%20on%20X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/mem_base)
[![Follow on LinkedIn](https://img.shields.io/badge/Follow%20on%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/aristotechnologies)
[![Join Discord](https://img.shields.io/badge/Join%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/invite/vRp5Zh3HGu)

English | [한국어](README.ko.md)

</div>

> Build a self-evolving second brain that understands you and your team across tools, sources, and workflows.

A curated comparison of second brain, AI memory, and knowledge systems for people who want AI to understand their personal context, team knowledge, and working history. It focuses on the full lifecycle: collecting scattered context, organizing it into durable knowledge, keeping it fresh over time, and making it useful when people or AI tools work.

## Second-Brain Lifecycle

Use this repo to decide how you want your second brain to work end to end:

| Stage | Key question | What to compare |
|---|---|---|
| Collect | How does context from chats, docs, apps, notes, calendars, Slack, email, code, and files enter the brain? | Connectors, imports, APIs, manual notes, custom collectors |
| Organize | Does raw context become structured knowledge instead of a pile of embeddings? | Entities, facts, links, summaries, timelines, tags, Wiki/pages |
| Evolve | Does memory improve as new context arrives and old context gets stale? | Consolidation, deduping, correction, refresh, dream/maintenance loops |
| Use | Can the right context show up when a person or AI tool is doing real work? | Search, grounding, filters, citations, AI-tool access, write-back |
| Govern | Can users and teams inspect, correct, delete, export, scope, and trust the brain? | UI, provenance, activation evidence, permissions, personal/team boundaries, local/cloud control |

## Choose by Primary Constraint

These entry points are a chooser, not a taxonomy. Pick the row that matches the constraint that matters most right now; many systems appear in more than one use case.

| If your main constraint is... | Start with | Why |
|---|---|---|
| Lowest-ops end-to-end setup | [Membase](solutions/membase.md) | Hosted setup for collecting context, organizing it into Memory and Wiki, and making it usable from dashboard chat or AI workflows without running local collectors, graph jobs, or memory infrastructure. |
| Local or self-hosted control | [OpenHuman](solutions/openhuman.md), [GBrain](solutions/gbrain.md), [Hermes Agent + LLM Wiki](solutions/hermes-llm-wiki.md), [Mnemosyne](solutions/mnemosyne.md), [Khoj](solutions/khoj.md), or [Obsidian/Logseq + AI bridge](solutions/obsidian-logseq.md) | Your data can live in local files or self-hosted services, but you own more setup, sync, indexing, and maintenance work. |
| Strong knowledge organization or graph memory | [Membase](solutions/membase.md), [GBrain](solutions/gbrain.md), [Hermes Agent + LLM Wiki](solutions/hermes-llm-wiki.md), [Mnemosyne](solutions/mnemosyne.md), [Hyperspell](solutions/hyperspell.md), [Honcho](solutions/honcho.md), [Zep/Graphiti](solutions/zep-graphiti.md), or [Cognee](solutions/cognee.md) | These systems make entities, links, facts, wiki pages, context graphs, graph structure, representations, or temporal memory part of how knowledge is retrieved and maintained. |
| A developer memory API | [Mem0/OpenMemory](solutions/mem0-openmemory.md), [Honcho](solutions/honcho.md), [Hindsight](solutions/hindsight.md), [Mnemosyne](solutions/mnemosyne.md), [Supermemory](solutions/supermemory.md), [Hyperspell](solutions/hyperspell.md), [Zep/Graphiti](solutions/zep-graphiti.md), or [Cognee](solutions/cognee.md) | They expose APIs, SDKs, MCP, or managed services for app builders. |
| Bounded source research or platform-native personalization | [NotebookLM](solutions/notebooklm.md), [ChatGPT Memory](solutions/chatgpt-memory.md), or [Claude Projects/Claude Code](solutions/claude-projects-code.md) | Useful when the work lives inside one notebook, source set, or AI platform. |

## Solution Layers

Use the layer label to avoid comparing a complete second-brain app with a backend memory substrate as if they solved the same job. Classify each system by what the user adopts first: an app, a workspace, an API layer, a substrate, or a platform feature. Some systems span multiple layers; the label marks the primary role this repo evaluates.

| Layer | What it means | Examples |
|---|---|---|
| End-to-end app | Collect, organize, retrieve, and user-facing workflows are packaged together. | [Membase](solutions/membase.md), [OpenHuman](solutions/openhuman.md), [Khoj](solutions/khoj.md) |
| Local workspace | The user owns local files, wiki pages, vaults, or a self-hosted brain that agents can operate. | [GBrain](solutions/gbrain.md), [Hermes Agent + LLM Wiki](solutions/hermes-llm-wiki.md), [Obsidian/Logseq + AI bridge](solutions/obsidian-logseq.md) |
| Agent memory layer | APIs, SDKs, MCP servers, or managed services that add memory to agents or products. | [Mem0/OpenMemory](solutions/mem0-openmemory.md), [Honcho](solutions/honcho.md), [Hindsight](solutions/hindsight.md), [Mnemosyne](solutions/mnemosyne.md), [Supermemory](solutions/supermemory.md), [Hyperspell](solutions/hyperspell.md) |
| Memory substrate | Lower-level graph, retrieval, or knowledge infrastructure that applications build on. | [Zep/Graphiti](solutions/zep-graphiti.md), [Cognee](solutions/cognee.md) |
| Platform baseline | Memory or source-grounded context inside one AI platform or bounded research surface. | [ChatGPT Memory](solutions/chatgpt-memory.md), [Claude Projects/Claude Code](solutions/claude-projects-code.md), [NotebookLM](solutions/notebooklm.md) |

## Lowest-Ops End-to-End Path

[Membase](https://membase.so/?utm_source=github&utm_medium=awesome-second-brain) is a natural default starting point when your main goal is to get a useful second brain running quickly with minimal operations. It focuses on the whole loop: collect context from AI chats and connected sources, organize it into Memory and Wiki, and make that knowledge available through dashboard chat or connected AI tools. If local ownership or self-hosted infrastructure is the main requirement, start with the local workspace options instead.

## Solution Snapshot

This snapshot compares primary fit and tradeoffs across layers. For detailed lifecycle coverage across collect, organize, evolve, use, and governance, use the [Capability Matrix](comparisons/capability-matrix.md).

### End-To-End Apps

| Solution | Primary fit | Best when | Main tradeoff |
|---|---|---|---|
| [Membase](solutions/membase.md) | Hosted second brain | You want a useful cross-tool second brain without operating collectors, graph jobs, or memory infrastructure. | Hosted path means less local infrastructure control. |
| [OpenHuman](solutions/openhuman.md) | Local-first personal AI assistant | You want automatic app capture and a productized local desktop assistant. | Early beta status and local setup details may vary. |
| [Khoj](solutions/khoj.md) | Personal AI over files and notes | You want chat and search over local notes, files, documents, and web sources. | More focused on personal assistant/search than full memory governance. |

### Local Workspaces

| Solution | Primary fit | Best when | Main tradeoff |
|---|---|---|---|
| [GBrain](solutions/gbrain.md) | Local/self-hosted brain operations | You want agents to operate a structured local brain with pages, graph, timeline, CLI/MCP, and maintenance jobs. | More setup and operational ownership. |
| [Hermes Agent + LLM Wiki](solutions/hermes-llm-wiki.md) | Agent-operated Markdown wiki | You want an inspectable local wiki that an agent can compile, query, lint, and maintain. | You still own the wiki discipline and workflow design. |
| [Obsidian/Logseq + AI bridge](solutions/obsidian-logseq.md) | Human-owned local knowledge base | You want a local PKM source of truth with optional AI bridges. | AI memory behavior depends on plugins, imports, or custom bridges. |

### Agent Memory Layers

| Solution | Primary fit | Best when | Main tradeoff |
|---|---|---|---|
| [Supermemory](solutions/supermemory.md) | Hosted memory API and connectors | You need hosted memory, connectors, MCP, API, SDK, and plugins for AI workflows or products. | App owners still need to verify how retrieved context is used. |
| [Hyperspell](solutions/hyperspell.md) | Hosted company/user context layer | You need workspace context, metadata, live search, procedural memory, and agent-facing APIs. | Private beta and product availability may affect adoption. |
| [Honcho](solutions/honcho.md) | Stateful agent memory and user modeling | You need peer representations, conclusions, session context, and user or agent modeling over time. | Developer integration and hosting choices matter. |
| [Hindsight](solutions/hindsight.md) | Agent memory API with memory banks | You need memory banks, observations, consolidation, and multi-mode recall for agents. | Retrieval-to-action evidence depends on the surrounding workflow. |
| [Mnemosyne](solutions/mnemosyne.md) | Local-first agent memory layer | You need local SQLite memory with MCP, SDK, CLI, Hermes integration, tiers, and consolidation. | Local operation and agent logging still need owner attention. |
| [Mem0/OpenMemory](solutions/mem0-openmemory.md) | Developer memory engine | You need user/run-scoped memory for apps with hosted or self-hosted paths. | More of an app memory primitive than a complete second-brain workflow. |

### Memory Substrates

| Solution | Primary fit | Best when | Main tradeoff |
|---|---|---|---|
| [Zep/Graphiti](solutions/zep-graphiti.md) | Temporal graph memory substrate | You need temporal graph memory and Graph RAG under an application. | Not a complete user-facing second brain by itself. |
| [Cognee](solutions/cognee.md) | Knowledge graph memory SDK | You need graph-oriented memory infrastructure with SDK, MCP, API, plugins, or cloud paths. | Requires application or workflow integration above it. |

### Platform Baselines

| Solution | Primary fit | Best when | Main tradeoff |
|---|---|---|---|
| [ChatGPT Memory](solutions/chatgpt-memory.md) | ChatGPT-native personalization | You already live in ChatGPT and want platform-local personalization. | Platform-controlled visibility, retrieval, and export. |
| [Claude Projects/Claude Code](solutions/claude-projects-code.md) | Claude-scoped project knowledge | Your work lives inside Claude Projects, Claude Code, or Claude connectors. | Context is scoped to Claude workflows and plan/workspace controls. |
| [NotebookLM](solutions/notebooklm.md) | Source-grounded research notebook | You need grounded work over a bounded source set. | Not designed as a cross-tool evolving second brain. |

## Deep Dives

| Page | Use it for |
|---|---|
| [Chooser](comparisons/chooser.md) | Pick a starting solution by goal and tradeoff. |
| [Solution Layers](comparisons/solution-layers.md) | Separate end-to-end apps, local workspaces, agent memory layers, memory substrates, and platform baselines. |
| [Capability Matrix](comparisons/capability-matrix.md) | Compare lifecycle support, governance, operating burden, activation surfaces, and setup time. |
| [Capability Definitions](capabilities/README.md) | Understand the evaluation dimensions behind the matrix. |
| [Activation Evidence](capabilities/activation-evidence.md) | Evaluate whether retrieved memory was loaded, cited, refused, written back, or actually used. |
| [Setup Burden](comparisons/setup-burden.md) | See what you actually have to operate. |
| [Agent Activation](comparisons/agent-access.md) | Compare MCP, API, SDK, CLI, and plugin access as second-brain activation channels. |
| [Local vs Cloud](comparisons/local-vs-cloud.md) | Decide where memory should live. |
| [Personal vs Team](comparisons/personal-vs-team.md) | Compare solo, project, team, and organization fit. |
| [Setup Guides](setup-guides/README.md) | Add hands-on setup notes only after verification. |
| [Examples](examples/README.md) | Describe concrete second-brain workflows and scenarios. |
| [Watchlist](watchlist.md) | Track promising systems that are not yet fully evaluated. |

## Evaluation Labels

| Label | Meaning |
|---|---|
| Built-in | The product directly supports the workflow. |
| Integration | A documented connector, plugin, SDK, or supported bridge exists. |
| Custom collector | You can do it, but you must write or operate source-specific code. |
| Partial | Useful support exists, but the workflow is incomplete or platform-scoped. |
| Not primary fit | The solution is not designed for this workflow. |
| Unknown | The repo has not verified this claim yet. |

Setup time is tagged as `Official`, `Hands-on`, or `Maintainer estimate`. When official docs provide a quickstart but no credible time estimate, the table says that hands-on time varies.

## Sources

Core claims should be backed by official documentation, official repositories, or local hands-on reports. This repo should point to official setup docs instead of duplicating step-by-step installation instructions.

## How To Contribute

1. Pick the smallest contribution type that fits your evidence: core solution, capability/comparison update, setup guide, example, or watchlist entry.
2. Use [templates/system-profile.md](templates/system-profile.md) or [templates/capability-page.md](templates/capability-page.md).
3. Use primary sources or mark unverified fields as `Unknown`.
4. For core solution profiles, link the solution from the relevant chooser, comparison, and capability pages so readers can evaluate it through the main decision paths.
5. Open a PR with sources, verification notes, and any known limitations.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the contribution guidelines.

## Star History

<a href="https://www.star-history.com/?repos=aristoapp%2Fawesome-second-brain&type=date&legend=top-left">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=aristoapp/awesome-second-brain&type=date&theme=dark&legend=top-left" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=aristoapp/awesome-second-brain&type=date&legend=top-left" />
   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=aristoapp/awesome-second-brain&type=date&legend=top-left" />
 </picture>
</a>
