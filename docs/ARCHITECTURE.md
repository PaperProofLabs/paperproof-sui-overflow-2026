# Architecture

## High-Level Architecture

TODO: Add a diagram or screenshot from the pitch deck.

PaperProof combines:

- Sui protocol objects for identity, state, governance, and events.
- Walrus content blobs and Walrus Sites for durable storage and static hosting.
- SDKs for developers, apps, scripts, and indexers.
- A static official application as the first user-facing entry point.
- Optional AI assistance through PaperProof Copilot in the web app.

## On-Chain Object Model

TODO: Summarize the actual contract object model.

Suggested structure:

- `PaperProofRoot`
- `TypeRegistry`
- `TypeInfo`
- `TypeIndex`
- `ArtifactSeries`
- typed version records
- `CommentsTree`
- `LikesBook`
- `GovernanceVault`
- proposals and voting records
- `FeeManager`

Important note:

`TypeRegistry` records enabled artifact types and TypeIndex IDs. It does not
directly own all `ArtifactSeries` objects. Each `ArtifactSeries` stores its
artifact type, and indexers rebuild artifact discovery from emitted events.

## SDK Architecture

TODO: Explain the three SDKs and why they exist.

- TypeScript SDK: frontend, browser wallet, Node.js scripts, watch/query APIs.
- Python SDK: notebooks, CSV/JSON export, research scripts, operational tools.
- Rust SDK: high-throughput indexers, checkpoint ingestion, DB sinks, services.

## Query and Indexing Strategy

TODO: Explain GraphQL/gRPC/query providers, deployment manifests, event IDs,
and indexer-friendly design.

## Trust and Safety Model

TODO: Explain what users should verify, what the SDK validates, and what the
protocol records on chain.
