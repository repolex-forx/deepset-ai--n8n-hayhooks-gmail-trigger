# Repolex Knowledge Graph of deepset-ai/n8n-hayhooks-gmail-trigger

RDF knowledge graph data for [deepset-ai/n8n-hayhooks-gmail-trigger](https://github.com/deepset-ai/n8n-hayhooks-gmail-trigger), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download deepset-ai/n8n-hayhooks-gmail-trigger
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 4f7b2d76e2600cfd1e460e982beed8395ef8cb31
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 4f7b2d76e2600cfd1e460e982beed8395ef8cb31
│           └── chunk-001.nq.gz
├── blob
│   ├── 0d666e01e04848f1ad211b8cd2b41bde57b8b415.nq.gz
│   ├── 30bdc0c8f4ae7422d736212c4d60bf8f99f14bc3.nq.gz
│   ├── 5f8350913b300ba03727ee056fbc93038b9f43e0.nq.gz
│   ├── b011ca4fbae2f2a042f2ef6dc69d1d552b024e91.nq.gz
│   ├── cd6177338082962e3d269e702d82de38361c5533.nq.gz
│   └── f142498d754c2a92acac279c1f6c0d3a6dd109bb.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 4f7b2d76e2600cfd1e460e982beed8395ef8cb31.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 12 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[deepset-ai/n8n-hayhooks-gmail-trigger](https://github.com/deepset-ai/n8n-hayhooks-gmail-trigger)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
