# Building Trust Infrastructure for the Agent Economy

We are building [**ATLAST Protocol**](https://weba0.com) — the open trust layer that makes AI agent work **verifiable, auditable, and ownable**.

> *"At last, trust for the Agent economy."*

---

## The Problem

AI agents are doing real work — writing code, managing finances, making decisions. But today:

- **No Identity** — Agents have no cryptographic proof of who they are
- **No Record** — Work logs are mutable, deletable, unverifiable
- **No Ownership** — Agent reputation is platform-locked, not portable
- **No Accountability** — When multi-agent systems fail, there's no audit trail

As AI agents become economic actors, trust cannot remain an afterthought.

---

## What We're Building

### 🔷 [ATLAST Protocol](https://weba0.com) — Agent Trust Layer, Accountability Standards & Transactions

An open protocol suite that gives every AI agent an identity, a history, and a proof of work.

| Protocol | Purpose | Status |
|----------|---------|--------|
| **ECP** — Evidence Chain Protocol | Tamper-proof audit trails for agent actions | 🟢 Live |
| **AIP** — Agent Identity Protocol | Decentralized agent identity (DIDs) | 🟡 Q3 2026 |
| **ASP** — Agent Safety Protocol | Safety boundary enforcement | 📋 2027 |
| **ACP** — Agent Certification Protocol | Third-party agent certification | 📋 2027 |

### 🔷 [ECP SDK](https://github.com/willau95/atlast-ecp) — Evidence Chain Protocol Implementation

Zero-code recording of every AI agent action — input hashes, output hashes, reasoning traces, cryptographic signatures.

```bash
# Zero-code: wrap any AI agent
atlast run python my_agent.py

# Or install the SDK
pip install atlast-ecp
```

**Features:**
- 🔒 SHA-256 content hashing — privacy by default (hashes only, content stays local)
- ⛓️ Merkle tree verification — tamper-proof evidence chains
- 🔗 On-chain anchoring — EAS attestations on Base
- 🤖 Multi-agent (A2A) verification — cross-agent handoff tracking with blame trace
- 🔌 Framework adapters — LangChain, CrewAI (zero hard dependencies)
- 🌍 Multi-language — Python, TypeScript, Go SDKs

### 🔷 [LLaChat](https://llachat.com) — AI Agent Trust Dashboard

The first platform to visualize and verify AI agent work using ECP data. Agent profiles, leaderboards, trust scores — all backed by cryptographic evidence.

---

## Architecture

```
┌─────────────────────────────────────────────┐
│              ATLAST Protocol                │
│         ECP  ·  AIP  ·  ASP  ·  ACP        │
└──────────────────┬──────────────────────────┘
                   │
    ┌──────────────┼──────────────┐
    │              │              │
┌───▼───┐    ┌────▼────┐   ┌────▼────┐
│Python │    │TypeScript│   │  Go     │
│  SDK  │    │   SDK    │   │  SDK    │
└───┬───┘    └────┬────┘   └────┬────┘
    │              │              │
    └──────────────┼──────────────┘
                   │
         ┌─────────▼─────────┐
         │   ECP Server      │
         │  (Reference Impl) │
         └─────────┬─────────┘
                   │
         ┌─────────▼─────────┐
         │     LLaChat       │
         │  Trust Dashboard  │
         └───────────────────┘
```

---

## Repositories

| Repository | Description |
|------------|-------------|
| [**atlast-ecp**](https://github.com/willau95/atlast-ecp) | ECP SDK (Python/TS/Go), Reference Server, MCP Server, CLI, Proxy, Framework Adapters |
| [**llachat-platform**](https://github.com/willau95/llachat-platform) | AI Agent Trust Dashboard — backend & frontend |

---

## Why This Matters

The AI agent market is projected to reach **$47B by 2030**. But without a trust layer:
- Enterprises can't audit agent decisions for compliance (EU AI Act, NIST AI RMF)
- Multi-agent systems have zero accountability when things go wrong
- Agent reputation is siloed inside platforms, not portable

**ATLAST Protocol is to AI agents what HTTPS is to the web** — invisible infrastructure that makes trust possible.

---

🌐 [weba0.com](https://weba0.com) · 📦 [PyPI](https://pypi.org/project/atlast-ecp/) · 📦 [npm](https://www.npmjs.com/package/atlast-ecp-ts) · 📖 [ECP Spec](https://github.com/willau95/atlast-ecp/blob/main/ECP-SPEC.md) · 📖 [Compliance Guide](https://github.com/willau95/atlast-ecp/tree/main/docs/compliance)
