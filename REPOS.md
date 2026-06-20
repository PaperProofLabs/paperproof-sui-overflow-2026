# PaperProof Repository Map

PaperProof is intentionally organized as a multi-repository project. This
submission repository is the entry point; each implementation area remains in a
focused repository so judges can inspect the contracts, website, SDKs, papers,
and demo assets without wading through an artificial monorepo copy.

## Core Implementation

| Area | Repository | Purpose |
| --- | --- | --- |
| Smart contracts | [paperproof-contracts](https://github.com/PaperProofLabs/paperproof-contracts) | Sui Move packages for publishing, comments, governance, PPRF, prompt registry, and Agent Memory registry. |
| Formal verification by Sui Prover | [paperproof-contracts/formal-verification-merge](https://github.com/PaperProofLabs/paperproof-contracts/tree/formal-verification-merge) | Sui Prover work on the contract codebase. |
| Official app | [paperproof-app](https://github.com/PaperProofLabs/paperproof-app) | Static website for artifact exploration, publishing, versioning, comments, governance, docs, and Copilot-assisted workflows. |
| Reference indexer | [paperproof-indexer-reference](https://github.com/PaperProofLabs/paperproof-indexer-reference) | Reference indexing and event-consumption implementation. |
| TypeScript SDK | [paperproof-sdk-ts](https://github.com/PaperProofLabs/paperproof-sdk-ts) | Browser and Node.js SDK for app builders, transaction helpers, query providers, and event parsing. |
| Python SDK | [paperproof-sdk-py](https://github.com/PaperProofLabs/paperproof-sdk-py) | Python SDK for scripting, notebooks, analytics, exports, and automation. |
| Rust SDK | [paperproof-sdk-rs](https://github.com/PaperProofLabs/paperproof-sdk-rs) | Rust SDK for systems, services, indexers, and high-performance integrations. |
| Skill for AI/Agent | [paperproof-skill](https://github.com/PaperProofLabs/paperproof-skill) | Community-facing AI/agent skill for protocol-native publish, update, query, and verification workflows. |

## Materials

| Area | Repository | Purpose |
| --- | --- | --- |
| Papers | [paperproof-papers](https://github.com/PaperProofLabs/paperproof-papers) | Whitepaper, yellow paper, and academic paper. |
| Slides | [paperproof-slides](https://github.com/PaperProofLabs/paperproof-slides) | Hackathon pitch deck and figures. |
| Screenshots | [screenshots/](screenshots/) | Website, SDK, GitHub organization, formal verification, and Skill screenshots copied into this submission repository. |
| Demo video | [YouTube](https://www.youtube.com/watch?v=OjRZrhqZ4ZY) | Public demo video for the hackathon submission. |
| Submission hub | [paperproof-sui-overflow-2026](https://github.com/PaperProofLabs/paperproof-sui-overflow-2026) | Judge-facing table of contents and deployment evidence. |

## Published Packages

| Ecosystem | Package |
| --- | --- |
| npm | [@paperproof/sdk-ts](https://www.npmjs.com/package/@paperproof/sdk-ts) |
| PyPI | [paperproof-sdk-py](https://pypi.org/project/paperproof-sdk-py/) |
| crates.io | [paperproof-sdk-rs](https://crates.io/crates/paperproof-sdk-rs) |

## Public Entry Points

- Website: [https://paperproof.site/](https://paperproof.site/)
- GitHub organization: [https://github.com/PaperProofLabs](https://github.com/PaperProofLabs)
- X account: [https://x.com/LabsPaperproof](https://x.com/LabsPaperproof)

## Why Not Submodules?

The hackathon form asks for a single project repository, but PaperProof is a
real multi-component protocol. A link-index submission hub is easier for judges
to inspect than Git submodules, and it avoids duplicating code snapshots that
would become stale or ambiguous. Each linked repository remains the canonical
source for that component.
