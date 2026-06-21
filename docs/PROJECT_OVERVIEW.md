# Project Overview

## One-Line Summary

PaperProof Protocol is a live Sui + Walrus provenance layer for durable,
verifiable, versioned, and community-governed knowledge artifacts.

## Tagline

Git-style version history, Walrus-backed content, and Sui-anchored provenance
for papers, datasets, software releases, reports, blogs, forums, and
AI-generated knowledge.

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
- AI agents need exact, durable, machine-readable artifact state for citation,
  verification, and automated workflows.

## Solution

PaperProof gives each work a stable on-chain identity on Sui and binds each
version to durable Walrus content. The protocol records artifact series,
version metadata, content hashes, blob references, comments, likes/dislikes,
governance hooks, prompt and memory registries, and indexer-friendly events.

The website is one access layer. SDKs and the PaperProof Skill expose the same
protocol to developers, scripts, indexers, third-party portals, and AI agents.

## Live Today

| Surface | Status |
| --- | --- |
| Mainnet contracts | Publishing, comments, governance, PPRF, prompt registry, and Agent Memory registry deployed on Sui mainnet. |
| Official website | Live at [paperproof.site](https://paperproof.site/). |
| Walrus-backed content | Used for papers, slides, docs, blogs, forum content, software releases, datasets, and versioned artifact payloads. |
| SDKs | TypeScript, Python, and Rust SDKs published on npm, PyPI, and crates.io. |
| AI/Agent | Configurable website Copilot with MemWal-backed memory plus the external PaperProof Skill. |
| Protocol materials | Whitepaper, yellow paper, academic paper, slides, screenshots, demo video, and deployment evidence are public. |

## Target Users

- Researchers publishing preprints, papers, technical reports, or datasets.
- Builders publishing software releases or reproducible project artifacts.
- Communities discussing, curating, and governing artifact records.
- Developers building portals, bots, indexers, dashboards, and verification
  tools.
- AI agents that need durable, machine-readable, verifiable artifact state.

## What Makes It Different

PaperProof is not a file upload app or a simple Walrus blob demo. It is a
protocol surface for durable artifact provenance:

- Sui anchors identity, lineage, commitments, governance, comments, likes, and
  events.
- Walrus stores large content bytes efficiently.
- The indexer makes shared public pages fast without becoming the trust root.
- SDKs make the protocol usable by applications and services.
- Copilot and Skill workflows make the protocol usable by humans and AI agents.
- PaperProof uses itself in production: its own docs, blog, forum posts, papers,
  slides, SDK releases, datasets, and Skill releases are represented as
  PaperProof artifacts.

## Hackathon Scope

This submission focuses on the deployed protocol, official website, SDKs,
Walrus-backed artifact storage, Sui mainnet verification, server-side indexed
content, and agent-native PaperProof workflows. It is presented as a working
protocol stack rather than a single demo script.

## Current Limitations

PaperProof is still early-stage infrastructure. The current website and SDKs
cover the core workflow, but broader ecosystem adoption will require more
third-party portals, richer governance operations, additional app integrations,
more community-published artifacts, and continued hardening of indexing and
agent workflows.
