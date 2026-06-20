# PaperProof Protocol - Sui Overflow 2026 Submission

PaperProof turns papers, datasets, technical reports, software releases, and
other long-lived digital works into durable protocol artifacts: each work gets a
stable Sui identity, versioned Walrus-backed content, verifiable provenance,
community interaction, SDK access, and agent-native operation.

The core idea is simple: important knowledge should not live as a fragile URL.
It should have a protocol identity that humans, apps, indexers, wallets, and AI
agents can all inspect and verify.

This repository is the judge-facing entry point for the PaperProof submission.
The implementation lives in focused repositories under the
[PaperProofLabs GitHub organization](https://github.com/PaperProofLabs), while
this hub links the live app, contracts, SDKs, papers, slides, demo materials,
and mainnet deployment evidence in one place.

## Why PaperProof

Research and technical artifacts are usually distributed through ordinary web
pages, PDF links, cloud files, git releases, or database records. Those systems
are useful, but they do not provide a shared protocol layer for identity,
versioning, storage references, verification, discussion, and future automation.

PaperProof adds that missing layer:

- A paper, dataset, report, or release gets a persistent `ArtifactSeries`
  identity on Sui.
- Every version is bound to content hashes, Walrus blob references, typed
  metadata, and protocol events.
- Community context such as comments, likes/dislikes, governance, and future
  curation can attach to the artifact itself.
- Developers can build apps, indexers, bots, dashboards, and research tooling
  from SDKs instead of scraping pages.
- AI agents can operate the protocol through a dedicated PaperProof Skill,
  lowering the barrier for ordinary users to publish and verify artifacts.

For judges, the project is not only "a website for papers." It is a working
artifact infrastructure stack that shows how Sui objects, Walrus storage, SDKs,
and agent workflows can become a common substrate for verifiable knowledge.

## Why Sui

PaperProof uses Sui where object-centric blockchain design matters most:
durable identities, version records, permissions, interaction objects,
governance state, and indexer-friendly events.

- `ArtifactSeries` objects represent stable artifact identity.
- Version objects record content hash, content type, metadata, and Walrus
  references.
- Comment trees, likes/dislikes, governance objects, prompt registry, and Agent
  Memory registry are modeled as protocol objects rather than off-chain-only
  app state.
- Sui events make artifact publication, version updates, comments, and
  governance actions queryable by SDKs and indexers.

If a hackathon form allows only one deployed package address, use the primary
publishing package:

```text
0xc9a75e4514db2a37df6f95b4e2b329c065ac6089953bd2c1c0a0c389835bd3d8
```

Additional mainnet package IDs and shared objects are listed in
[deployments/README.md](deployments/README.md).

## Why Walrus

Sui should not store large PDFs, datasets, source archives, or multimedia
payloads directly. PaperProof uses Walrus for durable content storage while Sui
records the verifiable binding between protocol state and stored bytes.

This split gives PaperProof a clean architecture:

- Sui records artifact identity, version metadata, hashes, permissions, and
  events.
- Walrus stores the large artifact content.
- The website, SDKs, and Skill connect the two so users can publish, retrieve,
  and verify artifacts without manually understanding every storage detail.

The result is stronger than a standalone blob store and more practical than
putting large files directly on chain.

## Agent-Native by Design

PaperProof includes a community-facing
[PaperProof Skill](https://github.com/PaperProofLabs/paperproof-skill) so AI
agents can interact with the protocol directly. The Skill can guide or perform
workflows such as preparing metadata, packaging local content, uploading to
Walrus, submitting Sui transactions, adding new artifact versions, querying
objects, and verifying results.

That matters because artifact infrastructure can be complex for normal users.
An agent can hide the operational complexity while preserving verifiability:
the final state is still on Sui and the bytes are still bound through Walrus
hashes and blob references.

This is also why PaperProof is more than a static publication website. It is a
protocol that can be used by humans through the website, by developers through
SDKs, and by agents through Skill-based workflows.

## Project Completeness

PaperProof is submitted as a working multi-component system, not a single
mockup or contract demo.

| Component | Status |
| --- | --- |
| Live website | [https://paperproof.site/](https://paperproof.site/) |
| Sui mainnet contracts | Deployed; see [deployment notes](deployments/README.md) |
| Walrus content workflow | Used for artifact content and version records |
| TypeScript SDK | Published on [npm](https://www.npmjs.com/package/@paperproof/sdk-ts) |
| Python SDK | Published on [PyPI](https://pypi.org/project/paperproof-sdk-py/) |
| Rust SDK | Published on [crates.io](https://crates.io/crates/paperproof-sdk-rs) |
| Skill for AI/Agent | [PaperProof Skill](https://github.com/PaperProofLabs/paperproof-skill) |
| Contracts | [paperproof-contracts](https://github.com/PaperProofLabs/paperproof-contracts) |
| Formal verification by Sui Prover | [paperproof-contracts/formal-verification-merge](https://github.com/PaperProofLabs/paperproof-contracts/tree/formal-verification-merge) |
| Papers | [whitepaper, yellow paper, academic paper](https://github.com/PaperProofLabs/paperproof-papers) |
| Slides | [paperproof-slides](https://github.com/PaperProofLabs/paperproof-slides) |
| Demo video | [YouTube](https://www.youtube.com/watch?v=OjRZrhqZ4ZY) |

## What Judges Can Verify Quickly

1. Open the live website: [https://paperproof.site/](https://paperproof.site/).
2. Inspect the primary Sui publishing package:
   `0xc9a75e4514db2a37df6f95b4e2b329c065ac6089953bd2c1c0a0c389835bd3d8`.
3. Check the SDKs on npm, PyPI, and crates.io.
4. Review the PaperProof Skill to see how an AI agent can operate the protocol.
5. Open the slides and papers for the architecture, protocol model, and design
   rationale.

## Start Here

| Item | Link |
| --- | --- |
| Live website | [paperproof.site](https://paperproof.site/) |
| GitHub organization | [github.com/PaperProofLabs](https://github.com/PaperProofLabs) |
| Project repo / submission hub | [paperproof-sui-overflow-2026](https://github.com/PaperProofLabs/paperproof-sui-overflow-2026) |
| Demo video | [YouTube](https://www.youtube.com/watch?v=OjRZrhqZ4ZY) |
| Pitch deck | [paperproof-slides](https://github.com/PaperProofLabs/paperproof-slides) |
| Papers | [paperproof-papers](https://github.com/PaperProofLabs/paperproof-papers) |
| Mainnet deployment notes | [deployments/README.md](deployments/README.md) |

## Repository Map

| Area | Repository |
| --- | --- |
| Sui Move contracts | [paperproof-contracts](https://github.com/PaperProofLabs/paperproof-contracts) |
| Formal verification by Sui Prover | [paperproof-contracts/formal-verification-merge](https://github.com/PaperProofLabs/paperproof-contracts/tree/formal-verification-merge) |
| Official website | [paperproof-app](https://github.com/PaperProofLabs/paperproof-app) |
| TypeScript SDK | [paperproof-sdk-ts](https://github.com/PaperProofLabs/paperproof-sdk-ts) |
| Python SDK | [paperproof-sdk-py](https://github.com/PaperProofLabs/paperproof-sdk-py) |
| Rust SDK | [paperproof-sdk-rs](https://github.com/PaperProofLabs/paperproof-sdk-rs) |
| Agent skill | [paperproof-skill](https://github.com/PaperProofLabs/paperproof-skill) |
| Reference indexer | [paperproof-indexer-reference](https://github.com/PaperProofLabs/paperproof-indexer-reference) |
| Docs and screenshots | [paperproof-docs](https://github.com/PaperProofLabs/paperproof-docs) |
| Papers | [paperproof-papers](https://github.com/PaperProofLabs/paperproof-papers) |
| Slides | [paperproof-slides](https://github.com/PaperProofLabs/paperproof-slides) |
| Screenshots | [screenshots/](screenshots/) |

See [REPOS.md](REPOS.md) for a fuller component-by-component map.

## Submission Materials

- [Project overview](docs/PROJECT_OVERVIEW.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Repository map](REPOS.md)
- [Deployment notes](deployments/README.md)
- [Demo script](demo/DEMO_SCRIPT.md)
- [Evidence checklist](evidence/EVIDENCE_CHECKLIST.md)
- [Judging checklist](SUBMISSION_CHECKLIST.md)

## License and Notice

This submission repository is governed by [LICENSE.md](LICENSE.md) and
[NOTICE.md](NOTICE.md). Linked repositories and packages are governed by their
own licenses.

PaperProof smart contract source code is source-available. Public availability
supports transparency, review, research, and interoperability, but does not
grant rights to copy, modify, redeploy, or commercialize the contract source
except as expressly permitted by the relevant contract license.

For user-content, app-display, takedown, wallet, AI, and risk boundaries, see
[docs/LEGAL_AND_SAFETY_BOUNDARIES.md](docs/LEGAL_AND_SAFETY_BOUNDARIES.md).
