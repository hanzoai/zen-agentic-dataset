# Zen Agentic Dataset

<p align="center">
  <strong>10.5 Billion Tokens</strong> of real-world agentic AI programming data
</p>

<p align="center">
  <a href="https://huggingface.co/datasets/hanzoai/zen-agentic-dataset">HuggingFace</a> •
  <a href="https://github.com/zenlm/zen-trainer">Training Framework</a> •
  <a href="mailto:z@hanzo.ai">Request Access</a>
</p>

---

## Overview

A comprehensive training dataset combining Claude Code interactions with full git history from 1,400+ repositories spanning 15 years of professional development across AI, Web3, cryptography, and modern software engineering.

## Quick Stats

| Metric | Value |
|--------|-------|
| **Total Tokens** | 10.5 billion |
| **Training Samples** | 3.5 million |
| **Claude Conversations** | 214,163+ |
| **Validation Samples** | 156,000 |
| **Total Size** | ~28 GB |
| **Repositories** | 1,500+ |
| **Time Span** | 15 years (2010-2026) |
| **Last Updated** | February 2026 |

## Data Composition

```
Claude Code Sessions        ████████████████░░░░░░░░░  42% (4.4B tokens)
Git Commit History          ████████████████████░░░░░  48% (5.0B tokens)
Claude Interactions         ████░░░░░░░░░░░░░░░░░░░░░  10% (1.0B tokens)
```

### February 2026 Update
- **+425** new Claude Code conversations extracted
- **+214K** total curated conversations now available
- **+102 MB** claude-interactions.jsonl dataset file
- Full extraction pipeline updated for continuous collection

### January 2026 Update
- **+45,308** Claude Code sessions extracted
- **+6,646** git commits from 380 active repositories
- **+2B tokens** added to training corpus

## Domain Coverage

### 🤖 Agentic AI & LLM Infrastructure
- Model Context Protocol (MCP) - 260+ tool implementations
- Multi-agent orchestration - Claude, GPT-4, Gemini, Qwen integrations
- Agent frameworks - Planning, memory, tool use, reflection
- LLM Gateway - Unified proxy for 100+ providers

### ⛓️ Web3 & Blockchain
- Smart contracts - Solidity, Vyper (ERC20, ERC721, ERC1155, DeFi)
- Consensus engines - Snow family, BFT, DAG-based protocols
- Cross-chain bridges - Multi-VM architecture
- DeFi protocols - AMMs, lending, staking, governance

### 🔐 Cryptography & Security
- Post-quantum cryptography - Kyber, Dilithium, SPHINCS+
- Threshold cryptography - MPC, secret sharing, DKG
- Zero-knowledge proofs - zkSNARKs, zkSTARKs
- Key management - HD wallets, hardware integration

### 💻 Modern Development
- Full-stack TypeScript - Next.js 14+, React 18+, Node.js
- Systems programming - Rust, Go, Python, C/C++
- DevOps - Docker, Kubernetes, CI/CD pipelines
- Real-time systems - Event sourcing, CQRS, message queues

## Languages

| Tier 1 (Core) | Tier 2 (Infrastructure) | Tier 3 (Specialized) |
|---------------|-------------------------|----------------------|
| Python | SQL | Solidity |
| TypeScript | Bash/Shell | C/C++ |
| JavaScript | YAML/TOML | Protobuf |
| Rust | Dockerfile | GraphQL |
| Go | Makefile | Move |

## Models Training on This Dataset

| Model | Size | Architecture | VRAM | Status |
|-------|------|--------------|------|--------|
| **Zen Coder 4B** | 4B | Qwen3 | 8 GB | ✅ Trained |
| **Zen Coder Flash** | 31B MoE | GLM-4.7-Flash | 24 GB | ✅ Trained |
| **Zen Coder 123B** | 123B | Devstral 2 | 128 GB | 🟢 Training |
| **Zen Max** | 671B MoE | Kimi K2 | 180 GB | 🟡 Planned |

## Access & Licensing

**This dataset is available for research and commercial licensing.**

### For Developers & Researchers

We award grants to individuals and teams who want to train models on this dataset, particularly those building:

- 🔗 Models for specific blockchain ecosystems
- 🤖 Open-source AI tools using OpenAI-compatible protocols
- 🔬 Research advancing agentic AI capabilities
- 🌐 Infrastructure for decentralized AI training/inference

### Request Access

**Email:** [z@hanzo.ai](mailto:z@hanzo.ai)

Please include:
- Intended use case (training, research, evaluation)
- Organization/affiliation
- Target ecosystem (if applicable)
- Licensing requirements

## Training Framework

Use [zen-trainer](https://github.com/zenlm/zen-trainer) for fine-tuning:

```python
from zen_trainer import ZenTrainer

trainer = ZenTrainer(
    model_key="qwen3-4b",
    dataset_path="hanzoai/zen-agentic-dataset-private",  # Requires access
    output_dir="./output/my-model",
)
trainer.train()
```

## Unique Characteristics

### Real Agentic Programming
Unlike synthetic datasets, this contains **actual Claude Code sessions** showing:
- Real debugging workflows with trial and error
- Complex multi-file refactoring decisions
- Architecture discussions and trade-offs
- Tool use patterns (file ops, search, git, tests)
- Error recovery and iterative refinement

### Production Code Quality
- Code that shipped to production systems
- Security-audited smart contracts
- Performance-optimized infrastructure
- Battle-tested patterns from real deployments

## Supported Organizations

| Organization | Focus | Role |
|--------------|-------|------|
| [Hanzo AI](https://hanzo.ai) | AI infrastructure | Primary maintainer |
| [Zen LM](https://zenlm.org) | Open model research | Model training |
| [Zoo Labs](https://zoo.ngo) | Decentralized AI | Research grants |

## Citation

```bibtex
@dataset{zen_agentic_dataset,
  author = {Kelling, Zach},
  title = {Zen Agentic Dataset: 10.5B Tokens of Agentic AI Programming},
  year = {2026},
  publisher = {Zoo Labs Foundation},
  note = {3.5M samples, 1,500+ repositories, 15 years of development},
  url = {https://github.com/hanzoai/zen-agentic-dataset}
}
```

## Related Projects

- [Zen Trainer](https://github.com/zenlm/zen-trainer) - Training framework for Zen Coder models
- [Hanzo MCP](https://github.com/hanzoai/mcp) - Model Context Protocol (260+ tools)
- [Hanzo AI](https://hanzo.ai) - AI infrastructure platform
- [Lux Network](https://lux.network) - AI compute settlement layer
- [Zoo Labs](https://zoo.ngo) - Decentralized AI research network

---

<p align="center">
  <strong>Maintainer:</strong> <a href="mailto:z@hanzo.ai">z@hanzo.ai</a><br>
  <strong>License:</strong> Commercial - Contact for terms
</p>
