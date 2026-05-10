# PaperProof Repository Map

This repository is the submission hub. The actual implementation lives in
focused repositories.

## Core Implementation

| Area | Repository | Purpose | Status |
| --- | --- | --- | --- |
| Smart contracts | TODO | Sui Move contracts for publishing, comments, governance, and protocol state. | TODO |
| Official app | TODO | Static frontend intended for Walrus Sites deployment. | TODO |
| TypeScript SDK | TODO | Browser and Node.js SDK for frontend apps, scripts, query providers, transaction builders, and watch APIs. | TODO |
| Python SDK | TODO | Scripting, analytics, export, notebook, and integration-oriented SDK. | TODO |
| Rust SDK | TODO | High-performance indexer, service, and systems-oriented SDK. | TODO |
| Slides | TODO | Pitch deck and presentation materials. | TODO |

## Package and Deployment Links

- npm package: TODO
- PyPI package: TODO
- crates.io package: TODO
- Walrus Sites URL: TODO
- Sui mainnet package/object manifest: TODO
- Sui Explorer evidence: TODO
- Walrus blob evidence: TODO

## Notes for Judges

The project is intentionally multi-repository. This keeps each component
focused and reviewable:

- Contracts can be audited separately from frontend code.
- SDKs can be published and versioned independently.
- The official app can remain a low-maintenance static site.
- The Rust SDK can evolve toward high-performance indexer use cases.

This submission hub should be read as the table of contents for the full
PaperProof project.
