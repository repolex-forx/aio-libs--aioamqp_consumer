# Repolex Knowledge Graph of aio-libs/aioamqp_consumer

RDF knowledge graph data for [aio-libs/aioamqp_consumer](https://github.com/aio-libs/aioamqp_consumer), parsed by [repolex](https://repolex.ai).

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
rlex download aio-libs/aioamqp_consumer
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── c687211e385f7d7b3a90a042c97213d469bdaaa6
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── c687211e385f7d7b3a90a042c97213d469bdaaa6
│           └── chunk-001.nq.gz
├── blob
│   ├── 0116d381056161843e8c3cf4ffb2173b25561c1c.nq.gz
│   ├── 01e553a8acd55bbcc625be389a0f7328ca16dec4.nq.gz
│   ├── 08118c91b7f18276f53b29d0375a03da8baa9b4e.nq.gz
│   ├── 09a59fae50aea44b8839e7e532b89f844602a6e5.nq.gz
│   ├── 11f7df34ac3a2165750a9eea2aaec53b6b03545a.nq.gz
│   ├── 1286a1065b2cdf4440d95ef298ea579cfc063f70.nq.gz
│   ├── 1a873ceaaed2dd4e92ee07573c1670f6c66f67f3.nq.gz
│   ├── 2f6dac4244089aba9e809f4c5f37243ac81dbd69.nq.gz
│   ├── 3c0a4db0c41d5852bb18fc235541d3ed3d53c4ea.nq.gz
│   ├── 41fb35bb1fc4f4d78aa1cc434f103add8ec348e7.nq.gz
│   ├── 4889936ad4bcf76138219742dd77cc8777a36aee.nq.gz
│   ├── 48fb665f4758d50f4f7091bf08039b3d9d888266.nq.gz
│   ├── 5e64bebb5d5a70711e5483a163e20d6d500aa8ad.nq.gz
│   ├── 5f9d2c0c45c043d1c78832aa6cc4cff505ba7645.nq.gz
│   ├── 61f4ca74c67809f92a98438310687697fdaf3838.nq.gz
│   ├── 67383b783373c8e29f9f416e87652748678c056c.nq.gz
│   ├── 6abfb9a6eb8912a8c7e52a2e06e8173ed3350cac.nq.gz
│   ├── 70f7982fce04b0939722c5b82c0b1e59aa02d624.nq.gz
│   ├── 759c8ba34ed45dbe11669e4d91bb47ea203507b4.nq.gz
│   ├── 76f40b6d6b5046352c8393367b957c58a70f248f.nq.gz
│   ├── 875c2e72e7a9fb6f490eab58cea0db03621f68b2.nq.gz
│   ├── 8af673f14890a1fedfe260da3f387773fb7fb17d.nq.gz
│   ├── 9d0a75844a4ab6c1c1cee737c11b11afe68767d0.nq.gz
│   ├── a05be5bdbe8b77e06bcfa82d8d91bbd37104c6bc.nq.gz
│   ├── aaf74f7f9c9dd9e7dead8780c4ad1faac4d0d938.nq.gz
│   ├── ac3de2f0091a165c358dc608f3d615c211d25291.nq.gz
│   ├── be7a829f1ead0fdd88339d57f930e175becdccfd.nq.gz
│   ├── bed826ef136de9e9d4e14fb4bd95b567364f9264.nq.gz
│   ├── cd91be06a1459000c4722b446b30777d85c9c8de.nq.gz
│   ├── d73b39fa493ca44388bcd4c747b008d9a838698d.nq.gz
│   ├── daa6ffef4102a65317a0ba8db0da8a6e8b1e162d.nq.gz
│   ├── e24206f7951ce600070c653a55f024bdf4d78a08.nq.gz
│   └── f0da477fb2edc61ca8c0efc4585997036689294b.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── c687211e385f7d7b3a90a042c97213d469bdaaa6.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 41 files
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

[aio-libs/aioamqp_consumer](https://github.com/aio-libs/aioamqp_consumer)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
