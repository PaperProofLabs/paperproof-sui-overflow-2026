# Evidence Checklist

This checklist lists the evidence judges can inspect through the submission hub
and linked repositories.

## Five-Minute Verification Path

1. Open the live website: [https://paperproof.site/](https://paperproof.site/).
2. Open a real artifact page and inspect metadata, downloads, version history,
   comments, likes, and explorer links.
3. Verify the primary Sui mainnet publishing package:
   `0xc9a75e4514db2a37df6f95b4e2b329c065ac6089953bd2c1c0a0c389835bd3d8`.
4. Check the SDK releases on npm, PyPI, and crates.io.
5. Review the PaperProof Skill, website Copilot, deployment notes, and demo
   video.

## App Evidence

- Live website: [https://paperproof.site/](https://paperproof.site/)
- Website repository: [paperproof-app](https://github.com/PaperProofLabs/paperproof-app)
- Screenshots in this submission repo: [screenshots/](../screenshots/)
- Demo video: [YouTube](https://www.youtube.com/watch?v=bIRykM53iFA)
- Slides with architecture and website screenshots:
  [paperproof-slides](https://github.com/PaperProofLabs/paperproof-slides)

## Chain Evidence

- Mainnet deployment notes: [deployments/README.md](../deployments/README.md)
- Primary publishing package:
  `0xc9a75e4514db2a37df6f95b4e2b329c065ac6089953bd2c1c0a0c389835bd3d8`
- Publishing package on SuiVision:
  [open package](https://suivision.xyz/package/0xc9a75e4514db2a37df6f95b4e2b329c065ac6089953bd2c1c0a0c389835bd3d8)
- Publishing package on Suiscan:
  [open object](https://suiscan.xyz/mainnet/object/0xc9a75e4514db2a37df6f95b4e2b329c065ac6089953bd2c1c0a0c389835bd3d8)
- Root object, type registry, governance objects, prompt registry, and memory
  registry are listed in [deployments/README.md](../deployments/README.md).

## Walrus and Artifact Evidence

- Artifact pages expose Walrus-backed content references, hashes, metadata, and
  version records through the app and protocol state.
- PaperProof's own whitepaper, yellow paper, academic paper, slides, docs, blog,
  forum content, SDK releases, Skill releases, and datasets are represented as
  PaperProof artifacts.
- Server-side indexing accelerates shared public pages; Sui and Walrus remain
  the verification roots.

## SDK Evidence

- npm: [@paperproof/sdk-ts](https://www.npmjs.com/package/@paperproof/sdk-ts)
- PyPI: [paperproof-sdk-py](https://pypi.org/project/paperproof-sdk-py/)
- crates.io: [paperproof-sdk-rs](https://crates.io/crates/paperproof-sdk-rs)
- SDK screenshots: [screenshots/sdks/](../screenshots/sdks/)

## AI/Agent Evidence

- PaperProof Skill repository:
  [paperproof-community-skill](https://github.com/PaperProofLabs/paperproof-community-skill)
- PaperProof Skill artifact page:
  [software release artifact](https://paperproof.site/#/artifact/PaperProof-software_release-001162-c5930499d055)
- Skill screenshots: [screenshots/skill-repo/](../screenshots/skill-repo/)
- Copilot screenshot: [screenshots/11-copilot-open.png](../screenshots/11-copilot-open.png)

## Materials Evidence

- Papers: [paperproof-papers](https://github.com/PaperProofLabs/paperproof-papers)
- Slides PDF:
  [paperproof-slides.pdf](https://github.com/PaperProofLabs/paperproof-slides/blob/main/paperproof-slides.pdf)
- Demo video: [YouTube](https://www.youtube.com/watch?v=bIRykM53iFA)
- Formal verification by Sui Prover:
  [paperproof-contracts/formal-verification-merge](https://github.com/PaperProofLabs/paperproof-contracts/tree/formal-verification-merge)

## Security Review Before Submission

- Do not include private keys, mnemonics, API keys, local `.env` files, or
  unreleased credentials in screenshots or videos.
- Keep wallet addresses and public package/object IDs visible only where they
  are intentionally part of the verification evidence.
- Do not imply official endorsement by Sui, Walrus, OpenZeppelin, or any package
  registry beyond the public facts linked in this repository.
