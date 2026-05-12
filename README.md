# PaperProof Protocol - Sui Overflow 2026 Submission

Official Sui Overflow 2026 submission hub for PaperProof Protocol: a Sui +
Walrus protocol for durable, verifiable, and community-governed research
artifacts, with mainnet contracts, SDKs, a static Walrus Sites app, and demo
materials.

This repository is the judge-facing entry point. The implementation is split
across focused repositories so contracts, SDKs, frontend code, documentation,
and pitch materials can evolve independently.

PaperProof Protocol refers to the open protocol layer and official deployed
protocol instances. PaperProof Labs refers to the originating team and
maintainer of the official interface, SDKs, reference indexer, documentation,
and brand identity.

## Quick Links

- Live app: TODO
- Demo video: TODO
- Pitch deck: TODO
- Mainnet deployment manifest: TODO
- TypeScript SDK on npm: TODO
- Contracts repository: TODO
- Official app repository: TODO
- TypeScript SDK repository: TODO
- Python SDK repository: TODO
- Rust SDK repository: TODO

## What PaperProof Is

PaperProof gives long-lived digital works an on-chain protocol identity. A work
can have typed versions, durable Walrus content, provenance, discussion,
likes/dislikes, governance hooks, SDK access, and indexer-friendly events.

The first official application focuses on research and publication-like
artifacts, but the protocol is intentionally broader: preprints, blog posts,
technical reports, datasets, software releases, and generic files can all use
the same identity and interaction model.

## Why Sui and Walrus

Sui provides object-centric state, low-cost interaction, and high-throughput
execution for protocol objects, governance, comments, and indexed events.
Walrus provides durable storage and distribution for the actual content files.

PaperProof combines them:

- Sui records identity, references, versions, permissions, governance, and
  events.
- Walrus stores large artifacts such as PDFs, datasets, archives, and long-form
  content.
- SDKs and apps make the protocol usable without requiring users to understand
  every Move object or storage detail.

## Repository Map

See [REPOS.md](REPOS.md) for the full list of implementation repositories and
what each one contains.

## Submission Materials

- [Project overview](docs/PROJECT_OVERVIEW.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Demo script](demo/DEMO_SCRIPT.md)
- [Video plan](demo/VIDEO_PLAN.md)
- [Evidence checklist](evidence/EVIDENCE_CHECKLIST.md)
- [Deployment notes](deployments/README.md)
- [Judging checklist](SUBMISSION_CHECKLIST.md)

## License and Notice

This submission repository is governed by [LICENSE.md](LICENSE.md) and
[NOTICE.md](NOTICE.md). Linked repositories and packages are governed by their
own licenses.

In particular, PaperProof smart contract source code is source-available, not
permissively open-source. Public availability supports transparency, review,
research, and interoperability, but does not grant rights to copy, modify,
redeploy, or commercialize the contract source except as expressly permitted by
the relevant contract license.

For user-content, app-display, takedown, wallet, AI, and risk boundaries, see
[docs/LEGAL_AND_SAFETY_BOUNDARIES.md](./docs/LEGAL_AND_SAFETY_BOUNDARIES.md).
