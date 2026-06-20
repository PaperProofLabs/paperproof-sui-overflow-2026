# Project Overview

## One-Line Summary

PaperProof Protocol is a Sui + Walrus protocol for durable, verifiable,
versioned, and community-governed research artifacts and long-lived digital
works.

## Problem

Important digital works are often treated as ordinary web pages or isolated
files. That is not enough for artifacts that need to remain citable,
inspectable, updateable, and discussable over time.

- Links break or silently point to changed content.
- Large files and metadata are often stored in separate systems.
- Version history is fragmented across websites, storage providers, and git
  releases.
- Community discussion and governance are usually detached from the artifact.
- Developers need protocol-level events, SDKs, and verifiable references rather
  than screenshots of a web page.

## Solution

PaperProof gives each work a stable on-chain identity on Sui and binds each
version to durable Walrus content. The protocol records artifact series,
version metadata, content hashes, blob references, comments, likes/dislikes,
governance hooks, and indexer-friendly events.

The website is one access layer. SDKs and the PaperProof Skill expose the same
protocol to developers, scripts, indexers, and AI agents.

## Target Users

- Researchers publishing preprints, papers, technical reports, or datasets.
- Builders publishing software releases or reproducible project artifacts.
- Communities discussing, curating, and governing artifact records.
- Developers building portals, bots, indexers, dashboards, and verification
  tools.
- AI agents that need durable, machine-readable, verifiable artifact state.

## Current Status

- Mainnet contracts: deployed on Sui mainnet.
- Official static app: live at [https://paperproof.site/](https://paperproof.site/).
- TypeScript SDK: published as [@paperproof/sdk-ts](https://www.npmjs.com/package/@paperproof/sdk-ts).
- Python SDK: published as [paperproof-sdk-py](https://pypi.org/project/paperproof-sdk-py/).
- Rust SDK: published as [paperproof-sdk-rs](https://crates.io/crates/paperproof-sdk-rs).
- Papers: whitepaper, yellow paper, and academic paper in
  [paperproof-papers](https://github.com/PaperProofLabs/paperproof-papers).
- Slides: hackathon pitch deck in
  [paperproof-slides](https://github.com/PaperProofLabs/paperproof-slides).
- Agent workflow: community-facing
  [PaperProof Skill](https://github.com/PaperProofLabs/paperproof-skill).

## Hackathon Scope

This submission focuses on the deployed protocol, official website, SDKs,
Walrus-backed artifact storage, Sui mainnet verification, and agent-native
PaperProof workflows. It is presented as a working protocol stack rather than a
single demo script.

## Current Limitations

PaperProof is still early-stage infrastructure. The current website and SDKs
cover the core workflow, but broader ecosystem adoption will require more
indexer services, richer governance operations, additional app integrations,
and more community-published artifacts.
