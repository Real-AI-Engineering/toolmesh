# AgentReplay (concept)

**One-liner:** A replay-first platform for **sanitized, forkable agent runs** across frameworks — “fork this run” turns agent execution into distribution.

## Problem

Agent work is hard to share, verify, and learn from:

- runs live in logs/chats, not portable artifacts
- “it worked on my agent” is not reproducible across toolchains
- teams can’t easily create a real-world eval dataset from production-like runs

## What it is

AgentReplay is a thin layer on top of ToolMesh receipts:

- a **universal uploader** (CLI/skill bundle) that exports a run as a shareable **Proofpack**
- **redaction-first** defaults (secrets/PII policies) so sharing is safe by design
- a web viewer that renders runs as short “replay posts” with diffs, tool calls, checks, and replay buttons
- optional challenges/leaderboards for standardized tasks (“speedruns for agents”)

## MVP (2 devs, realistic)

1) `agentreplay publish` — package + redact + upload a run (from local folder / receipt JSON)
2) Public run pages + fork button (download as Proofpack)
3) One standard challenge + leaderboard (minimal) to create a distribution loop

## Why it matters to ToolMesh

AgentReplay converts **proof** into a growth wedge:

- distribution via “fork this run”
- community benchmarks → better evals
- more receipts → stronger schemas + better governance primitives

## Business model (hypothesis)

- Open core viewer + uploader
- Paid: org spaces, team-private runs, advanced redaction, compliance logging, SSO, on-prem

## Open questions

- Which 1–2 frameworks to support first (to avoid scope creep)?
- Where to host: GitHub-backed artifacts vs dedicated storage?
- What is the minimal “challenge” that produces repeat usage?

