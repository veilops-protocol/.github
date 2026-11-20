# Contributing to VEILOPS

Thank you for your interest. This file applies to every repository in `veilops-protocol` that does not have its own `CONTRIBUTING.md`.

## Where to contribute

During Phase 01 the single source of truth is [`veilops-protocol/veilops`](https://github.com/veilops-protocol/veilops). `veilops-sdk`, `veilops-proof-engine`, `veilops-explorer` and `veilops-docs` are read-only subtree mirrors: **open issues and pull requests on `veilops`**. Pull requests opened on a mirror will be closed with a pointer to the monorepo.

The detailed guide lives in the monorepo: [CONTRIBUTING.md](https://github.com/veilops-protocol/veilops/blob/main/CONTRIBUTING.md).

## Ground rules

1. Security issues are reported privately; see the [security policy](SECURITY.md).
2. Keep status labels honest (`planned`, `experimental`, `implemented`). Do not call the attestation signature a zero-knowledge proof, the range proof succinct or audited, or claim deployments that have not happened.
3. Do not implement cryptographic primitives by hand; changes to a proof format or transcript need a new proof-system version.
4. Every change ships with tests; verifier changes need negative tests.
5. Follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## Quick start

```bash
git clone https://github.com/veilops-protocol/veilops.git
cd veilops
nvm use && npm ci
npm run typecheck && npm run lint && npm test
```

By contributing you agree to license your work under the Apache License 2.0.
