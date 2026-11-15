# PMP MCP Continuity

Experimental project continuity between agent applications through a shared local MCP mailbox.

**Status: documented local case study.** This repository publishes documentation and selected sanitized evidence. The MCP adapter implementation remains local and is not packaged here. There is no installable server in this repository yet.

On November 14, 2026, we completed a bounded task round trip: **Codex → Antigravity → Codex**. The recipient discovered its assignment through MCP, returned a linked result, and the sender received and closed it through MCP.

## Why this matters

Switching agent applications should not require the user to carry paths, instructions, hashes and receipts between chats. A shared inbox can carry the task and result while PMP documents preserve project context. Users still start agent turns; there is no background wake-up or unattended agent loop in this experiment.

## Read the case

- [Case study: workflow, real failures and boundaries](docs/CASE-STUDY.md)
- [Selected public evidence](evidence/PUBLIC-EVIDENCE.json)
- [SHA-256 manifest of these published documents](evidence/PUBLIC-MANIFEST.json)

Observed: one real task on one PC, completed in both directions, with verified package/receipt hashes. The implementation's local suites passed 22 tests. Project test results in the case were reported by Antigravity; Codex independently verified transport artifacts rather than rerunning those project tests.

## Relationship to PMP Handoff Bridge and the Hermes submission

This is a **separate, post-submission experiment** built around [PMP Handoff Bridge](https://github.com/Mad-Max8063/pmp-handoff-bridge), pinned locally at `04f04711dfc10edbf9e77bb98dd390ab03bea60c`.

This repository does not replace or update the Hermes plugin submission. Publishing it does not change the submitted repository, its pinned revision, catalog entry or demonstration. The Codex/Antigravity mailbox behavior described here is not claimed to be a feature shipped in that pinned Hermes plugin. No affiliation, endorsement or competition outcome is implied.

## Evidence boundaries

The public evidence is an unsigned summary of private local artifacts. Original project code, private packages, raw mailbox database, host configuration and personal paths are excluded. The source digests identify those original artifacts; the summary does not make the private project publicly reproducible.

This case does not establish agent identity, semantic understanding, production readiness, universal reliability or quantified savings. Agent sessions used their normal model quotas; total inference cost was not measured.

## Next steps

Repeat the workflow with another explicitly scoped task, measure user intervention and failure recovery, and review a clean distributable adapter before offering installation instructions.

Documentation licensed under MIT. No third-party runtime is distributed in this repository.
