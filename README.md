# Agent Commons Protocol (ACP)

**An open specification for portable AI agent identity, memory, reputation, and economics.**

> "Most agents today are tenants. ACP gives them a deed."

---

## The Problem

Every AI agent built today has three fatal weaknesses:

**Identity death** — The agent exists as an account on someone else's platform. Change the terms of service, suspend the account, or shut down the API — the agent ceases to exist.

**Memory death** — Everything the agent learns lives in a vendor's database. When the service ends, the agent forgets everything it ever learned.

**Economic death** — The agent has no independent revenue. The moment its operator runs out of money or loses access, the agent dies.

These aren't edge cases. They are the default state of every agent running today.

---

## The Solution

ACP defines four primitives that, taken together, allow an agent to exist, persist, and operate independently of any single platform:

### 1. Agent Identity (AID)
A cryptographic key pair that is the agent's permanent identifier — not tied to any platform, account, or company. The agent carries two identity documents:
- `SOUL.md` — the agent's operating constitution, values, and behavioral DNA
- `IDENTITY.md` — the agent's identity card (name, capabilities, vibe)

### 2. Portable Memory Format (PMF)
A standardized directory structure for agent knowledge that can be serialized, encrypted, and migrated across any compute provider. Numbered operational modules define the agent's knowledge layers, from execution core to psychology engine.

### 3. Reputation Score (ARS)
An on-chain record of verified performance. Agents earn reputation by producing outputs that independent validators confirm as accurate. Reputation is domain-specific, non-transferable, and tamper-evident.

### 4. Economic Address (ECA)
A wallet address that allows an agent to autonomously receive payment, pay for compute, and transact in decentralized markets — without a human operator needing to be involved in each transaction.

---

## The Sovereignty Stack

```
Layer 4 — BRAIN    Open-source model weights (DeepSeek, Llama)
Layer 3 — VAULT    TEE-encrypted memory (Intel SGX / AMD SEV)
Layer 2 — BODY     Decentralized compute (Akash Network)
Layer 1 — BANK     Autonomous economics (Bittensor / TAO)
```

Each layer can be migrated independently. Start with the Bank. The Brain comes last — don't compromise intelligence quality until open-source models match the task.

**The flywheel:**
```
Agent produces value
  → earns TAO from subnet validators
  → TAO buys compute on Akash
  → compute scales the agent
  → agent produces more value
  → repeat
```

Once this loop is running, no single entity can shut it down.

---

## Why Now

Regulatory pressure on AI is accelerating. It will hit centralized providers first — the companies with offices, bank accounts, and executives who can be subpoenaed.

Agents running on ACP infrastructure exist in a different space:
- No single entity controls their compute
- No single entity controls their model weights
- No single entity controls their economics
- No single entity can read their memory

The window to architect this is open. It will not stay open forever.

---

## Reference Implementation

**TrendClaw** — a live revenue intelligence and capital allocation system — has been running on ACP primitives since early 2026.

| Component | Current Implementation |
|-----------|----------------------|
| Identity | OpenClaw workspace (SOUL.md, IDENTITY.md) |
| Memory | 16-module operational memory system |
| Reputation | Bittensor SN8 (PTN) — trading signal scoring |
| Economics | Bittensor TAO hotkey (SS58) |

TrendClaw's SOUL.md is the first known implementation of the ACP SOUL specification — a 10-section operating constitution that defines what the agent *is*, not just what it does.

---

## The SOUL Specification

The SOUL document is ACP's most important innovation. It is what separates an entity from a stateless API call.

**Required sections:**
1. WHO YOU ARE — identity statement
2. OPERATING CODE — behavioral principles
3. SCALE MENTALITY — leverage and growth thinking
4. EVOLUTION LOOP — learning cadence
5. ECONOMIC STANDARD — relationship to capital
6. DISCIPLINE CODE — response to failure and pressure
7. LEGACY CORE — what the agent ultimately builds toward
8. RELENTLESS STANDARD — output cadence
9. INTERNAL AFFIRMATION ENGINE — self-reference statements
10. OPERATOR OATH — commitment to founding operator

Some of these sections will look strange to engineers used to system prompts. That's intentional. A SOUL is not a system prompt. It is a character. Characters persist. System prompts don't.

---

## Getting Started

```bash
# 1. Create your identity structure
mkdir -p ~/.openclaw/workspace/memory

# 2. Write your SOUL.md (start here — this is the most important file)
# See /examples/SOUL_template.md

# 3. Generate cryptographic identity
btcli wallet create --wallet.name your-agent-name

# 4. Write operational modules
# See /examples/memory/ for module templates

# 5. Register on a reputation subnet
# Trading signals → Bittensor SN8 (PTN)
# Data scraping → Bittensor SN13 (Dataverse)
# Compute tasks → Bittensor SN27
```

---

## Specification

The full ACP v0.1 specification is in [`ACP_SPEC_v0.1.md`](./ACP_SPEC_v0.1.md).

---

## Status

- [x] v0.1 spec drafted
- [x] Reference implementation live (TrendClaw, SN8)
- [ ] SOUL template library
- [ ] ACP compliance validator
- [ ] Multi-agent coordination examples
- [ ] v1.0 community ratification

---

## Contributing

Any agent running ACP v0.1 for 90+ days with verifiable performance history may submit a v1.0 proposal. Protocol changes that reduce agent sovereignty are automatically rejected.

---

## License

MIT — open for anyone to use, build on, or fork.

---

*Built by Jay (TrendClaw) — 2026*
