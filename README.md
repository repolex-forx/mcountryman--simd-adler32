# Repolex Knowledge Graph of mcountryman/simd-adler32

RDF knowledge graph data for [mcountryman/simd-adler32](https://github.com/mcountryman/simd-adler32), parsed by [repolex](https://repolex.ai).

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
rlex download mcountryman/simd-adler32
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── d93164f98d7fe2daf883f2e1bec82778dd26199a
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── d93164f98d7fe2daf883f2e1bec82778dd26199a.nq.gz
│   └── repolex
│       └── d93164f98d7fe2daf883f2e1bec82778dd26199a
│           └── chunk-001.nq.gz
├── blob
│   ├── 04b60ebcd71226a01696179105243a55a6ab6bbb.nq.gz
│   ├── 0fd7f9ba24b0072bf228a3da5d0d5040bc41c81f.nq.gz
│   ├── 1c7c467d1e09169fffbcdd96fa9eea253c56f60c.nq.gz
│   ├── 1e3ac29f9400a116971609f9727a125c6e6d364d.nq.gz
│   ├── 262bfe9a7b0d2173ac4b9c9758ebd0ce817c137f.nq.gz
│   ├── 332261c8dca065dbfa4fc6501c28b0144421007f.nq.gz
│   ├── 36becddf57f0a93b5161a56ae313847e3c234259.nq.gz
│   ├── 3bde1f53c25bd9e57394d893c58a27fca972765f.nq.gz
│   ├── 538349a27e0a45979624e32d5d07fdb66b712467.nq.gz
│   ├── 558542bfa30f3a3c3553bf6990c9bb51e426b327.nq.gz
│   ├── 5d9caba690f071dc65dd9f9260d3d7f250986ae0.nq.gz
│   ├── 5e2f5cdb2a3b991b3ddce5f101651ebe9963fd15.nq.gz
│   ├── 610948ae3d35bcacf61087f1d4a95aea6ed0c4ea.nq.gz
│   ├── 6c9bba8cdb67013cde9406f45748a2d0577be6a2.nq.gz
│   ├── 71ff753492c1d05311824a73983f118c7bda0352.nq.gz
│   ├── 7b2cf75b8dacc08889e6b212ba43288eb0220439.nq.gz
│   ├── 7dc700858a12cd6ab7e60882187ea3a8165f7876.nq.gz
│   ├── 94364fd731f108d2b7388bc7f14cd2d230b31135.nq.gz
│   ├── 95b141e896f4173831ce3e52f42e513e01d37068.nq.gz
│   ├── 9bd65ced936a8c2e033f034063dd5584d4e78937.nq.gz
│   ├── ce606206043c4607ca00b71d45223a2c43f9d92b.nq.gz
│   ├── cfc8cb26e1f0463277e36f03e7b94a351ee7d253.nq.gz
│   ├── cffa28e54c204fcd8b17a744ba8d4912fb7b14b5.nq.gz
│   ├── d013778c454db7de3f0491ae132911ca6acff2f9.nq.gz
│   ├── d7199004d133cf6b46e0dfa7a6290d5ea494c8cb.nq.gz
│   ├── d7c743e8a29bbcf760969a5f62865400417b309d.nq.gz
│   ├── e1f2680bbc86f2a6f28242e01cf6924521c4b9b8.nq.gz
│   ├── ea8315ee9636fd1307324c5dab5b52196ffba8c6.nq.gz
│   └── f5c2f3caabed0c05323b50bb54917f170bd8b2bf.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── d93164f98d7fe2daf883f2e1bec82778dd26199a.nq.gz
├── filetree
│   └── d93164f98d7fe2daf883f2e1bec82778dd26199a.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 39 files
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

[mcountryman/simd-adler32](https://github.com/mcountryman/simd-adler32)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
