# Judging Notes

## Suggested Evaluation Path

1. Read the root [README](../README.md), especially **Judge Quick View** and
   **What Judges Can Verify in 5 Minutes**.
2. Open the live app at [https://paperproof.site/](https://paperproof.site/).
3. Open a real artifact page and inspect metadata, downloads, version history,
   comments, likes, and explorer links.
4. Watch the [demo video](https://www.youtube.com/watch?v=bIRykM53iFA).
5. Inspect the [pitch deck PDF](https://github.com/PaperProofLabs/paperproof-slides/blob/main/paperproof-slides.pdf).
6. Check the [deployment notes](../deployments/README.md), primary publishing
   package, shared objects, and explorer links.
7. Check the SDK packages on npm, PyPI, and crates.io.
8. Inspect the [PaperProof Skill](https://github.com/PaperProofLabs/paperproof-community-skill)
   and the Copilot evidence to see the agent-native surface.

## What To Look For

- Real Sui mainnet deployment and verifiable package/object IDs.
- Walrus usage as the durable content layer for versioned artifact bytes.
- A practical website, not just a contract-only demo.
- Artifact versioning with content hashes, blob references, metadata, and
  protocol events.
- Comments, likes, governance, prompt registry, and Agent Memory registry as
  protocol surfaces rather than app-only UI state.
- Published SDKs for TypeScript, Python, and Rust.
- Agent-native operation through website Copilot and PaperProof Skill.
- PaperProof using itself in production: docs, blog, forum, papers, slides,
  SDK releases, Skill releases, datasets, and other materials are represented
  as PaperProof artifacts.
- Formal verification by Sui Prover in the
  [formal-verification-merge](https://github.com/PaperProofLabs/paperproof-contracts/tree/formal-verification-merge)
  branch.
- Event and object design suitable for indexers and ecosystem integrations.

## Track Fit

PaperProof fits the Special - Walrus track because it moves beyond raw blob
storage toward a reusable artifact provenance layer. Sui anchors artifact
identity, version lineage, commitments, interaction state, governance, and
registry events; Walrus stores the durable content bytes; the indexer and app
make shared public content fast to browse without becoming the trust root.

PaperProof also fits agentic workflows. The website Copilot helps humans use the
protocol, while the PaperProof Skill lets AI agents package, publish, update,
query, cite, and verify protocol artifacts directly.

## Important Boundary

The submission is multi-repository by design. This hub is the judge-facing entry
point; the linked repositories are the canonical implementation sources for each
component. This avoids stale copied code while still giving the hackathon form a
single project repository.
