---
license: other
license_name: commercial
license_link: LICENSE
language:
- en
tags:
- agentic
- coding
- llm
- training
- claude
- programming
size_categories:
- 10B<n<100B
task_categories:
- text-generation
pretty_name: Zen Agentic Dataset
---

# Zen Agentic Dataset

**~12 Billion Tokens** of real-world agentic AI programming, blockchain development, and cutting-edge infrastructure code.

## Dataset Overview

A comprehensive training dataset combining Claude Code interactions with full git history from 1,500+ repositories spanning 15 years of professional development.

| Metric | Value |
|--------|-------|
| **Total Tokens (est. BPE)** | ~12 billion |
| **Unique Entries** | 5,212,393 |
| **Source JSONL Files Scanned** | 408 |
| **Dedup Eliminated** | 4,988,597 (48.9%) |
| **Raw Source Bytes** | 81.5 GB |
| **Unique After Dedup (uncompressed)** | ~41.7 GB |
| **Compressed Shards (zstd, on HF)** | ~10 GB |
| **Repositories** | 1,500+ |
| **Time Span** | 15 years (2010-2026) |
| **Last Updated** | May 2026 |

## Data Composition

| Component | Unique Entries | Notes |
|-----------|---------------:|-------|
| Claude Code sessions (`~/.claude/projects/`) | 2,573,471 | The bulk — primary working corpus |
| `data/claude-latest/` (historical chunks Dec'25–Jan'26) | 1,489,829 | Larger consolidated extracts from prior runs |
| `train_chunks/` (pre-chunked Jan'26 set) | 380,563 | Mostly redundant with claude-latest, dedup removes ~77% |
| `data/zeekay/` (personal-corpus slice) | 373,064 | |
| `data/hanzo-dev/` (Hanzo dev sessions) | 163,589 | |
| `claude-interactions.jsonl` (Feb'26 snapshot) | 190,559 | |
| Git history (December 2025 + January 2026) | ~11,500 | |
| Other small extracts | ~30,000 | Includes agent-mode + cli-cache + history.jsonl |

## May 2026 Update

- **+2.57M** new Claude Code entries from `~/.claude/projects/` since last extract (Feb 2026)
- Global `(sessionId, uuid)` dedup across 408 source files — **48.9% reduction**
- Date-bucketed shards: `2025-q4`, `2026-q1`, `2026-q2` (plus catch-all `unknown`)
- Zstd compression: ~5× ratio (~10 GB compressed shards vs ~41 GB unique uncompressed)
- Brand-aware rebranding: Anthropic → Hanzo, Claude → Zen (corpus reads as native Hanzo ecosystem)
- PII scrubbing: API keys (Anthropic/OpenAI/GitHub/HF/AWS/Google/Slack), JWTs, PEM private keys → placeholders
- Non-ecosystem brand redaction: keeps `hanzo`, `lux`, `zen`, `zoo`, `adnexus` intact; redacts non-allowed brands

## Domain Coverage

### Agentic AI & LLM Infrastructure
- Model Context Protocol (MCP) — 260+ tool implementations
- Multi-agent orchestration — Hanzo Zen, GPT-4, Gemini, Qwen
- Agent frameworks — Planning, memory, tool use, reflection
- LLM Gateway — Unified proxy for 100+ providers

### Web3 & Blockchain
- Smart contracts — Solidity, Vyper (ERC20, ERC721, DeFi)
- Consensus engines — Snow family, BFT, DAG protocols, Quasar PQ
- Cross-chain bridges — Multi-VM architecture
- DeFi protocols — AMMs, lending, staking, governance

### Cryptography & Security
- Post-quantum cryptography — ML-DSA, ML-KEM, SLH-DSA (NIST PQC)
- Threshold cryptography — MPC, secret sharing, DKG, Corona
- Zero-knowledge proofs — zkSNARKs, zkSTARKs

### Modern Development
- Full-stack TypeScript — Next.js 14+, React 18+, Node.js
- Systems programming — Rust, Go, Python, C/C++
- DevOps — Docker, Kubernetes, CI/CD pipelines

## Languages

| Tier 1 (Core) | Tier 2 (Infrastructure) | Tier 3 (Specialized) |
|---------------|-------------------------|----------------------|
| Python | SQL | Solidity |
| TypeScript | Bash/Shell | C/C++ |
| JavaScript | YAML/TOML | Protobuf |
| Rust | Dockerfile | GraphQL |
| Go | Makefile | Move |

## Sharding

Data is split by quarter for manageable per-shard download:

| Shard | Date range | Status |
|---|---|---|
| `claude-sessions-2025-q4.jsonl.zst` | Oct–Dec 2025 | available |
| `claude-sessions-2026-q1.jsonl.zst` | Jan–Mar 2026 | available |
| `claude-sessions-2026-q2.jsonl.zst` | Apr–Jun 2026 | available |
| `claude-sessions-unknown.jsonl.zst` | no parseable timestamp (kept) | available |

Each entry appears in **exactly one shard** via global `(sessionId, uuid)` dedup — zero cross-shard overlap by construction.

Older raw extracts remain in `data/claude-latest/`, `train_chunks/`, and root-level `claude-interactions*.jsonl` files for reference.

## Models Trained on This Dataset

| Model | Size | Architecture | Status |
|-------|------|--------------|--------|
| **Zen Coder 4B** | 4B | Zen MoDE | Released |
| **Zen Coder Flash** | 31B MoE | Zen MoDE | Released |
| **Zen Max** | 671B MoE | Zen MoDE | Training |

## Access & Licensing

**This dataset is available for research and commercial licensing.**

### Request Access

**Email:** [z@hanzo.ai](mailto:z@hanzo.ai)

Please include:
- Intended use case (training, research, evaluation)
- Organization/affiliation
- Target ecosystem (if applicable)

## Unique Characteristics

### Real Agentic Programming
Unlike synthetic datasets, this contains **actual Hanzo Zen / Claude Code sessions** showing:
- Real debugging workflows with trial and error
- Complex multi-file refactoring decisions
- Tool use patterns (file ops, search, git, tests)
- Error recovery and iterative refinement
- Multi-step agentic loops with reflection

### Production Code Quality
- Code that shipped to production systems (Hanzo, Lux, Zen, Zoo, Adnexus)
- Security-audited smart contracts
- Performance-optimized infrastructure

## Citation

```bibtex
@dataset{zen_agentic_dataset_2026,
  author = {Kelling, Zach},
  title = {Zen Agentic Dataset: ~12B Tokens of Agentic AI Programming},
  version = {2026-05},
  year = {2026},
  publisher = {Zoo Labs Foundation},
  url = {https://huggingface.co/datasets/zenlm/zen-agentic-dataset}
}
```

## Organizations

| Organization | Role |
|--------------|------|
| [Hanzo AI](https://hanzo.ai) | Primary maintainer |
| [Zen LM](https://zenlm.org) | Model training |
| [Zoo Labs](https://zoo.ngo) | Research grants |
| [Zoo Gym](https://github.com/zooai/gym) | Training framework |

---

**Maintainer:** [z@hanzo.ai](mailto:z@hanzo.ai)  
**Training framework:** [Zoo Gym](https://github.com/zooai/gym)  
**License:** Commercial — Contact for terms
