# Judging Notes

## Suggested Evaluation Path

1. Read the root [README](../README.md).
2. Open the live app at [https://paperproof.site/](https://paperproof.site/).
3. Watch the [demo video](https://www.youtube.com/watch?v=bIRykM53iFA).
4. Inspect the [pitch deck](https://github.com/PaperProofLabs/paperproof-slides).
5. Check the [contracts](https://github.com/PaperProofLabs/paperproof-contracts)
   and [deployment notes](../deployments/README.md).
6. Check the SDK packages on npm, PyPI, and crates.io.

## What To Look For

- Real Sui mainnet deployment and verifiable package/object IDs.
- Walrus usage for durable artifact bytes and static-site-oriented delivery.
- A practical website, not just a contract-only demo.
- Artifact versioning with content hashes and blob references.
- Published SDKs for TypeScript, Python, and Rust.
- Agent-native operation through PaperProof Skill.
- Formal verification by Sui Prover in the
  [formal-verification-merge](https://github.com/PaperProofLabs/paperproof-contracts/tree/formal-verification-merge)
  branch.
- Event and object design suitable for indexers and ecosystem integrations.

## Track Fit

PaperProof fits the Sui/Walrus infrastructure story because it uses Sui for
object identity, version records, events, comments, governance, and interaction
state, while using Walrus for large artifact content. It also fits agentic
workflows: the PaperProof Skill lets an AI agent package, publish, update,
query, and verify protocol artifacts directly for users.

## Important Boundary

The submission is multi-repository by design. This hub is the judge-facing
entry point; the linked repositories are the canonical implementation sources
for each component.
