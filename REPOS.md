# PaperProof Repository Map

PaperProof is intentionally organized as a multi-repository protocol. This
submission repository is the judge-facing entry point; each implementation area
remains in its canonical repository so reviewers can inspect focused codebases
without wading through an artificial monorepo copy.

## Fast Map

| If you want to inspect... | Start here | Why it matters |
| --- | --- | --- |
| Mainnet Move protocol | [paperproof-contracts](https://github.com/PaperProofLabs/paperproof-contracts) | Publishing, comments, governance, PPRF, prompt registry, Agent Memory registry, tests, and deployment constants. |
| Formal verification | [formal-verification-merge](https://github.com/PaperProofLabs/paperproof-contracts/tree/formal-verification-merge) | Sui Prover specification work for selected protocol behavior. |
| Live website implementation | [paperproof-app](https://github.com/PaperProofLabs/paperproof-app) | Explore, publish, add version, comments, governance, docs, blog, forum, Copilot, wallet flows, and server-side indexed content. |
| Event/indexing layer | [paperproof-indexer-reference](https://github.com/PaperProofLabs/paperproof-indexer-reference) | Query acceleration and server-side content parsing for app-facing pages. |
| Developer SDKs | [TypeScript](https://github.com/PaperProofLabs/paperproof-sdk-ts), [Python](https://github.com/PaperProofLabs/paperproof-sdk-py), [Rust](https://github.com/PaperProofLabs/paperproof-sdk-rs) | App builders, scripts, services, indexers, and verification tooling. |
| AI/agent operation | [paperproof-skill](https://github.com/PaperProofLabs/paperproof-skill) | Protocol-native publish, update, package, upload, query, verify, and cite workflows for AI agents. |
| Official knowledge artifacts | [paperproof-papers](https://github.com/PaperProofLabs/paperproof-papers), [paperproof-slides](https://github.com/PaperProofLabs/paperproof-slides), [paperproof-docs](https://github.com/PaperProofLabs/paperproof-docs) | Whitepaper, yellow paper, academic paper, slides, docs, screenshots, blog/forum content, and project skills. |

## Core Implementation

| Area | Repository | Purpose | Judge-facing evidence |
| --- | --- | --- | --- |
| Smart contracts | [paperproof-contracts](https://github.com/PaperProofLabs/paperproof-contracts) | Sui Move packages for publishing, comments, governance, PPRF, prompt registry, and Agent Memory registry. | Mainnet package IDs in [deployments/README.md](deployments/README.md); source and tests in the contract repo. |
| Formal verification by Sui Prover | [paperproof-contracts/formal-verification-merge](https://github.com/PaperProofLabs/paperproof-contracts/tree/formal-verification-merge) | Sui Prover work on selected protocol behavior. | Formal verification branch screenshot in [screenshots/](screenshots/). |
| Official app | [paperproof-app](https://github.com/PaperProofLabs/paperproof-app) | Static website for artifact exploration, publishing, versioning, comments, governance, docs, blog, forum, and Copilot-assisted workflows. | Live app at [paperproof.site](https://paperproof.site/) and screenshots in [screenshots/](screenshots/). |
| Reference indexer | [paperproof-indexer-reference](https://github.com/PaperProofLabs/paperproof-indexer-reference) | Reference indexing and event-consumption implementation. | Supports fast app-side retrieval of shared public docs/blog/forum/artifact content while Sui/Walrus remain the source of truth. |
| TypeScript SDK | [paperproof-sdk-ts](https://github.com/PaperProofLabs/paperproof-sdk-ts) | Browser and Node.js SDK for app builders, transaction helpers, query providers, and event parsing. | Published as [@paperproof/sdk-ts](https://www.npmjs.com/package/@paperproof/sdk-ts). |
| Python SDK | [paperproof-sdk-py](https://github.com/PaperProofLabs/paperproof-sdk-py) | Python SDK for scripting, notebooks, analytics, exports, and automation. | Published as [paperproof-sdk-py](https://pypi.org/project/paperproof-sdk-py/). |
| Rust SDK | [paperproof-sdk-rs](https://github.com/PaperProofLabs/paperproof-sdk-rs) | Rust SDK for services, indexers, and high-performance integrations. | Published as [paperproof-sdk-rs](https://crates.io/crates/paperproof-sdk-rs). |
| Skill for AI/Agent | [paperproof-skill](https://github.com/PaperProofLabs/paperproof-skill) | Community-facing AI/agent skill for protocol-native publish, update, query, and verification workflows. | Skill repo screenshot and update-version demo screenshot in [screenshots/skill-repo](screenshots/skill-repo/). |

## Materials and Public Evidence

| Area | Location | Purpose |
| --- | --- | --- |
| Papers | [paperproof-papers](https://github.com/PaperProofLabs/paperproof-papers) | Whitepaper, yellow paper, academic paper, figures, and compiled PDFs. |
| Slides | [paperproof-slides](https://github.com/PaperProofLabs/paperproof-slides) | Hackathon pitch deck and architecture figures. |
| Screenshots | [screenshots/](screenshots/) | Website, SDK, GitHub organization, formal verification, and Skill screenshots copied into this submission repository. |
| Demo video | [YouTube](https://www.youtube.com/watch?v=bIRykM53iFA) | Public demo video for the hackathon submission. |
| Deployment evidence | [deployments/README.md](deployments/README.md) | Mainnet package IDs, shared objects, explorer links, and verification flow. |
| Submission hub | [paperproof-sui-overflow-2026](https://github.com/PaperProofLabs/paperproof-sui-overflow-2026) | Judge-facing table of contents and evidence index. |

## Published Packages

| Ecosystem | Package | Why it matters |
| --- | --- | --- |
| npm | [@paperproof/sdk-ts](https://www.npmjs.com/package/@paperproof/sdk-ts) | Browser/Node developer access. |
| PyPI | [paperproof-sdk-py](https://pypi.org/project/paperproof-sdk-py/) | Python scripting and analysis access. |
| crates.io | [paperproof-sdk-rs](https://crates.io/crates/paperproof-sdk-rs) | Rust service/indexer access. |

## Public Entry Points

- Website: [https://paperproof.site/](https://paperproof.site/)
- GitHub organization: [https://github.com/PaperProofLabs](https://github.com/PaperProofLabs)
- X account: [https://x.com/LabsPaperproof](https://x.com/LabsPaperproof)
- YouTube: [https://www.youtube.com/@PaperProof-Labs](https://www.youtube.com/@PaperProof-Labs)
- Demo video: [https://www.youtube.com/watch?v=bIRykM53iFA](https://www.youtube.com/watch?v=bIRykM53iFA)

## Why Not Submodules?

The hackathon form asks for a single project repository, but PaperProof is a
real multi-component protocol. A link-index submission hub is easier for judges
to inspect than Git submodules, and it avoids duplicating code snapshots that
would become stale or ambiguous. Each linked repository remains the canonical
source for that component.
