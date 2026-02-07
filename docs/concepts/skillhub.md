# SkillHub (concept)

**One-liner:** A registry of **verified skill bundles** (tool adapters + contracts + receipts) with a compatibility matrix — “works on my agent” guarantees.

## Problem

Agent tooling is fragmented:

- skill/tool adapters break across runtimes and versions
- teams re-implement the same glue (auth, schemas, retries, rate limits)
- there’s no standard way to prove a skill is safe (policy) and correct (eval)

## What it is

SkillHub is a distribution and governance layer for ToolMesh primitives:

- **bundles**: skill code + contract schema + tests/evals + redaction/policy rules
- **verification**: automated checks that produce a Proofpack (evidence) per release
- **compat matrix**: “supports Claude Code / OpenAI / LangGraph / …” with version pins
- **auto-updates**: safe rollouts (canary) + receipts when updating bundles

## MVP

- Bundle format + CLI to install/lock versions
- Basic verifier that runs tests/evals and emits receipts
- Simple registry UI (even GitHub-based) + compatibility table

## Why it matters to ToolMesh

SkillHub makes the “mesh” concrete: the glue becomes **packaged, testable, and enforceable**.

