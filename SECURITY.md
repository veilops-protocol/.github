# Security Policy (veilops-protocol)

This policy applies to every repository in the `veilops-protocol` organization that does not define its own `SECURITY.md`.

## Project status

VEILOPS is **experimental** and **has not been audited** or externally reviewed. There are no releases and no production or mainnet deployments. Do not rely on it to protect real funds or real personal data.

## Reporting a vulnerability

**Do not open a public issue, discussion or pull request for a security problem.**

Report privately through GitHub Security Advisories:

1. Open the affected repository (for code, almost always [`veilops-protocol/veilops`](https://github.com/veilops-protocol/veilops), the source of truth; the other repositories are mirrors).
2. Go to **Security → Report a vulnerability**.
3. Include the affected package and file, the commit hash, the impact, and a minimal reproduction (ideally a vitest test).

A dedicated address, `security@veilops.tech`, is planned; until it is announced as active, use GitHub Security Advisories only.

## What to expect

- Acknowledgement, as a goal, within a few days.
- A published GitHub Security Advisory with credit (unless you prefer anonymity) once a fix is available.
- We ask for reasonable time before public disclosure; we suggest 90 days, or sooner once a fix ships.

There is **no bug bounty program**.

## Scope

In scope: the proof system (`veilops-range-v1`) and attestation, envelope encryption, policy enforcement, the SDK, the Solana memo adapter, canonicalization, and CI workflows.

Out of scope: metadata documented as public in the [security model](https://github.com/veilops-protocol/veilops/blob/main/docs/security.md), compromise of an operator's own keys, documented performance limitations, third-party dependency issues without demonstrated impact, the marketing site unless it exposes keys or user data, social engineering and denial of service against infrastructure.

## Safe harbor

We will not pursue action against researchers who act in good faith, avoid privacy violations and data destruction, and give us a reasonable chance to fix issues before disclosure.
