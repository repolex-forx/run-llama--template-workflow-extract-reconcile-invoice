# Repolex Knowledge Graph of run-llama/template-workflow-extract-reconcile-invoice

RDF knowledge graph data for [run-llama/template-workflow-extract-reconcile-invoice](https://github.com/run-llama/template-workflow-extract-reconcile-invoice), parsed by [repolex](https://repolex.ai).

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
rlex download run-llama/template-workflow-extract-reconcile-invoice
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 74792fc12acf525254508def62bf833f9493e8e9
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 74792fc12acf525254508def62bf833f9493e8e9
│           └── chunk-001.nq.gz
├── blob
│   ├── 02ef475147fd445f215358bde2bbd77bff6baaab.nq.gz
│   ├── 0d4d82c95db1f71f4d9f35b674e24e8eaa5bb5de.nq.gz
│   ├── 0dc927a0659097c006f1f8466541e6e8053be44d.nq.gz
│   ├── 1bd7e75eb30d851dfcb2a0735b070e4b5a9a0c31.nq.gz
│   ├── 1db54c3f1357df8c6f65f2ecb4bd4580bf18b551.nq.gz
│   ├── 1efcb486d494ffa8bc78af0ce405f8da160d38e2.nq.gz
│   ├── 25ad5bcbea25ab78a63bd3f3f84a66693ffa7f2f.nq.gz
│   ├── 26c86ac2d0eb0fbcc883948e7bd4faa28e8876d3.nq.gz
│   ├── 2de430f5285d9526295e1a4538c94994a2be0376.nq.gz
│   ├── 301e399e9d3cbd0a4fe02443e3b713290b8228d3.nq.gz
│   ├── 35fca6eac9cae2583c8c1de898b60f793a1ec092.nq.gz
│   ├── 3cdee003bf488e12d3a4fa4953119126da830f87.nq.gz
│   ├── 3ef840615d4640601ef02d130ad64520554f45ce.nq.gz
│   ├── 45b37fc91442a293c8805c74bf853e259bab8ed1.nq.gz
│   ├── 4da33406e72b559c03d608dd6285862cf3587d83.nq.gz
│   ├── 586e5141802a869825bffb277a53b2665d2186d2.nq.gz
│   ├── 6fa106702b614ba5fa6b97a24ff2b6c53c7f9f81.nq.gz
│   ├── 7e3d8a83eea8182c9e03bffd092477da61ee8407.nq.gz
│   ├── 800bc6ad052fd0f8c6b71ae928ab138a3f6e430a.nq.gz
│   ├── 85c9a64cc53f6202cf5a66bcb8da2b80d60a1090.nq.gz
│   ├── 881adaad2217aa75f669d37cfd3cdf46e64c56c4.nq.gz
│   ├── 88acac8845cf45be2f401aa449d0fcf2f5b786c3.nq.gz
│   ├── 97856e842efe3cace2180a4d1171b10594a84831.nq.gz
│   ├── a737ef81472ed530806f616d6d2d895df2b2b04f.nq.gz
│   ├── b1f3492860feb8fe54d06551703182c6259ca77e.nq.gz
│   ├── b56bed7e80ac87ea7ce50913ef870f0db71980f1.nq.gz
│   ├── bb158d8cbb9cee365d0948944819541b12675536.nq.gz
│   ├── c01805e89c1684e79130151abc23bb80401583a9.nq.gz
│   ├── c46dba90edea279d600d88611d5abb65b787d9e1.nq.gz
│   ├── c5da6423128173b14442dc855c06a1d535726117.nq.gz
│   ├── d8e401fe8f32fff3f18b4763baf4bb4fd63725b4.nq.gz
│   ├── e09ce2f151b1fe838738c5eb1bb415a203883070.nq.gz
│   ├── e5439b09bd058b9bbf5e3dc61d7f5eae6eb306eb.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── f900b7ec6513a252686e4363d6232bd846bb3b59.nq.gz
│   ├── fa1153bde2ddc9706c829fb272779827d49fa700.nq.gz
│   └── fc8b9169a72a1e357acb111a717f8241b282f8c8.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 74792fc12acf525254508def62bf833f9493e8e9.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 43 files
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

[run-llama/template-workflow-extract-reconcile-invoice](https://github.com/run-llama/template-workflow-extract-reconcile-invoice)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
