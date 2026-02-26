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
- 1B<n<10B
task_categories:
- text-generation
pretty_name: Zen Agentic Dataset
---

# Zen Agentic Dataset

**10.5 Billion Tokens** of real-world agentic AI programming, blockchain development, and cutting-edge infrastructure code.

## Dataset Overview

A comprehensive training dataset combining Claude Code interactions with full git history from 1,500+ repositories spanning 15 years of professional development.

| Metric | Value |
|--------|-------|
| **Total Tokens** | 10.5 billion |
| **Training Samples** | 3.5 million |
| **Validation Samples** | 156,000 |
| **Total Size** | ~120 GB |
| **Repositories** | 1,500+ |
| **Time Span** | 15 years (2010-2026) |
| **Last Updated** | February 2026 |

## Data Composition

| Component | Tokens | Percentage |
|-----------|--------|------------|
| Claude Code Debug Sessions | 2.42B | 23% |
| Claude Code Latest | 4.0B | 38% |
| Claude Conversations | 1.14B | 11% |
| Claude Interactions | 0.86B | 8% |
| Git History | 2.1B | 20% |

## February 2026 Update

- **+425** new Claude Code conversations extracted
- **+214K** total curated conversations
- Full extraction pipeline for continuous collection
- Dataset now exceeds **120 GB** raw data

## Domain Coverage

### Agentic AI & LLM Infrastructure
- Model Context Protocol (MCP) - 260+ tool implementations
- Multi-agent orchestration - Claude, GPT-4, Gemini, Zen
- Agent frameworks - Planning, memory, tool use, reflection
- LLM Gateway - Unified proxy for 100+ providers

### Web3 & Blockchain
- Smart contracts - Solidity, Vyper (ERC20, ERC721, DeFi)
- Consensus engines - Snow family, BFT, DAG protocols
- Cross-chain bridges - Multi-VM architecture
- DeFi protocols - AMMs, lending, staking, governance

### Cryptography & Security
- Post-quantum cryptography - Kyber, Dilithium, SPHINCS+
- Threshold cryptography - MPC, secret sharing, DKG
- Zero-knowledge proofs - zkSNARKs, zkSTARKs

### Modern Development
- Full-stack TypeScript - Next.js 14+, React 18+, Node.js
- Systems programming - Rust, Go, Python, C/C++
- DevOps - Docker, Kubernetes, CI/CD pipelines

## Languages

| Tier 1 (Core) | Tier 2 (Infrastructure) | Tier 3 (Specialized) |
|---------------|-------------------------|----------------------|
| Python | SQL | Solidity |
| TypeScript | Bash/Shell | C/C++ |
| JavaScript | YAML/TOML | Protobuf |
| Rust | Dockerfile | GraphQL |
| Go | Makefile | Move |

## Models Trained on This Dataset

| Model | Size | Architecture | Status |
|-------|------|--------------|--------|
| **Zen Coder 4B** | 4B | Zen | ✅ Released |
| **Zen Coder Flash** | 31B MoE | Zen Coder Flash | ✅ Released |
| **Zen Max** | 671B MoE | Zen Max | 🟢 Training |

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
Unlike synthetic datasets, this contains **actual Claude Code sessions** showing:
- Real debugging workflows with trial and error
- Complex multi-file refactoring decisions
- Tool use patterns (file ops, search, git, tests)
- Error recovery and iterative refinement

### Production Code Quality
- Code that shipped to production systems
- Security-audited smart contracts
- Performance-optimized infrastructure

## Citation

```bibtex
@dataset{zen_agentic_dataset,
  author = {Kelling, Zach},
  title = {Zen Agentic Dataset: 10.5B Tokens of Agentic AI Programming},
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

---

**Maintainer:** [z@hanzo.ai](mailto:z@hanzo.ai)  
**License:** Commercial - Contact for terms
