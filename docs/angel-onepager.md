# ToolMesh — Prompts → Proof

**One-liner:** ToolMesh builds **agent-native SDLC primitives** (contracts, receipts, replay) so teams can ship AI-agent work with **enterprise-grade reliability** — without inventing new models.

## The problem

Most tooling and operating models were built for humans. When the *executor* becomes an AI agent, teams hit the same wall:

- work lives in chat threads, not **machine-readable contracts**
- changes ship without **replayable evidence** (what happened, what tools/data were used, why it’s safe)
- no deterministic **quality gates** for agent behavior (evals, policy, least privilege, audits)

The result: agent projects stall at “demo”, or regress in production because they can’t be verified like normal software.

## The idea

Replace “prompt-and-pray” with **proof-carrying delivery**:

`Contract → Execute → Receipts → Replay/Verify (CI) → Ship + Observe`

Humans can audit; CI and agents can *consume* the artifacts.

## Flagship wedge (v0): ReceiptCI / Proofpack

**ReceiptCI** is a CI gate for agent-produced work.

Every agent change must include a **Proofpack**:

- **Contract** (inputs/outputs, constraints, acceptance gates)
- **Receipts** (tool calls, diffs, test results, eval outputs, provenance)
- **Replay path** (how CI can re-run verification deterministically)
- **Redaction rules** (share-safe by default; enterprise-grade sanitization)

This turns agent work into something teams can review, rerun, and trust.

## Who it’s for (ICP)

Teams shipping agent workflows inside real systems:

- platform / infra teams enabling internal automation
- AI/ML engineering teams productizing agent workflows
- backend teams integrating agents into ops, support, and developer tooling

## Why we win

- **Adapters over models:** glue around existing runtimes/models (fast iteration, low burn).
- **Proof as a first-class artifact:** receipts + replay become the unit of progress.
- **Agent-native contracts:** machine-readable specs that agents and CI can enforce.
- **Lab → cases → product:** we build “test rigs” and productize what repeats.

## Business model

1) **Agent-to-Prod Sprint (2–4 weeks)** — paid engagement to ship the first production use-case and install the loop.
2) **Product subscription** — ReceiptCI/Proofpack hosted or self-hosted with enterprise controls (policy, audit, redaction, SSO).

## Why now

- LLM costs dropped; adoption moved from pilots to “ship it”
- agent frameworks proliferate, but **verification + governance** is missing
- enterprises need auditable, deterministic gates before agents can touch production

## Team

Small team (2 devs) focused on **engineering discipline**: CI primitives, contracts, and interoperability — not training models.

## Ask

- Intros to teams running (or about to run) agent workflows in production
- 2–3 pilot partners for the Agent-to-Prod Sprint
- Early angel conversations around a pre-seed to productize ReceiptCI/Proofpack

**Links**

- Org: https://github.com/Real-AI-Engineering (rebranding to ToolMesh)
- Repo hub: https://github.com/Real-AI-Engineering/toolmesh
